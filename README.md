Food Waste Reduction Platform
Overview
The Food Waste Reduction Platform (FWRP) aims to address the global issue of food waste by providing a comprehensive solution that connects food retailers, consumers, and charitable organizations. The platform promotes sustainability, reduces hunger, and builds more resilient food ecosystems by facilitating the efficient redistribution of surplus food. It encourages collaboration among stakeholders in the food supply chain to address one of the most pressing challenges of our time.

This project is developed as part of the CST – 8288 Final Project.

Features
FR – 01: User Registration and Authentication
Registration: Users can create accounts by providing their name, email, password, and user type (Retailers, Consumers, or Charitable Organizations).
Authentication: Login/logout functionality is available for all users.
FR – 02: Retailers
Inventory Management: Retailers can manage their inventory of food items by adding new items, updating quantities, and setting expiration dates.
Surplus Food Identification: Retailers can identify and flag surplus food items nearing expiration (within the next week) or in excess of demand.
Listing Surplus Food Items: Retailers can list surplus food items for donation or sale at a discounted price.
FR – 03: Charitable Organizations
Claim Food: Charitable organizations, such as food banks, can claim surplus food items listed by retailers for donation.
Update Inventory: The retailer’s inventory is automatically updated when a charitable organization claims a food item.
FR – 04: Consumers
Purchase: Consumers can purchase surplus food items listed by retailers at a discounted price.
Update Inventory: Retailer inventory is updated when a consumer purchases an item.
FR – 05: Surplus Food Alerts
User Subscription: Users can subscribe to receive alerts about surplus food based on their location, communication method (email/phone), and food preferences.
Automatic Notifications: Subscribed users receive automatic notifications whenever retailers list surplus food items.
FR – 06: Bonus Functionality
A unique additional feature to enhance the platform. Details will be provided in the High-Level Design (HLD) document.
Architecture
1. Presentation Layer (User Interface / MVC)
This layer is responsible for interacting with users and providing the user interface.
2. Business Layer (Business Logic / Functionalities)
Contains the business logic and handles the processing of user requests.
3. Database Layer (Persistence / DAO / JDAL / Database)
Manages and stores the persistent data used by the application.
The platform follows a 3-Tier Architecture to ensure separation of concerns.

Database
The system is supported by a relational database management system (RDBMS) named FWRP. The schema is designed to handle all the functional requirements of the platform, including:

User management
Inventory management
Surplus food management
Claiming and purchasing of surplus food
Notifications and alerts for users
The database design includes tables and relationships as per the functional requirements, along with sample datasets for testing.

Version Control
GitHub Usage
GitHub Repository: The project uses GitHub for version control and collaboration.
The Team Lead is responsible for creating the repository and managing branches and pull requests.
Each team member works on their own branch, creating pull requests for their contributions.
All code must be merged into the main repository using pull requests.
GitHub Workflow
The Team Lead creates the GitHub repository.
Other team members clone the repository and work on their branches.
Code is submitted to the main repository via pull requests, which the Team Lead approves.
Regular code merging is encouraged; last-minute merges are discouraged.
Testing
JUnit
JUnit Tests are required for all major functionalities of the platform.
JUnit tests must reside in a separate test package, apart from the main codebase.
The test cases will cover essential features such as user registration, inventory management, surplus food listing, claiming, purchasing, and notification alerts.
Technologies and Tools
Java / J2EE: The core programming language for the project.
Servlets & JSP: For handling requests and responses in the web application.
MySQL/PostgreSQL: For relational database management.
JUnit: For writing and executing unit tests.
Maven: For project management and dependency management.
GitHub: For version control.
Design Patterns: The solution will incorporate various design patterns such as Singleton, DAO, and MVC.
Project Setup
Prerequisites
Java JDK: Make sure Java JDK is installed.
MySQL or PostgreSQL: Setup a relational database and create the FWRP schema.
Maven: Ensure Maven is installed for managing dependencies.
