# FreshCart v5.2 — API + Expanded Grocery Catalogue

## Run
1. Install Node.js 18+.
2. Open a terminal in `backend`.
3. Run `npm install`.
4. Run `npm start`.
5. Open `http://localhost:5000`.

## API
- GET /api/products
- GET /api/products?category=Vegetables
- GET /api/products/:id
- POST /api/auth/register
- POST /api/auth/login
- GET /api/addresses
- POST /api/addresses
- GET /api/orders
- POST /api/orders
- PATCH /api/admin/products/:id/stock

## Catalogue changes
The Vegetables category now contains 30 products, including Tomato, Potato, Carrot, Broccoli, Capsicum, Onion, Brinjal, Ladies Finger, Cauliflower, Cabbage, Spinach, Beans, Beetroot, Radish, Cucumber, Green Peas, Pumpkin, Bottle Gourd, Bitter Gourd, Ridge Gourd, Sweet Corn, Garlic, Ginger, Green Chilli, Coriander, Mint, Spring Onion, Drumstick, Yam and Raw Banana.

Stock is intentionally different per product. The order API stores product name, brand, unit, price, image and quantity as a snapshot, so tracking pages can show exactly what was ordered and how many.
