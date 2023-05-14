# plato-pizza
## Introduction
Plato Pizza is a restaurant that deals with sales of all varieties of pizza. Currently, things are going smoothly but there seem to be a room for improvement.The management at Plato Pizza have been collecting transactional data for the past year, but really haven't been able to put it to good use. The management hopes the  transactional data can be analyzed and insights derived to foster the growth of the business to drive more sales and work more efficiently

## Statements of Problem
Mr Mario Maven (Manager, Plato's Pizza), hopes to find answers to the following questions:<br> 
• What days and times do we tend to be busiest? <br> 
• What are our best and worst selling pizzas? <br> 
• What's our average order value? <br> 
• How much money did we make this year? Can we identify any seasonality in the sales?<br> 

## Data Source
The dataset can be found [here](https://drive.google.com/drive/folders/1sT5AReif21UXjW1kICtZPrBb8yshNSOs). This dataset contains 4 tables in CSV format.<br> 
• The **Orders** table contains the date & time that all table orders were placed.<br> 
• The **Order Details** table contains the different pizzas served with each order in the Orders table, and their quantities.<br> 
• The **Pizzas table** contains the size and price for each distinct pizza in the Order Details table, as well as its broader pizza type.<br> 
• The **Pizza Types** table contains details on the pizza types in the Pizzas table, including their name as it appears on the menu, the category it falls under, and its list of ingredients.<br> 

## Data Cleaning (Extract, Transformation, Loading)

## Data Modelling
• Fact table: order details table <br> 
• Dimensional table: Pizzas types, Orders tables<br> 
• Bridge Table: Orders and Pizza tables<br> 
• Date Table : CalendarTable<br> 
![model](https://github.com/anibihakeem/plato-pizza/assets/105971924/25fd3ae5-2591-4046-91f2-01f2d691fe28)
