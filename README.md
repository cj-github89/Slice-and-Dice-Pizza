# Slice-and-Dice-Pizza
A summary of sales data for Slice and Dice Pizza company using Excel and Power BI

**Original data set:**

https://www.kaggle.com/datasets/mexwell/pizza-sales

**Objective:**

To create a dashboard summarising sales data for the fictional company Slice and Dice Pizza. The design of the dashboard should be in the style of the Contoso Skateboard Store dashboard (see attached word document for screenshot).

**Method:**

Along with the CSV file, Kaggle had some text available in the Data Card section that detailed the fictional menu items. I copied this and used Excel to create a Menu table to be used in analysis.
I connected the Excel file to Power Query and transformed the data to establish several dim tables, setting their relationships to the fact_sales table. It was necessary to form a bridge table to allow for analysis of individual ingredient use.

Once the model was loaded to Power BI, I was able to add a custom date table using DAX along with several custom measures.
I built out a high-level sales summary page using a combination of shapes, text boxes and visuals to emulate the Contoso example as closely as possible. I expanded the report adding two further pages in the same style.

**Pages:**

_Summary_ 

A high-level summary of sales by revenue and by volume. Sales are broken down by category and size. The menu performance is summarised by showing the top ten and bottom ten performing pizzas by revenue (sales).

_Sales Trends_

This page looks at averages over time which would assist the business owner to make staffing and stock decisions. To accurately calculate the average pizzas sold per hour, it was necessary to add a calculated table to the model (DateHourTable) which included an entry for each hour of each day included in the data set and provided the total number of pizzas sold during that period. From this, I was able to include the zero values necessary to calculate a true average for each time period.

Measures were added to allow for day of week and day of month averages to be calculated and plotted. As only one year of data was available, totals were provided in place of averages for the monthly summary.

_Ingredients_ 

The final page summarises the individual ingredient use with the idea being that this assists with stock planning and management.  A matrix is provided giving actual volumes used per week of year. Cards illustrate that as many as 38 ingredients are used in as little as one pizza type. A tree map illustrates the top ten most versatile ingredients.

**Conclusion:**

I enjoyed working with this data set and the challenge of creating the right data structure to allow me to illustrate the menu elements. The design challenge forced me to explore all the formatting options available to me, learning as I did, and mimicked the business scenario where a client requests an existing portfolio of reports is expanded. 

I am pleased with the resulting report and welcome any thoughts, feedback or questions.

