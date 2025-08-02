# SQL-50-LeetCode-Challenges
SQL 50 Leet Code challenges — part of my learning path towards becoming a Data Analyst in the Oil &amp; Gas domain.


👩‍🎓 **Created by:** Karishma Bhavani Maddimsetti  
🎓 Petroleum Engineer | Aspiring Data Analyst


## 📍 About This Project

I am currently learning **SQL** to enhance my data analysis skills, especially for Oil & Gas Data Analytics.  
This repository contains my solutions to the **Top 50 SQL questions** on LeetCode.

It will help me in:
- Oil & Gas data projects
- Real-time data monitoring
- Data Analyst role preparation



### 📝 Task 1: Recyclable and Low Fat Products

#### Problem:

Given a table Products:


| Column Name | Type    |
|-------------|---------|
| product_id  | int     |
| low_fats    | enum    |
| recyclable  | enum    |
   


**Goal:**  
Find the product IDs where:
- The product is low fat (`low_fats = 'Y'`)
- The product is recyclable (`recyclable = 'Y'`)

#### Example:

Input: 
Products table:

| product_id | low_fats | recyclable |
|------------|----------|------------|
| 0          | Y        | N          |
| 1          | Y        | Y          |
| 2          | N        | Y          |
| 3          | Y        | Y          |
| 4          | N        | N          |

Output: 
| product_id |
|------------|
| 1          |
| 3          |


#### Solution Explanation:

**ENUM **is used for predetermined values in `low_fats` and `recyclable`.
**product_id** is a **primary key**, so it stores unique values only.
We use **WHERE** clause to filter rows where both `low_fats` and `recyclable` are `'Y'`.

#### SQL Query:

```sql
-- LeetCode #1757 Recyclable and Low Fat Products

SELECT product_id
FROM products
WHERE low_fats = 'Y' AND recyclable = 'Y';


## 🚀 More Coming Soon

I will continue solving more problems and update this repository.



## 📧 Connect with Me

* [LinkedIn](https://www.linkedin.com/in/karishma-bhavani-maddimsetti-petroleumengineer)


SQL-50-LeetCode-Challenges/
├── 01_Recyclable_and_Low_Fat_Products.sql
├── README.md



