---
title: Title
description: Desc
date: 2025-09-14T20:12:52+08:00
lastmod: 2025-09-14T20:12:52+08:00
tags:
  - blog
  - github
categories:
  - dev
---

2025-10-02
Tags: #server #caching 

# IoRedis

Redis client for [[Node.js]]  

### Install with npm 

```bash
npm i ioredis 
```

### Create & export Instance at app.js

```javascript
const Redis = require('redis');
export const redis = new Redis({
	host: process.env.REDIS_HOST,
	port: process.env.REDIS_PORT,
	password: process.env.REDIS_PASSWORD,
});
```

### Log message when connected 

```javascript
redis.on("connect", () => {
	console.log("Redis connected");
})
```

View Example usage for IoRedis functions at [IoRedis](https://github.com/redis/ioredis/tree/561f3540e7161455a1d19aea14f5cb3fd6ae9dcd/examples)
All methods listed here too [IoRedis](https://redis.github.io/ioredis/classes/Redis.html)

### Basic usage with express 

```javascript
app.get("/products", async (req, res) => {
	let products = await redis.get("products");
	// if products found in redis memory return them	
	if (products) {
		console.log("Got from cache");
		return res.json({
			products: JSON.parse(products);
		});
	}
	// if not found query the main db
	products = await Product.find({});
	// cache the products
	await redis.set("products", JSON.stringify(products));
	res.json({products});
})
```

ps: learn about [[JSON]] methods 

### Caching with expiration

```javascript
app.get("/product/:id", async (req, res) => {
	const id = req.params.id;
	const key = `product:${id}`;
	let product = await redis.get(key);
	
	if (product) {
		return res.json({
			product: JSON.parse(product)
		});
	}
	
	product = await Product.findById(id);
	await redis.setex(key, 200, JSON.stringify(product));
	res.json({product});
})
```

