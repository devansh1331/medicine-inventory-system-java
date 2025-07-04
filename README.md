# 💊 Medicine Inventory Management System (Java + MySQL)
A basic **Java OOP project** for managing medicine stock, built with **Java**, **Swing**, and **MySQL**. Designed for academic learning and small-scale use
---

## 🧠 Features

- 👥 **Role-based login**: Buyers and Sellers
- 📦 **Stock management**: Add, view, and update medicines
- 🛒 **Purchase system**: Buy medicines with quantity checks
- 💽 **Transaction records**: Logged for every sale or addition
- 🖥️ **GUI Interface**: Built with Java Swing
- 🛢️ **Database Integration**: MySQL + JDBC

---

## 🔐 User Roles

### 🏭 Seller
- Adds medicines (min 10,000 and max 20,000 units)
- Input includes name, quantity, manufacture and expiry dates
- Adds records to both stock and transaction logs

### 🛒 Buyer
- Can view available stock
- Can purchase up to 10 units of a medicine
- Purchase gets recorded in the transaction table
- Stock is updated in real-time

---

## 🗃️ Database Tables

1. `accounts` — stores user login credentials  
   **Fields**: `username`, `password`, `role`

2. `stock` — stores medicine details  
   **Fields**: `username`, `med_name`, `quantity`, `DOM`, `DOE`

3. `transaction` — stores all purchase/sell history  
   **Fields**: `user_id`, `med_name`, `quantity`

---

## ⚙️ Tech Stack

- **Java** (OOP)
- **Java Swing** (GUI)
- **MySQL** (DBMS)
- **JDBC** (Database connectivity)

---

## 🖥️ How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/devansh1331/medicine-inventory-java.git
   cd medicine-inventory-java
   
2. **Set up MySQL**

Create a database named medicine_inventory

Create tables: accounts, stock, transaction.

3. **Configure your DB credentials in Java files:**
   ```java
   DriverManager.getConnection("jdbc:mysql://localhost:3306/medicine_inventory", "root", "yourpassword");

4. **Run the project**

Open in any IDE (IntelliJ / Eclipse)

Compile and run User_class.java



