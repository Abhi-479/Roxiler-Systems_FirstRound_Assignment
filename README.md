# Roxiler-Systems_FirstRound_Assignment
# MERN Stack Transaction Dashboard

This project is a MERN (MongoDB, Express, React, Node.js) stack application with a simple frontend using HTML, CSS, and JavaScript. The application displays and manages product transactions using backend APIs and includes interactive data visualizations.

## 🚀 Features

- Fetches transaction data from a third-party API and seeds it into the database.
- Backend APIs provide:
  - Listing and searching transactions with pagination.
  - Transaction statistics (total sales, sold items, unsold items).
  - Price range distribution for a bar chart.
  - Category distribution for a pie chart.
  - Combined API to aggregate data.
- Frontend built with plain HTML, CSS, and JavaScript:
  - Displays transactions in a searchable and paginated table.
  - Visualizes data using bar and pie charts.
  - Dropdown for selecting a month to filter data.

---

## 🛠️ Technologies Used

### Backend:
- **Node.js**: Runtime environment.
- **Express.js**: Framework for building APIs.
- **MongoDB**: Database for storing transaction data.

### Frontend:
- **HTML**: Structure of the application.
- **CSS**: Styling and layout.
- **JavaScript**: Interactive functionality and API integration.
- **Chart.js**: For rendering bar and pie charts.

---

## 📚 API Endpoints

### 1. **Initialize Database**
- **URL**: `/api/initialize`
- **Method**: `GET`
- **Description**: Fetches data from the third-party API and seeds the database.

### 2. **List Transactions**
- **URL**: `/api/transactions`
- **Method**: `GET`
- **Query Parameters**:
  - `month` (required): Month to filter transactions (e.g., January).
  - `search`: Search term for title/description/price.
  - `page`: Page number (default: 1).
  - `perPage`: Items per page (default: 10).

### 3. **Transaction Statistics**
- **URL**: `/api/statistics`
- **Method**: `GET`
- **Query Parameters**:
  - `month` (required): Month to filter transactions.

### 4. **Bar Chart Data**
- **URL**: `/api/bar-chart`
- **Method**: `GET`
- **Query Parameters**:
  - `month` (required): Month to filter transactions.
