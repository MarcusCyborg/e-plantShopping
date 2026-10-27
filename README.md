# Paradise Nursery Shopping Application

**Paradise Nursery** is an e-commerce web application for an online plant shop where houseplant enthusiasts can explore, browse, and purchase indoor plants. Our motto is **"Where Green Meets Serenity"**.

---

## Project Overview

The **Paradise Nursery Shopping Application** was built using **React** and **Redux Toolkit**. It provides an interactive shopping cart experience designed to make purchasing plants intuitive and seamless.

Key features include:
- A landing page with background imagery, brand mission details, and a quick **Get Started** button.
- An **About Us** section describing the company's background and commitment to quality greenery.
- A categorized **Product Listing Page** with 5 categories (Air Purifying, Aromatic Fragrant, Insect Repellent, Medicinal, Low Maintenance) displaying 6 unique houseplants in each category (30 unique plants total).
- Real-time cart state management using **Redux Toolkit** (`addItem`, `removeItem`, `updateQuantity`).
- Dynamic cart counter badge displayed on the navigation bar across both the catalog and cart views.
- A **Shopping Cart Page** with item quantity adjustment (+/-), item removal, per-item cost subtotal, and total cart amount calculation.
- **Continue Shopping** and **Checkout** ("Coming Soon") actions.

---

## Features & Implementation Details

### 1. Landing Page (`App.jsx`, `App.css`, `AboutUs.jsx`)
- Fullscreen greenhouse background image with smooth overlay.
- Heading banner: **Welcome To Paradise Nursery** with tagline **Where Green Meets Serenity**.
- **Get Started** button to smoothly slide into the plant catalog.
- Company details presented through the `AboutUs` component.

### 2. Redux State Management (`CartSlice.jsx`, `store.js`)
- `addItem`: Adds selected plant to cart or increments quantity if already added.
- `removeItem`: Removes a specific plant from the cart by identifier.
- `updateQuantity`: Updates plant quantity dynamically when incremented or decremented.

### 3. Product Listing Page (`ProductList.jsx`, `ProductList.css`)
- Over 30 unique houseplants categorized into 5 distinct categories (minimum requirement is 3 categories with 6 plants each).
- Each product card contains a thumbnail image, plant name, description, and price.
- **Add to Cart** button adds product to the Redux cart, switches to disabled "Added to Cart" state, and dynamically increments the cart count badge in the navbar.
- Navigation bar includes branding link to Home, link to Plants, and Cart icon with badge counter.

### 4. Shopping Cart Page (`CartItem.jsx`, `CartItem.css`)
- Displays real-time **Total Cart Amount**.
- Displays each plant with image, name, unit price, quantity controls (`+` and `-`), item total cost, and a **Delete** button.
- **Continue Shopping** button allows users to navigate back to the product listing.
- **Checkout** button displays a friendly "Coming Soon" notification.

---

## Project Structure

```text
paradise-nursery-shopping/
├── index.html
├── package.json
├── vite.config.js
├── README.md
├── public/
│   └── vite.svg
└── src/
    ├── main.jsx
    ├── App.jsx
    ├── App.css
    ├── AboutUs.jsx
    ├── AboutUs.css
    ├── ProductList.jsx
    ├── ProductList.css
    ├── CartItem.jsx
    ├── CartItem.css
    ├── CartSlice.jsx
    ├── store.js
    └── index.css
```

---

## Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) (v16 or higher)
- [npm](https://www.npmjs.com/)

### Installation & Local Development

1. Clone the repository:
   ```bash
   git clone https://github.com/MarcusCyborg/e-plantShopping.git
   cd e-plantShopping
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the Vite development server:
   ```bash
   npm run dev
   ```

4. Open your browser and navigate to `http://localhost:5173`.

### Production Build
To create an optimized production build:
```bash
npm run build
```

---

## Technologies Used
- **React 18**
- **Redux Toolkit & React-Redux**
- **Vite**
- **HTML5 & CSS3 (Flexbox, Responsive Design)**
