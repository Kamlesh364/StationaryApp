# Ecommerce Wiki Documentation
**Stationery & Sports Store – Technical Documentation**

---

## Navigation
<select id="pageSelector" onchange="showPage()">
  <option value="page1">Page 1: Product Listing App (MVP)</option>
  <option value="page2">Page 2: End-Consumer App</option>
  <option value="page3">Page 3: Admin Dashboard</option>
</select>

---

<div id="page1" class="page-content">
# Page 1: Product Listing App (MVP)

## Overview
The Product Listing App serves as the **first step** toward the full ecommerce platform. It enables users to browse available stationery and sports products online.

## Features
- Display all products in a grid layout
- Search products by name and filter by category
- View product details: description, price, stock availability, and image
- Lightweight and mobile-friendly design

## Tech Stack
- **Frontend**: React + Tailwind CSS
- **Backend**: Node.js (Express)
- **Database**: SQLite/MySQL
- **Hosting**: Vercel/Netlify (Frontend), Render/Heroku (Backend)

## API Endpoints
- `GET /api/products` → Fetch all products
- `GET /api/products/:id` → Fetch single product details
- `POST /api/products` → Add product (Admin only)
- `PUT /api/products/:id` → Update product
- `DELETE /api/products/:id` → Delete product

## Future Scope
- Add cart & checkout flow
- Integrate payment system
- Enable product reviews
</div>

<div id="page2" class="page-content" style="display: none;">
# Page 2: End-Consumer App

## Overview
The **End-Consumer App** is the ecommerce platform for customers. It provides product discovery, order placement, and delivery/pickup options.

## Features
- **User Authentication** (Register/login with email or phone)
- **Browse & Search** with filters and sorting
- **Cart & Checkout** with delivery eligibility (≥ INR 500)
- **Order Fulfillment**: Home Delivery & Store Pickup
- **Payments**: Razorpay/UPI integration
- **Order Tracking & Notifications**

## Workflow
1. Customer logs in
2. Browses catalog, adds items to cart
3. Chooses delivery or pickup option
4. Completes payment
5. Receives confirmation and status updates

## Future Scope
- Loyalty program and discount coupons
- Personalized recommendations
- Subscription-based stationery supplies
</div>

<div id="page3" class="page-content" style="display: none;">
# Page 3: Admin Dashboard

## Overview
The **Admin Dashboard** allows shop owners and staff to manage the ecommerce system effectively.

## Features
- **Product Management** (Add/edit/remove products, manage stock levels)
- **Order Management** (view/update orders, assign delivery agents)
- **Customer Management** (view customers, manage returns/refunds)
- **Analytics** (sales reports, popular products, delivery trends)

## Tech Stack
- **Frontend**: React (Admin template)
- **Backend**: Shared with consumer app (Node.js/Django REST API)
- **Database**: Shared product, orders, users schema

## Future Scope
- Advanced reporting with dashboards
- AI-driven demand forecasting
- Multi-store management
</div>

---

<script>
function showPage() {
    const selector = document.getElementById('pageSelector');
    const selectedPage = selector.value;
    
    // Hide all pages
    const pages = document.querySelectorAll('.page-content');
    pages.forEach(page => {
        page.style.display = 'none';
    });
    
    // Show selected page
    const selectedPageElement = document.getElementById(selectedPage);
    if (selectedPageElement) {
        selectedPageElement.style.display = 'block';
    }
}

// Initialize with first page
document.addEventListener('DOMContentLoaded', function() {
    showPage();
});
</script>

<style>
select {
    padding: 8px 12px;
    border: 1px solid #ddd;
    border-radius: 4px;
    background-color: white;
    font-size: 14px;
    margin-bottom: 20px;
}

.page-content {
    border-top: 1px solid #eee;
    padding-top: 20px;
}

.page-content h1 {
    color: #2c3e50;
    border-bottom: 2px solid #eee;
    padding-bottom: 10px;
    margin-bottom: 20px;
}

.page-content h2 {
    color: #2c3e50;
    margin-top: 25px;
    margin-bottom: 15px;
}

.page-content ul {
    margin-bottom: 15px;
}

.page-content li {
    margin-bottom: 5px;
}
</style>
