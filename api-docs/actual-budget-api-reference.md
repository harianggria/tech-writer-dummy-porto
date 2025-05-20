# Actual Budget API Reference

## Base URL
http://localhost:5000/api

## 📘 Budget Endpoints

### `GET /budgets`

**Description:**  
Retrieve a list of all budgets.

**Response Example:**
```json
[
  {
    "id": "budget-1",
    "name": "Personal Budget",
    "total": 15000000
  }
]
```

### `POST /budgets`

**Description:**  
Create a new budget.
**Request Body :**
```json
{
  "name": "Monthly Expenses",
  "total": 2000000
}
```
**Response Example :**
```json
{
  "id": "budget-2",
  "name": "Monthly Expenses",
  "total": 2000000
}
```

## 📘 Transaction Endpoints
### `GET /transactions`

**Description:**  
Retrieve all transactions.

**Response Example:**
```json
[
  {
    "id": "tx-1",
    "amount": 50000,
    "budgetId": "budget-1",
    "description": "Groceries"
  }
]
```
### `POST /transactions`

**Description:**  
Create a new transaction.

**Request Body:** 
```json
{
  "amount": 50000,
  "budgetId": "budget-1",
  "description": "Groceries"
}
```
**Response Example:**
```json
{
  "id": "tx-2",
  "amount": 50000,
  "budgetId": "budget-1",
  "description": "Groceries"
}
```

