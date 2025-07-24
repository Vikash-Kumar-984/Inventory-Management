# FactoryFlow - Manufacturing Inventory Management System

## Website Deployment on Google Firebase: https://inventory-58bee.web.app/

## 1. Project Description

FactoryFlow is a comprehensive, real-time web application designed for small to medium-sized manufacturing businesses. It provides a centralized dashboard to manage the entire production lifecycle, from tracking raw materials and defining product recipes to logging sales and managing manufacturing orders.

This tool is built to replace complex spreadsheets and provide a clear, live overview of your business operations, helping you make informed decisions about stock levels, purchasing, and production priorities.

---

## 2. Core Features

* **📊 Interactive Dashboard:** A high-level overview of key business metrics, including total revenue, open sales orders, and low-stock alerts for both products and materials.
* **📦 Raw Materials Management:** Keep a detailed record of all your raw materials, including stock levels, suppliers, cost per unit, and reorder points.
* **🛍️ Products Master:** A master list of all finished goods you produce. Each product has a unique SKU, selling price, and a **Bill of Materials (BOM)** that defines its "recipe."
* **🛒 Sales Order Tracking:** Log sales from various online platforms (like Flipkart, Myntra, etc.). The system automatically deducts stock from finished goods inventory.
* **🏭 Manufacturing Management:** Create manufacturing orders to produce new batches of your products. The system automatically checks for sufficient raw materials based on the product's BOM and deducts them from inventory when production begins. When production is complete, the finished goods stock is automatically updated.
* **倉庫 (Warehouse) Live Inventory View:** A real-time snapshot of all your stock levels, highlighting items that are running low and need attention.

---

## 3. Technology Stack

This application was built using a modern, efficient, and scalable technology stack.

* **Frontend Framework:**
    * **[React](https://reactjs.org/):** A powerful JavaScript library for building user interfaces.
    * **[Vite](https://vitejs.dev/):** A next-generation frontend build tool that provides an extremely fast development experience.

* **Backend & Database:**
    * **[Google Firebase](https://firebase.google.com/):** A comprehensive platform for building web and mobile applications.
        * **Firestore:** A flexible, scalable NoSQL cloud database for storing all application data in real-time.
        * **Firebase Authentication:** Used for securing the application and managing user data.

* **Styling:**
    * **[Tailwind CSS](https://tailwindcss.com/):** A utility-first CSS framework for rapidly building modern, custom designs.

* **Icons:**
    * **[Lucide React](https://lucide.dev/):** A beautiful and consistent open-source icon library.

---

## 4. Local Setup and Installation

To run this project on your local computer, follow these steps:

#### **Prerequisites:**

* **Node.js (LTS version):** Download from [nodejs.org](https://nodejs.org/).
* A **Firebase Project:** Create a free project at the [Firebase Console](https://console.firebase.google.com/).

#### **Installation:**

1. **Clone the repository (or copy the files) into a new folder.**

2. **Navigate into the project directory:**
   ```bash
   cd factoryflow-inventory-app
   ```

3. **Install all required packages:**
   ```bash
   npm install
   ```

4. **Configure Firebase:**
   * Open the `src/App.jsx` file.
   * Locate the `firebaseConfig` object.
   * Replace the placeholder values with your actual Firebase project configuration keys, which you can find in your Firebase project settings.

5. **Set up Firebase Services:**
   * In your Firebase project, enable **Authentication** (with the "Anonymous" sign-in provider enabled) and **Firestore Database** (start in test mode for local development).

6. **Run the development server:**
   ```bash
   npm run dev
   ```
   The application will now be running at `http://localhost:5173`.

---

## 5. Deployment

To publish this website online, you can use Firebase Hosting.

1. **Build the project:**
   ```bash
   npm run build
   ```
   This creates a `dist` folder with the optimized production files.

2. **Deploy using the Firebase CLI:**
   ```bash
   firebase deploy
   ```
   Follow the command-line instructions to deploy the contents of the `dist` folder.
