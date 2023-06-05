# SQL-Analysis-Finding-best-performing-Salespeople-and-Products

### Business Context. 

You work for AdventureWorks, a company that sells outdoor sporting equipment. The company has many different locations and has been recording the sales of different locations on various products. You, their new data scientist, have been tasked with the question: What are our best products and salespeople and how can we use this information to improve our overall performance?

You have been given access to the relevant data files with documentation from the IT department. Your job is to extract meaningful insights from these data files to help increase sales. First, you will look at the best products and try to see how different products perform in different categories. Second, you will analyze the best salespeople to see if the commission percentage motivates them to sell more.

### Business Problem. 
Your task is to write queries in SQL to carry out the requested analysis.

### Analytical Context. 
You are given the data as a SQLite database. The company has been pretty vague about how they expect you to extract insights, but you have come up with the following plan of attack:

Load the database and ensure you can run basic queries against it
Look at how product ratings and total sales are related
See how products sell in different subcategories (bikes, helmets, socks, etc.)
Calculate which salespeople have performed the best in 2014
See if total sales are correlated with commission percentage
Of course, this is only your initial plan. As you explore the database, your strategy will likely change.

Overview of the data
The data for this case is contained in the AdventureWorks.db SQLite database. We will be focusing on the tables that belong to the Sales and Product categories. Complete documentation, with schemas, for the original data (of which you have only a subset) can be found here.

Product Tables (Pg. 34 in documentation):

Product: one row per product that the company sells
ProductReview: one row per rating and review left by customers
ProductModelProductDescriptionCulture: a link between products and their longer descriptions also indicating a "culture" - which language and region the product is for
ProductDescription: a longer description of each product, for a specific region
ProductCategory: the broad categories that products fit into
ProductSubCategory: the narrower subcategories that products fit into
Sales Tables (Pg. 71 in documentation):

SalesPerson: one row per salesperson, including information on their commission and performance
SalesOrderHeader: one row per sale summarizing the sale
SalesOrderDetail: many rows per sale, detailing each product that forms part of the sale
SalesTerritory: the different territories where products are sold, including performance
CountryRegionCurrency: the currency used by each region
CurrencyRate: the average and closing exchange rates for each currency compared to the USD
Tip: Review the documentation carefully to learn more about the tables (like relevant columns in each) and the relationships between them. Note that not all columns may be available in the subset provided in this case as they are not necessary for the following exercises.
