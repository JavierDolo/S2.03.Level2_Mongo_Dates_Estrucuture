# 🍕 MongoDB Food Ordering System – Level 2

## 📄 Description – Exercise Statement

This project involves designing and implementing a **NoSQL database** using **MongoDB** for an online food ordering system. The main goal is to model customers, orders, products (pizzas, burgers, drinks), stores, and employees with appropriate relationships, following the exercise's detailed requirements.

The system supports multiple products per order, stores managing orders, employees with specific roles, and delivery tracking for home orders.


## 💻 Technologies Used

- **MongoDB** (Document Database)
- **MongoDB Compass** (GUI for managing and visualizing the database)
- **JSON** for structured data insertion
- **JavaScript** (basic Mongo Shell syntax)
- **Markdown** for documentation

## 📋 Requirements

Before running the project, ensure the following tools are installed:

- MongoDB Community Server (v6.x or later recommended)
- MongoDB Compass (optional but useful)
- Node.js (only if you plan to use scripts via shell – optional)

## 🛠️ Installation

To set up the database locally:

1. Clone the repository:

   git clone https://github.com/JavierDolo/S2.03.Level2_Mongo_Dates_Estrucuture.git

2. Open MongoDB Compass or connect to your local MongoDB server.

3. Create a new database, for example: `food_ordering_db`.

4. Create the following collections manually:
   - `customers`
   - `pizza_categories`
   - `products`
   - `stores`
   - `employees`
   - `orders`

5. Use the **Insert Many** option to load the JSON data provided in the project folder into each collection.

## ▶️ Execution

Once the database is populated:

- You can perform queries in MongoDB Compass or Mongo Shell.
- Example: list all delivery orders with assigned employees:

   db.orders.find({ deliveryType: "home" }).pretty();

- Example: list all employees working in a specific store:

   db.employees.find({ storeId: ObjectId("your_store_id_here") });

## 🌐 Deployment

If you wish to deploy this project:

- Use MongoDB Atlas for cloud-hosted database.
- Import your data using mongoimport or through Atlas' import tools.
- Adjust connection strings in your frontend/backend (if built).

## 🤝 Contributions

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to your branch (`git push origin feature/your-feature`).
5. Open a Pull Request.

Please follow consistent formatting and include useful commit messages.
