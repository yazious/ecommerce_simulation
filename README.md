E-Commerce Simulation Project
Project Description

This is a web-based e-commerce simulation built using Python and Flask. The system allows users to view products, add them to the cart, manage bundles, apply discounts, filter and search products, and manage a wishlist. It demonstrates the use of multiple software design patterns including Factory, Singleton, Decorator, Builder, and Facade.

Features
Core Features

View product catalog

Add products to shopping cart

Checkout with flat or percentage discounts

Bundle products with discount

Inventory management with stock checks

Price drop notifications (simulated)

Optional Features

Product search

Filter products by category

Wishlist to save desired products

Design Patterns Used

Factory Pattern

Problem Solved: Simplifies product creation for different categories.

Implementation: ElectronicsFactory, ClothingFactory, HomeAppliancesFactory create category-specific products.

Singleton Pattern

Problem Solved: Ensures a single shared inventory instance across the application.

Implementation: InventorySingleton

Decorator Pattern

Problem Solved: Adds flexible discount options without modifying the original cart calculation logic.

Implementation: PercentageDiscount and FlatDiscount classes decorate CartTotal

Builder Pattern

Problem Solved: Simplifies the creation of complex cart objects.

Implementation: CartBuilder class

Facade Pattern

Problem Solved: Simplifies the checkout process.

Implementation: CheckoutFacade class

Technology Stack

Backend: Python 3, Flask

Frontend: HTML, CSS, JavaScript

Version Control: Git, GitHub

Design Patterns: Factory, Singleton, Decorator, Builder, Facade

Folder Structure

ecommerce_simulation/
├── app.py
├── models/
│ ├── product.py
│ ├── inventory.py
│ ├── cart.py
│ ├── category.py
│ ├── bundles.py
│ └── discounts.py
├── facade/
│ └── checkout_facade.py
├── utils/
│ └── notifications.py
├── templates/
│ └── index.html
├── static/
│ ├── style.css
│ └── script.js
├── README.md
└── .gitignore

How to Run the System

Clone the repository
git clone https://github.com/yazious/ecommerce_simulation.git

cd ecommerce_simulation

Create a virtual environment (optional but recommended)
python -m venv venv

Windows

venv\Scripts\activate

Mac/Linux

source venv/bin/activate

Install dependencies
pip install Flask

Run the Flask application
python app.py

Open in browser
http://127.0.0.1:5000/


Authors

Muhammad Ayaz

CMS Number: 62795

Section: [Your Section]
