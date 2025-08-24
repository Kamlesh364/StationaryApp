# Ecommerce Wiki Documentation
**Stationery & Sports Store – Technical Documentation**

---

## 📋 Table of Contents
- [Overview](#overview)
- [Page 1: Product Listing App (MVP)](#page-1-product-listing-app-mvp)
  - [Features](#features)
  - [Tech Stack](#tech-stack)
  - [API Endpoints](#api-endpoints)
  - [Future Scope](#future-scope)
- [Page 2: End-Consumer App](#page-2-end-consumer-app)
  - [Features](#features-1)
  - [Workflow](#workflow)
  - [Future Scope](#future-scope-1)
- [Page 3: Admin Dashboard](#page-3-admin-dashboard)
  - [Features](#features-2)
  - [Tech Stack](#tech-stack-1)
  - [Future Scope](#future-scope-2)
- [Additional Resources](#additional-resources)

---

## Overview

This documentation covers the complete ecommerce platform for a Stationery & Sports Store, divided into three main components:

1. **Product Listing App (MVP)** - Initial product browsing functionality
2. **End-Consumer App** - Full ecommerce platform for customers  
3. **Admin Dashboard** - Management interface for shop owners

---

## Page 1: Product Listing App (MVP)

### Overview
The Product Listing App serves as the **first step** toward the full ecommerce platform. It enables users to browse available stationery and sports products online.

### Features
- Display all products in a grid layout
- Search products by name and filter by category
- View product details: description, price, stock availability, and image
- Lightweight and mobile-friendly design

### Tech Stack
- **Frontend**: React + Tailwind CSS
- **Backend**: Node.js (Express)
- **Database**: SQLite/MySQL
- **Hosting**: Vercel/Netlify (Frontend), Render/Heroku (Backend)

### API Endpoints
- `GET /api/products` → Fetch all products
- `GET /api/products/:id` → Fetch single product details
- `POST /api/products` → Add product (Admin only)
- `PUT /api/products/:id` → Update product
- `DELETE /api/products/:id` → Delete product

### Future Scope
- Add cart & checkout flow
- Integrate payment system
- Enable product reviews

---

## Page 2: End-Consumer App

### Overview
The **End-Consumer App** is the ecommerce platform for customers. It provides product discovery, order placement, and delivery/pickup options.

### Features
- **User Authentication** (Register/login with email or phone)
- **Browse & Search** with filters and sorting
- **Cart & Checkout** with delivery eligibility (≥ INR 500)
- **Order Fulfillment**: Home Delivery & Store Pickup
- **Payments**: Razorpay/UPI integration
- **Order Tracking & Notifications**

### Workflow
1. Customer logs in
2. Browses catalog, adds items to cart
3. Chooses delivery or pickup option
4. Completes payment
5. Receives confirmation and status updates

### Future Scope
- Loyalty program and discount coupons
- Personalized recommendations
- Subscription-based stationery supplies

---

## Page 3: Admin Dashboard

### Overview
The **Admin Dashboard** allows shop owners and staff to manage the ecommerce system effectively.

### Features
- **Product Management** (Add/edit/remove products, manage stock levels)
- **Order Management** (view/update orders, assign delivery agents)
- **Customer Management** (view customers, manage returns/refunds)
- **Analytics** (sales reports, popular products, delivery trends)

### Tech Stack
- **Frontend**: React (Admin template)
- **Backend**: Shared with consumer app (Node.js/Django REST API)
- **Database**: Shared product, orders, users schema

### Future Scope
- Advanced reporting with dashboards
- AI-driven demand forecasting
- Multi-store management

---

## Additional Resources

### Project Files
- [Delivery Pickup Flow Diagram](Delivery_Pickup_Flow.png)
- [Project Presentation](Ecommerce_Stationery_Sports_Presentation.pdf)
- [Project Report](Ecommerce_Stationery_Sports_Report.pdf)

### Development Phases
1. **Phase 1**: Product Listing App (MVP) - Basic product browsing
2. **Phase 2**: End-Consumer App - Full ecommerce functionality
3. **Phase 3**: Admin Dashboard - Management interface

### Key Technologies
- **Frontend**: React.js, Tailwind CSS
- **Backend**: Node.js/Express or Django
- **Database**: MySQL/PostgreSQL
- **Payment**: Razorpay integration
- **Hosting**: Vercel, Netlify, Render

---

*Last updated: December 2024*
