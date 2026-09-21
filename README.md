# Inventory Management System

## Overview

The **Inventory Management System** is a full-stack web application developed to streamline and automate inventory-related operations within an organization. The system enables efficient management of products, categories, suppliers, stock levels, and inventory transactions through a centralized platform.

The primary goal of the system is to improve inventory accuracy, minimize manual effort, reduce stock-related errors, and provide users with real-time visibility into inventory operations.

---

## Key Features

- **User Authentication & Authorization**
  - Secure access to the system using JWT-based authentication.

- **Dashboard**
  - Provides an overview of inventory status, stock levels, and recent activities.

- **Product Management**
  - Create, update, delete, and manage product information.

- **Category Management**
  - Organize products into relevant categories.

- **Inventory Management**
  - Monitor stock quantities and maintain inventory records.

- **Stock In & Stock Out**
  - Track incoming and outgoing inventory transactions.

- **Supplier Management**
  - Maintain supplier information and associated products.

- **Low Stock Monitoring**
  - Identify products that have reached their minimum stock threshold.

- **Search & Filtering**
  - Quickly locate products and records.

- **Transaction History**
  - Maintain records of inventory-related activities.

---

## Objectives

The Inventory Management System is designed to:

1. Automate inventory management processes.
2. Maintain accurate and up-to-date stock information.
3. Reduce errors associated with manual inventory tracking.
4. Improve inventory management efficiency.
5. Provide centralized management of products and suppliers.
6. Enable faster access to inventory information.
7. Monitor stock levels and identify low-stock products.
8. Provide useful inventory information for better decision-making.

---

## System Modules

### 1. Authentication & User Management

The authentication module provides secure access to the application using JWT-based authentication.

### 2. Dashboard

The dashboard provides an overview of the inventory system, including:

- Total products
- Total categories
- Available stock
- Low-stock products
- Recent inventory activities

### 3. Product Management

Users can manage product information, including:

- Product name
- Product code/SKU
- Category
- Quantity
- Price
- Supplier
- Stock threshold
- Product status

### 4. Inventory Management

The inventory module maintains stock information and records stock movements.

### 5. Supplier Management

This module allows users to maintain supplier records and supplier-related information.

### 6. Stock Management

Users can record stock movements and monitor changes in inventory quantities.

### 7. Reports and Inventory Information

The application provides useful inventory summaries and information about stock levels and activities.

---

## System Workflow

```text
                    ┌─────────────────┐
                    │      Login      │
                    └────────┬────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │    Dashboard    │
                    └────────┬────────┘
                             │
             ┌───────────────┼───────────────┐
             │               │               │
             ▼               ▼               ▼
       ┌───────────┐   ┌───────────┐   ┌───────────┐
       │ Products  │   │ Suppliers │   │ Categories│
       └─────┬─────┘   └─────┬─────┘   └─────┬─────┘
             │               │               │
             └───────────────┼───────────────┘
                             ▼
                    ┌─────────────────┐
                    │    Inventory    │
                    │     Updates     │
                    └────────┬────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │ Stock & Activity│
                    │     Reports     │
                    └─────────────────┘