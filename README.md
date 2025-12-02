# E-Commerce Simulation Project

## Project Description
This project is a **web-based e-commerce simulation** built using **Python** and **Flask**. It allows users to:

- Browse a product catalog with multiple categories
- Add products to a shopping cart
- Apply bundles and discounts during checkout
- Manage inventory and track stock
- Receive notifications for price drops (simulated)
- Search and filter products
- Save desired products in a wishlist

The project demonstrates the use of **multiple software design patterns** including **Factory, Singleton, Decorator, Builder, and Facade**. It is designed as a learning simulation rather than a production-level system.

---

## Features

### Core Features
- View product catalog
- Add products to cart
- Checkout with flat or percentage discounts
- Bundle products with discount
- Inventory management with stock checks
- Price drop notifications (simulated)

### Optional Features
- Product search
- Filter products by category
- Wishlist to save desired products

---

## Technology Stack
- **Backend:** Python 3, Flask
- **Frontend:** HTML, CSS, JavaScript
- **Version Control:** Git, GitHub
- **Design Patterns:** Factory, Singleton, Decorator, Builder, Facade

---

## Folder Structure

ecommerce_simulation/
    app.py                 # Main Flask application
    models/                # Product, Cart, Inventory, Bundles, Discounts, Category
        product.py
        inventory.py
        cart.py
        category.py
        bundles.py
        discounts.py
    facade/                # Checkout Facade implementation
        checkout_facade.py
    utils/                 # Utility classes like notifications
        notifications.py
    templates/             # HTML templates
        index.html
    static/                # CSS and JavaScript
        style.css
        script.js
    report/                
    README.md              # This file
    .

    
---

Design Patterns Used
---
Factory Pattern
--
Problem Solved: Simplifies product creation for different categories.

Implementation: ElectronicsFactory, ClothingFactory, HomeAppliancesFactory create category-specific products.

Singleton Pattern
-
Problem Solved: Ensures a single shared inventory instance across the application.

Implementation: InventorySingleton

Decorator Pattern
-
Problem Solved: Adds flexible discount options without modifying the original cart calculation logic.

Implementation: PercentageDiscount and FlatDiscount decorate CartTotal.

Builder Pattern
-
Problem Solved: Simplifies creation of complex cart objects.

Implementation: CartBuilder class.

Facade Pattern
-
Problem Solved: Simplifies the checkout process for users.

Implementation: CheckoutFacade class.

Technology Stack
-
Backend: Python 3, Flask

Frontend: HTML, CSS, JavaScript

Version Control: Git, GitHub

Design Patterns: Factory, Singleton, Decorator, Builder, Facade



## How to Run the System

Follow these steps to run the e-commerce simulation locally:

### 1. Clone the repository
```bash
git clone https://github.com/yazious/ecommerce_simulation.git
cd ecommerce_simulation

2. Create a virtual environment (optional but recommended)
python -m venv venv

Activate the environment

Windows:

venv\Scripts\activate


Mac/Linux:

source venv/bin/activate

3. Install dependencies
pip install Flask

4. Run the Flask application
python app.py

5. Open in browser

Visit: http://127.0.0.1:5000/

---

