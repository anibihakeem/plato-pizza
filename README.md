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

## Data Cleaning and Transformation
Dataset cleaning process took place using power query by;<br> 
• Checking for duplicates and empty rows<br>
• Validation of data to ensure they are in the appropriate format<br>
• Inconsistency in dataset<br>
• Checking for missing data from each columns<br>

## DAX Measures 
• Hour Column <br>
![Hour](https://github.com/anibihakeem/plato-pizza/assets/105971924/2d7b6755-1591-4fef-bc82-bd06bb112a4f) <br>
• Revenue Column <br>
![Revenue](https://github.com/anibihakeem/plato-pizza/assets/105971924/1385119e-fac5-4494-8d7a-0f12a1b9b11f)<br>
• AVG Order Value <br>
![AVG Order Value](https://github.com/anibihakeem/plato-pizza/assets/105971924/fd6159f4-637c-4b6f-91d0-ffaddfe28c49)<br>
• AVG Quantity per Order <br>
![AVG Quantity per Order](https://github.com/anibihakeem/plato-pizza/assets/105971924/b4e8650a-ca65-47e5-857a-c045b5cc92ac)<br>
• A calendar table was created, consisting of Date, Year, Month, MonthNumber, Day, Quarter, Weekdays columns<br>
![Calendar DAX](https://github.com/anibihakeem/plato-pizza/assets/105971924/226b636a-40a9-402a-8f11-e608fd28c345)<br>
<br>

## Data Modelling
• Fact table: order details table <br> 
• Dimensional table: Pizzas types, Orders tables<br> 
• Bridge Table: Orders and Pizza tables<br> 
• Date Table : CalendarTable<br> 
![model](https://github.com/anibihakeem/plato-pizza/assets/105971924/25fd3ae5-2591-4046-91f2-01f2d691fe28)

## Data Analysis and Insights
• With a total revenue of $818k from over 20k orders resulting into 50k pizzas been sold, the revenue figures show monthly fluctuations throughout the year. There was an average order value of $38.  The highest revenue was recorded in July (72.6k), followed closely by May ($71.4k). The lowest revenue was in October $64.0k, followed by September $64.2k. There seems to be a pattern of higher revenue during the summer months (May to July) and lower revenue towards the end of the year (September to December). This suggests a possible seasonal influence on the business's revenue with a potential correlation between warmer months and increased business activity. The latter part of the year witnessed a dip in revenue. October marked the lowest point with $64.0k, followed by a marginal increase in November to $70.4k. December concluded the year with revenue amounting to $64k. This downward trend may indicate a seasonal slowdown or external factors impacting consumer behavior and spending habits during the holiday season. Despite the monthly fluctuations, our revenue remains relatively stable within a specific range between $64k and $72.6k. 
![metrics](https://github.com/anibihakeem/plato-pizza/assets/105971924/202cc682-1da9-4a92-adef-24e820436a44)
![trend](https://github.com/anibihakeem/plato-pizza/assets/105971924/7a032e73-7f00-44a2-a380-81f9e625de76) <br>
•The hour of 12 PM (noon) stands out as the peak time for receiving orders, with a substantial volume of 2,520 orders. This indicates that customers tend to make their purchases during the lunchtime period. Following closely, the hours of 1 PM and 5 PM show considerable order activity, with 2,455 and 2,366 orders respectively. These hours likely correspond to the post-lunch and late afternoon periods when customers are still active in making their purchases. There is a consistent pattern of higher pizza orders during the weekends. On Fridays, the number of orders significantly increases to 3.5k , indicating a strong demand for pizza at the start of the weekend, possibly as a treat or as part of their leisure activities. The consistent demand throughout the midweek indicates that pizza remains a popular choice for convenient and enjoyable meals, even during busy weekdays. Sundays show the lowest number of pizza orders compared to other weekdays, with 2,600 recorded. This could be attributed to various factors, such as individuals spending time with family or cooking at home.
![busy orders](https://github.com/anibihakeem/plato-pizza/assets/105971924/6d079986-14cb-4a4e-a15d-4fbe9c3fc3da)<br>
•THAI CHICKEN PIZZA - large size emerges as the highest revenue-generating pizza with a revenue of $29k and 1365 pieces been sold. With the lowest revenue of $1,000, The GREEK PIZZA - XXL  indicates a relatively lower demand for this particular variety.
![top and bottom](https://github.com/anibihakeem/plato-pizza/assets/105971924/57a58ca3-c30a-404b-9214-2969caf30100) <br>

## Recommendations
•Recognizing the higher demand on weekends, we can focus the marketing efforts and promotions during these days to attract more customers and increase sales. Nevertheless, we can also ensure sufficient staffing and resources during peak hours to meet customer demand efficiently and provide excellent service. We can consider offering lunchtime specials or promotions to attract more customers during the peak hours of 12 PM to 1 PM. This can help increase order volume and overall revenue during this period
<br>
•Capitalizing on Popular Pizzas; the top-performing pizzas, such as the Thai Chicken L, Five Cheese, and Four Cheese, indicate a strong customer demand. We can consider promoting these pizzas through targeted marketing campaigns and special offers to further boost their popularity and drive additional revenue
<br>
•The bottom-performing pizzas, such as The Greek, Calabrese, Chicken Alfredo, Green Garden, and Mexicana, may require some attention. We can further evaluate their recipes, pricing, and marketing efforts to identify potential areas for improvement. Furthermore, we can consider revising the toppings, exploring customer feedback, or repositioning these pizzas to increase their appeal
<br>
•To boost overall revenue, implementing an online ordering system can be a highly effective strategy. The convenience and accessibility of online ordering have become increasingly popular among customers, and tapping into this trend can significantly expand your customer base and increase sales.

## Data Visualization 
For better interaction with the dashboard, click [here](https://app.powerbi.com/view?r=eyJrIjoiYzM3MWFmN2EtOTM5NC00YjYzLWJhNTItMDFhODU4ZTdmMDNhIiwidCI6ImRmODY3OWNkLWE4MGUtNDVkOC05OWFjLWM4M2VkN2ZmOTVhMCJ9) <br>
Note: Two buttons ("Visuals", "Insights") were added to alternate easily between the visuals and insights of the report. Hence, CTRL + click on button to alternate <br>

![Plato](https://github.com/anibihakeem/plato-pizza/assets/105971924/8adab0f1-a1ec-410f-aae7-c8c7a830c0c8)





