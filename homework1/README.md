# 📘 Homework 4 — AI-Powered Managerial Chatbot

This homework focuses on building an AI-powered managerial assistant that can understand natural-language questions and automatically translate them into SQL queries. The system uses Google Gemini to interpret queries, generate structured JSON, and retrieve answers from a fully populated Northwind database.

## 🚀 What I Implemented

### ✔ 1. Gemini API Integration
- Loaded the Gemini API key securely using `.env`
- Initialized the Gemini client
- Created a chat session using `gemini-2.5-flash`
- Ensured model outputs are returned as structured JSON, not plain text

### ✔ 2. SQLite Database Creation
- Created an SQLite database (`myDatabase.db`)
- Implemented the full Northwind schema, including tables for:
  - Customers
  - Orders
  - Employees
  - Products
  - Shippers
  - Categories
  - Suppliers
  - Order Details
- Ensured all tables are recreated cleanly before usage

### ✔ 3. Data Population
- Inserted realistic sample data from the Northwind dataset
- Ensured the chatbot has real business information to query

### ✔ 4. Natural-Language → SQL Chatbot
- Built a chatbot interface where users can ask questions in English or Turkish
- Used Gemini to translate the question into SQL
- Executed the SQL query on the local database
- Returned results in a friendly, conversational style

### ✔ 5. User Interface (Gradio)
- Developed a simple and interactive web UI
- Displays the conversation between the user and the AI
- Sends natural-language queries and displays structured responses

