# 🎬 Movie Booking SQL Project

## 📘 Project Overview  
This SQL project is designed to analyze a **Movie Booking System** dataset using core and intermediate SQL concepts. It demonstrates how SQL can be used for **data extraction, transformation, and analysis** to generate insights about movies, bookings, customers, and payments.  

The project focuses on **real-world use cases** such as tracking customer activity, identifying revenue trends, and managing show details using SQL queries.

---

## 🧾 Dataset Information  
The dataset contains multiple tables related to a movie booking system:  
- **Movies** – Movie details like title, genre, and release date  
- **Customers** – Customer profiles and locations  
- **Shows** – Show timings, ticket prices, and theatres  
- **Bookings** – Records of customer bookings and seats booked  
- **Payments** – Payment information with amount and status  
- **Theatres** – Theatre names and IDs  

File: `movie_booking_basic_sql.xlsx`

---

## 🧠 Concepts Covered  
This project includes queries demonstrating:  
- **SELECT & DISTINCT** – Fetch and filter movie and customer data  
- **WHERE & Operators** – Apply conditional filters  
- **ORDER BY** – Sort data by specific columns  
- **GROUP BY & Aggregations** – Summarize seats booked and payments  
- **HAVING** – Filter grouped data  
- **LIMIT & OFFSET** – Retrieve specific record ranges  
- **Subqueries** – Extract dependent query results  
- **JOINS** – Combine data from multiple tables  
- **DELETE** – Manage and clean data  

---

## 🧩 Example Queries  
```sql
-- Find total seats booked per customer
SELECT CustomerID, SUM(SeatsBooked) 
FROM movie_slot.movie_booking_booking 
GROUP BY CustomerID;

-- List movies released in 2024
SELECT * 
FROM movie_slot.movie_booking 
WHERE ReleaseDate BETWEEN '2024-01-01' AND '2024-12-31';
