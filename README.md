# DatabaseDesign
**This Repository showcases the implementation of Database and Warehouse for the Wine Company**

## Problem Statement 
The file path DB_Design/Problem_Statement.doc demonstrates the background of the Wine company and its day-to-day operations. 
It contains the Database design and development requirements that needs to be fullfilled.

## Solution Design

This report demonstrates the day-to-day operations of a Wine-stopper Website that allows the customers to place online orders for Wine of their choice. Also, it will demonstrate the backend operations of a Distribution center stocking and ordering the wines from their respective warehouses when the stock needs to be replenished.
The Wine can be categorized as per Colour, Country, Sweetness Indicator.  Additionally, there are various promotions on the offer with different types and delivery charge calculations. All of these factors are taken into consideration while designing the problem statement.
The objective of this report is to get a holistic view of Wine Stopper day-to day operations that includes following -
1.	Customer adding Items into their shopping basket
1.	Customer adding items into their shopping list
1.	Customer placing an order to generate an invoice
1.	Distribution center placing Standing Order for wine from the warehouse
1.	Distribution center placing Special Order for wine from the warehouse
1.	Promotions applied for shopping and its related calculations
1.	Delivery charges calculation 
1.	Stock maintenance and updates at the distribution center
1.	Setting the Expiry to the Shopping List (Wish List) and to clear it if it is more than 60 days

The first part of the report is mentioning about the ER Diagram that will be highlighted with the assumptions and constraints while designing the entity relationships.
This Diagram is classified into 3 main parts with corresponding entities designed as described below



| **Part**                         |     **Main and Supporting Entities**                                                | **Entities (Tables)**                                                       |
| ---------------------------- | ---------------------------------------------------- | ------------------------------------------------------------------------- |
| ***Wine Entities***               | Main                                                 | WS\_WINE, WS\_WINE\_DETAILS                                               |
|                              | Supporting                   | WS\_WINE\_CATEGORY, WS\_WINE\_INDICATOR, WS\_COUNTRY |
| ***Customer Entities***           | Main                                                 | WS\_CUSTOMER, WS\_SHOPPING\_BASKET, WS\_SHOPPING\_LIST, WS\_INVOICE       |
|                              | Supporting                   | WS\_PROMOTION, WS\_CALCULATE\_DELIVERY\_CHARGE       |
| ***Distribution Center Entities*** | Main                                                 | WS\_CENTER, WS\_WAREHOUSE, WS\_STOCK\_INFO, WS\_ORDER, WS\_ORDER\_DETAILS |
|                              | Supporting                   | WS\_REGION, WS\_LOCATION, WS\_ORDER\_TYPE            |

## Designing the DB schema using the ER diagram
The file path DB_Design/DB_Assignment_ER_Diagram.pdf leads to the database ER diagram that was designed for the Wine company 

## Demonstration of OLTP queries for day-to-day operations
This is section 4 of the problem statement questions and has 5 OLTP queries for Wine Company's day-to-day operations.
Refer file path DB_Design/SQL_Queries_for_OLTP_Transactions.txt.

## Database Design Report
The report of the problem statement is created and consist of chapters for introduction, ER Diagrams, Implementation, SQL query demonstration for OLTP transactions and Conclusion.
The report can be referred at DB_Design/DatabaseAssignment-Report-Final.docx


#Data Warehouse Design

## Problem Statement 
The file path Warehouse_Design/Problem_Statement.doc demonstrates the ask for the assignment.

## Star Schema
The star schema is desinged for the Fact and Dimension table and can be referred using Warehouse_Design/Star_Schema.pdf.
The design was done using Visio.

The data warehouse grain to design the Fact table in the Star schema is as below

> ***“Wine purchase made by a customer in an invoice transaction taking into account the promotion offers and discount” ***


## Warehouse Design Report
The report of the problem statement is created and can be referred at Warehouse_Design/Data_Warehouse-Report-Final.docx
