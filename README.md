# 🍽️ Food Waste Reduction Platform (FWRP)

The Food Waste Reduction Platform (FWRP) addresses the global issue of food waste by providing a solution that connects **food retailers**, **consumers**, and **charitable organizations**. It promotes sustainability, reduces hunger, and enhances food redistribution by facilitating surplus food sharing.

This project is developed as part of the **CST – 8288 Final Project**.

---

## 🔑 Features

### FR – 01: User Registration and Authentication
- Users can register with name, email, password, and user type (Retailer, Consumer, Charitable Organization)
- Login and logout functionality for all users

### FR – 02: Retailers
- **Inventory Management**: Add/update food items with expiration dates
- **Surplus Flagging**: Identify items expiring soon or overstocked
- **Listing**: Share flagged items for donation or discounted sale

### FR – 03: Charitable Organizations
- **Claim Items**: View and claim surplus food
- **Auto Update**: Inventory adjusts after claiming

### FR – 04: Consumers
- **Purchase Surplus**: Buy discounted surplus food
- **Inventory Update**: Auto update on successful purchase

### FR – 05: Surplus Food Alerts
- **Subscription**: Users can subscribe for location-based surplus alerts
- **Notifications**: Auto alerts via email/phone based on preferences

### FR – 06: Bonus Functionality
- An additional unique feature described in the High-Level Design (HLD) document

---

## 🏗️ Architecture

FWRP follows a **3-Tier Architecture**:

1. **Presentation Layer (MVC/UI)** – User-facing interface
2. **Business Layer** – Handles logic and user actions
3. **Database Layer (DAO/JDAL)** – Manages data persistence

---

## 🗃️ Database

A relational database schema (`FWRP`) includes:

- User management
- Inventory & surplus food tracking
- Purchase and claiming functionality
- Alerts and notifications

Database includes sample datasets for testing.

---

## 📂 Project Setup

### Prerequisites
- Java JDK (installed)
- MySQL/PostgreSQL (with `FWRP` schema created)
- Maven (installed)

---

## 🚀 Installation Steps

1. Clone the Repository:
   ```bash
   git clone https://github.com/yourusername/fwrp-project.git
   cd fwrp-project
Configure the Database:

Create a schema named FWRP in MySQL or PostgreSQL

Import the schema and sample data

### Set up Environment (if applicable)

Create a `.env` file in the server directory and add the following:

```env
DB_URL=jdbc:mysql://localhost:3306/FWRP
DB_USER=your_username
DB_PASSWORD=your_password


🛠️ Build the Project
Use Maven to build the entire project:

bash
Copy
Edit
mvn clean install
