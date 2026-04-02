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

- 
---

## ✅ Validation Rules
- Quantity must be greater than zero  
- Prevent order when stock is 0  

---

## ⚙️ Automation (Flows)
### When Order is Created
- Assign nearest dealer  
- Send confirmation email  
- Create processing task  

### When Order is Confirmed
- Reduce stock automatically  

### When Stock is Low
- Send alert notification  

---

## 💻 Apex Implementation

### Trigger Logic
- Validate stock availability  
- Auto-update order status  

### Apex Class
- Dealer assignment  
- Inventory updates  
- Notifications  

---

## 🔐 Security
- Roles: Admin, Sales User, Dealer Manager  
- Field-level security for pricing  
- Sharing rules for dealer-specific access  

---

## 👥 User Management
- Create users  
- Assign roles & profiles  

---

## 📈 Reports & Dashboards

### Reports
- Orders by Status  
- Vehicle Stock Levels  
- Pending Orders  
- Low Stock Vehicles  

### Dashboard
- Total Orders  
- Confirmed Orders  
- Pending Orders  
- Stock Alerts  

---

## 🔄 Use Case Flow

Customer places order  
→ Order created in Salesforce  
→ Dealer assigned automatically  
→ Stock checked  
→ If available → Confirmed  
→ If not → Pending  
→ Inventory updated  
→ Notification sent  
→ Customer tracks order  
→ Dashboard updated  

---

## 🔗 Deliverables
- Data Model Diagram  
- Object & Field List  
- Flow Automation  
- Apex Code + Test Class  
- Security Setup  
- Reports & Dashboard  
- Demo Link  
- GitHub Repository  

---

## 👨‍💻 Author
Naveen Kumar .S
MAHESHWARAN J
DHANUSH P
PRAVEENA S
