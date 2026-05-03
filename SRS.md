# Smart Pharmacy Management System with POS, E-commerce & Inventory Control

## 1. Introduction

### 1.1 Purpose
The purpose of this document is to define the requirements of a Smart Pharmacy Management System.
The system is designed to:
- Manage online medicine sales (E-commerce)
- Support in-store and hospital billing (POS system)
- Maintain real-time inventory synchronization

This SRS serves as a reference for developers, instructors, and stakeholders.

### 1.2 Scope
The system provides a complete pharmacy solution, including:
- Customer-facing website for online orders
- Admin dashboard for inventory and system control
- POS system for physical sales (shop/hospital)

**Key Highlight:**
A centralized stock system shared across online store, hospital, and POS.

### 1.3 Definitions
| Term | Description |
|---|---|
| POS | Point of Sale system for billing |
| Inventory | Available stock of medicines |
| Admin | Authorized system manager |
| Pharmacist | User handling POS and medicine sales |
| Customer | End user purchasing medicines |

## 2. Overall Description

### 2.1 Product Perspective
This is a web-based responsive system accessible on:
- Mobile devices
- Tablets
- Desktop systems

It integrates:
- E-commerce
- POS billing
- Inventory system

### 2.2 User Classes and Characteristics
1. **Customer**
   - Basic user
   - Can browse and order medicines

2. **Admin**
   - Full system control
   - Manages stock, medicines, and reports

3. **Pharmacist (POS User)**
   - Handles billing
   - Generates receipts
   - Works in hospital/shop environment

### 2.3 Operating Environment
- Web browsers (Chrome, Edge, etc.)
- Internet connection
- Backend server (Node/PHP + Database)

### 2.4 System Constraints
- Requires stable internet connection
- Payment gateway integration needed
- Must follow medical data handling standards

## 3. System Features

### 3.1 Medicine Management
- Add new medicines
- Update medicine details
- Delete medicines
- Categorize medicines

**Extra Feature:**
- Store expiry date and batch number

### 3.2 Inventory Management (Core Feature)
- Track real-time stock
- Auto-update stock after:
  - Online purchase
  - POS sale
  - Hospital usage

**Visibility Rule:**
- Admin: Exact stock quantity
- Customer: Only “In Stock / Out of Stock”

### 3.3 Unified Stock System (Unique Feature)
A single inventory system shared across:
- Website orders
- Physical pharmacy sales
- Hospital medicine usage

Benefits:
- Prevents stock mismatch
- Ensures accuracy

### 3.4 Low Stock & Smart Alerts
- Alert when stock is low
- Dashboard notifications
- Future enhancement:
  - Predict stock shortage using sales data

### 3.5 E-commerce Module
- Search medicines
- Add to cart
- Checkout system

**Payment Options:**
- Cash on Delivery
- Online payment (optional)

### 3.6 POS Billing System
- Select medicines
- Enter quantity
- Generate bill

**Receipt Includes:**
- Medicine name
- Quantity
- Price
- Date & Time
- Pharmacist name

### 3.7 Order Management
- Store all orders
- View order history
- Track sales

### 3.8 Authentication System
- Secure login for admin
- Role-based access

### 3.9 Prescription Handling (Advanced Feature)
- Upload prescription
- Restrict certain medicines
- Admin approval system

## 4. Functional Requirements

### 4.1 Customer Requirements
- The system shall allow customers to browse medicines
- The system shall allow customers to place orders
- The system shall not display exact stock quantity
- The system shall show stock status (available/unavailable)

### 4.2 Admin Requirements
- The system shall allow admin to add/update/delete medicines
- The system shall display exact stock levels
- The system shall generate alerts for low stock
- The system shall manage orders and users

### 4.3 Pharmacist (POS) Requirements
- The system shall allow medicine selection for billing
- The system shall generate receipts
- The system shall update stock automatically
- The system shall record date and time of purchase

### 4.4 Inventory Requirements
- The system shall maintain a centralized inventory
- The system shall update stock in real-time
- The system shall prevent negative stock

## 5. Non-Functional Requirements

### 5.1 Performance
- Fast system response
- Handle multiple users simultaneously

### 5.2 Security
- Secure authentication system
- Data protection mechanisms
- Role-based access control

### 5.3 Usability
- Simple and user-friendly UI
- Easy navigation
- Mobile responsive design

### 5.4 Reliability
- Accurate stock updates
- No data loss
- System availability

### 5.5 Scalability
- Can handle increasing number of users
- Can support multiple pharmacy branches (future)

## 6. Use Case Summary
| Actor | Actions |
|---|---|
| Customer | Browse, Order |
| Admin | Manage medicines, view stock |
| Pharmacist | Generate bill, sell medicines |

## 7. Future Enhancements
- AI-based medicine recommendations
- Sales prediction system
- Expiry alerts automation
- Mobile application (Android/iOS)
- Multi-branch pharmacy support

## 8. Conclusion
The Smart Pharmacy Management System provides a complete and integrated solution for pharmacy operations.

Unlike traditional systems, it combines:
- E-commerce
- POS billing
- Real-time inventory

This ensures:
- Accuracy
- Efficiency
- Better decision-making
