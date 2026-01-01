# Vehicle Rental System – Database Design & SQL Queries

## 📌 Project Overview
This project demonstrates the design and implementation of a **Vehicle Rental System** using relational database concepts.  
It focuses on **ERD design**, **table relationships**, and **SQL queries** using `JOIN`, `EXISTS`, `WHERE`, `GROUP BY`, and `HAVING`.

The system manages:
- Users
- Vehicles
- Bookings

---

## 🎯 Objectives
- Design an ERD with correct relationships
- Implement tables using Primary Keys and Foreign Keys
- Write SQL queries to retrieve meaningful business data
- Practice SQL concepts for viva and interviews

---

## 🗂 Database Tables

### Users
Stores user information such as customers and admins.

**Fields:**
- user_id (PK)
- name
- email (UNIQUE)
- phone
- role (Admin / Customer)

---

### Vehicles
Stores vehicle details available for rent.

**Fields:**
- vehicle_id (PK)
- name
- type (car / bike / truck)
- model
- registration_number (UNIQUE)
- rental_price
- status (available / rented / maintenance)

---

### Bookings
Stores booking information linking users and vehicles.

**Fields:**
- booking_id (PK)
- user_id (FK → users)
- vehicle_id (FK → vehicles)
- start_date
- end_date
- status (pending / confirmed / completed / cancelled)
- total_cost

---

## 🔗 Relationships
- **One-to-Many:** One user can have many bookings
- **Many-to-One:** Many bookings can reference one vehicle
- **One-to-One (Logical):** Each booking links exactly one user and one vehicle

---

## 🧪 SQL Queries Explanation

### Query 1 – INNER JOIN
Retrieves booking information along with customer name and vehicle name.

### Query 2 – NOT EXISTS
Finds vehicles that have never been booked.

### Query 3 – WHERE
Retrieves available vehicles of a specific type.

### Query 4 – GROUP BY & HAVING
Finds vehicles that have more than two bookings.

All queries are available in `queries.sql`.

---

## 📎 Submission Links
- **GitHub Repository:** (Add your repo link here)
- **ERD Link:** (Lucidchart public link)
- **Viva Video Link:** (YouTube / Google Drive public link)

---

## 📝 Author
Prepared for database design and SQL practice assignment.
