# 🍽️ Restaurant Management System

A Python CLI application demonstrating object-oriented programming (OOP) principles, structured class hierarchies, and clean domain modeling for restaurant operations.

[![Python: 3.x](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## Overview

The **Restaurant Management System** models real-world food service operations through an interactive terminal interface. It demonstrates core OOP patterns—including abstract base classes, inheritance, composition, and property decorators—by separating administrative management workflows from customer ordering and billing pipelines.

---

## Features

### 👤 Customer Workflow
- **Interactive Menu Browsing**: View available food items with real-time pricing and stock quantity.
- **Cart Management**: Add items with inventory validation and quantity checks.
- **Order Review**: View items in cart with aggregated subtotal and dynamic total calculations.
- **Billing**: Execute payment settlements and automatic cart clearing.

### 🛠️ Administrative & Staff Management
- **Menu Engineering**: Add new food items with designated price and stock thresholds; delete discontinued items.
- **Staff Administration**: Register employees with detailed profiles (designation, age, contact, salary) and inspect staff records.
- **Inventory Oversight**: Inspect restaurant-wide menu catalogs and availability.

---

## Technical Highlights & OOP Architecture

- **Abstract Base Classes (`ABC`)**: Implements `User(ABC)` to enforce standardized interface contracts for `Customer`, `Employee`, and `Admin`.
- **Inheritance & Polymorphism**: Reuses shared identity and contact properties while providing role-specific behavior.
- **Composition**: The `Restaurent` class composes `Menu` and `Employee` collections, while `Customer` composes an `Order` cart containing `FoodItem` objects.
- **Encapsulation & Properties**: Uses Python's `@property` decorator for dynamic order sum calculations (`Order.total_price`).

```text
┌───────────────────────────────────────────────┐
│                   User (ABC)                  │
└───────┬───────────────┬───────────────┬───────┘
        │               │               │
        ▼               ▼               ▼
   Customer          Employee         Admin
 (owns Cart/Order)  (Staff Data)    (Menu & Staff)
        │
        ▼
   FoodItem ◄─────── Menu ◄─────── Restaurent
```

---

## Tech Stack

- **Language**: Python 3.x
- **Standard Library**: `abc` (Abstract Base Classes)

---

## Project Structure

```text
Resturen_Project_python_oop_practice/
├── main.py        # Complete OOP implementation and CLI menu loops
├── LICENSE        # MIT License
└── README.md      # Technical documentation
```

---

## Installation & Execution

### Prerequisites
- Python 3.8 or higher

### 1. Clone the Repository
```bash
git clone https://github.com/sazzadhossainsakib13/Resturen_Project_python_oop_practice.git
cd Resturen_Project_python_oop_practice
```

### 2. Run the Application
```bash
python main.py
```

---

## Terminal Screenshots

<div align="center">

| Customer Interface & Cart | Admin Menu & Staff Management |
| :---: | :---: |
| <img width="432" alt="Customer Menu Terminal" src="https://github.com/user-attachments/assets/5ac6199b-fe0e-4610-8a6b-c509c4a00a74" /> | <img width="461" alt="Admin Control Terminal" src="https://github.com/user-attachments/assets/0341d6ac-d5bb-4e08-b636-f2fabc9e5a40" /> |

| Order Checkout & Billing | Menu Modification |
| :---: | :---: |
| <img width="387" alt="Checkout Terminal" src="https://github.com/user-attachments/assets/f658d7e6-10b9-460d-b0bf-928999f3838c" /> | <img width="326" alt="Menu Terminal" src="https://github.com/user-attachments/assets/3322a7b6-b4a8-41f6-8ea7-8443cac4f694" /> |

</div>

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Author

**Sazzad Hossain Sakib**  
- GitHub: [@sazzadhossainsakib13](https://github.com/sazzadhossainsakib13)




