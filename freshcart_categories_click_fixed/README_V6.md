# FreshCart v6 — Large Grocery E-commerce Demo

FreshCart v6 is a full-stack grocery e-commerce project with a large generated catalogue and production-style shopping flows.

## Included
- 582 catalogue products across 20 grocery categories
- Search, category, brand, price, rating and stock filters
- Pagination and sorting
- Product details, wishlist, compare and recently viewed
- Cart quantity/stock validation
- Saved addresses and PIN serviceability check
- Delivery slots and order tracking
- Account registration/login with hashed passwords
- Order cancellation and review API
- Admin inventory endpoints
- Razorpay-ready online payments plus explicit demo fallback when keys are absent
- Responsive UI and icon-based navigation

## Run
```bash
cd backend
npm install
npm start
```
Open http://localhost:5000

## Razorpay
Copy `.env.example` to `.env` and set test credentials:
```text
RAZORPAY_KEY_ID=...
RAZORPAY_KEY_SECRET=...
```
Without keys, online payment uses a clearly labelled demo flow. A real charge is only possible after configuring your Razorpay merchant account and completing the provider's verification/onboarding requirements.

## Important production steps
The included JSON database is a development/demo database. For a production deployment, move users, sessions, products, inventory and orders to MongoDB/PostgreSQL, add secure cookie/JWT session handling, rate limiting, CSRF/CORS policy, webhook-based payment confirmation, image CDN/storage, backups, monitoring and real delivery-zone logic.
