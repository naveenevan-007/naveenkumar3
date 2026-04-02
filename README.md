# 🚗 WhatsNext Vision Motors  
### Salesforce-Based Automotive Order Management System

## 📌 Project Overview
WhatsNext Vision Motors is a Salesforce-driven Order Management System (OMS) designed to:

- Automate vehicle order processing
- Track vehicle inventory in real-time
- Improve customer experience
- Assign nearest dealers automatically
- Ensure data security
- Provide reports & dashboards

---

## 🎯 Objectives
- Efficient order management
- Real-time stock tracking
- Automated workflows
- Secure data handling
- Business insights via dashboards

---

## 🧱 Data Model

### Core Objects
- Customer (Account / Contact)
- Vehicle
- Order
- Order Line Item
- Inventory
- Dealer

### Relationships
- One Customer → Many Orders  
- One Order → Many Order Line Items  
- One Vehicle → Many Inventory Records  
- One Dealer → Many Orders  

---

## 📊 Fields

### Order Object
- Order ID  
- Order Status (New, Pending, Confirmed, Delivered)  
- Order Date  
- Total Amount (Formula)

### Order Line Item
- Vehicle  
- Quantity  
- Price  

### Inventory
- Stock Available  
- Reorder Level  
- Last Updated  

---

## 🧮 Formula Fields
- **Total Amount** = Quantity × Price  
- **Stock Status** =  
