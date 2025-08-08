# 🛒 Shopping Cart Frontend

A fully functional **shopping cart** web application built with modern web technologies and connected to a custom mock REST API hosted on [Render](https://render.com).  
The app allows users to browse products, view details, add items to the cart, and adjust quantities — all with a responsive and clean UI.

---

## 🚀 Live Demo
Frontend: **https://shopping-cart-ui-pi.vercel.app/**  
API: **https://mock-api-zk2c.onrender.com/products**

---

## 📦 Features
- **Product Listing** — Displays all products from the mock API with images, names, categories, prices, ratings, and descriptions.
- **Product Details** — View full product descriptions and ratings.
- **Add to Cart** — Add items directly from the product list or detail view.
- **Cart Management** — Update quantities or remove items from the cart.
- **Responsive Design** — Works seamlessly on desktop and mobile.
- **Real API Integration** — Uses the deployed JSON Server mock API.

---

## 🗂 Project Structure
shopping-cart/
├── public/
│ ├── product-1.png
│ ├── product-2.png
│ └── ...
├── src/
│ ├── components/ # UI components
│ ├── pages/ # Page views
│ ├── hooks/ # Custom hooks
│ ├── styles/ # CSS/Tailwind styles
│ ├── App.js
│ └── index.js
├── package.json
└── README.md

yaml
Copy
Edit

---

## 🔌 API Example
The mock API returns data from the `db.json` file:  
```json
{
  "id": 1,
  "name": "Wireless Headphones",
  "description": "Noise-cancelling headphones with deep bass and Bluetooth 5.0 support.",
  "price": 59.99,
  "quantity": 25,
  "category": "Audio",
  "rating": 4.5,
  "image": "/product-1.png"
}
API Endpoints:

bash
Copy
Edit
GET    /products
GET    /products/:id
POST   /products
PUT    /products/:id
PATCH  /products/:id
DELETE /products/:id
💻 Local Development
Clone the repo and install dependencies:

bash
Copy
Edit
git clone https://github.com/<your-username>/<your-frontend-repo>.git
cd <your-frontend-repo>
npm install
Start the app locally:

bash
Copy
Edit
npm start
🌐 Environment Variables
To switch between local development and production API:

env
Copy
Edit
REACT_APP_API_URL=http://localhost:10000/products   # Local JSON Server
REACT_APP_API_URL=https://<your-render-url>.onrender.com/products   # Production API
In your code:

js
Copy
Edit
fetch(`${process.env.REACT_APP_API_URL}`)
  .then(res => res.json())
  .then(data => console.log(data));
🛠 Tech Stack
React (or Next.js if used)

Tailwind CSS / CSS Modules

JavaScript (ES6+)

JSON Server (mock API)

Netlify (frontend hosting)

Render (API hosting)

📌 Notes
Free Render services may “sleep” after inactivity — first request might take a few seconds.

This is a frontend-only cart — no payment gateway integration.

📄 License
MIT License — free to use and modify.

yaml
Copy
Edit

---

Just replace `<your-netlify-url>` and `<your-render-url>` with your actual deployed URLs.  

If you want, I can help you add screenshots or usage instructions next!
