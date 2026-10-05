# SHOPFLIX Backend

SHOPFLIX is an online marketplace backend built with Node.js, Express, PostgreSQL, Paystack, JWT authentication, and Cloudinary.

## Features

- Customer registration and login
- JWT authentication
- Customer, seller, and admin roles
- Product listing
- Seller product uploads and management
- Product stock management
- Orders
- Paystack payments and verification
- Admin user and role management
- Admin order status management

## Render Environment Variables

Configure these on Render:

- `DATABASE_URL`
- `PAYSTACK_SECRET_KEY`
- `JWT_SECRET`

Never put real secret values in this README or in GitHub.

## Render Settings

Build Command:

`npm install`

Start Command:

`npm start`

## API

- `GET /`
- `GET /api/health`
- `POST /api/auth/register`
- `POST /api/auth/login`
- `GET /api/auth/me`
- `GET /api/products`
- `GET /api/products/:id`
- `POST /api/products`
- `GET /api/seller/products`
- `POST /api/orders`
- `POST /api/payments/initialize`
- `GET /api/payments/verify/:reference`
- `GET /api/orders/:id`
- `GET /api/admin/users`
- `PATCH /api/admin/users/:id/role`
- `PATCH /api/orders/:id/status`

## Health Check

After deployment, open `/api/health`.

Expected:

```json
{
  "status": "ok",
  "database": "connected",
  "paystack": "configured",
  "jwt": "configured"
}
```
