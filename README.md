# Product CRUD API (Node.js + Express + Mongoose)

## Overview
Simple REST API to perform CRUD operations on a `products` collection using Mongoose and MongoDB.

## Requirements
- Node.js >= 18 recommended
- MongoDB instance (local or cloud). Example: mongodb://localhost:27017/products_db

## Setup
1. Copy `.env.example` to `.env` and update `MONGO_URI` if needed.
2. Install dependencies:
   ```bash
   npm install
   ```
3. Run the app (development):
   ```bash
   npm run dev
   ```
   or production:
   ```bash
   npm start
   ```

## API Endpoints
- `GET /products` - list products
- `POST /products` - create product (JSON body: `{ name, price, category }`)
- `GET /products/:id` - get product by id
- `PUT /products/:id` - update product by id
- `DELETE /products/:id` - delete product by id

## Notes
- Schema validation errors return HTTP 400 with details.
- Ensure MongoDB is reachable at `MONGO_URI` in `.env`.
