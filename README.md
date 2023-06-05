# House Prices Data
Using the SQL skills that I’ve learned so far, and the dataset involving house prices information, I will answer a series of questions about the data. I'll be using the houseprices table from the houseprices database for all questions.

## #1
First, I want to write a query that returns a list of distinct values in the yearbuilt field.

<img width="503" alt="1" src="https://github.com/romaoeh/HousingPrices/assets/131217181/cf38dde7-4571-49b0-a947-dc1051a638d6">

## #2
How many unique values are there for the mszoning field (alias as count_mszoning), and mssubclass field (alias as count_mssubclass)?

<img width="504" alt="2" src="https://github.com/romaoeh/HousingPrices/assets/131217181/037f243c-9174-4ed6-a8ca-8884d50893f9">

## #3
Write a query that returns a list of all the unique combinations for street and lotshape, sorted alphabetically by street.

<img width="507" alt="3" src="https://github.com/romaoeh/HousingPrices/assets/131217181/e50720ab-1a4b-4282-9b03-14b98344b2d1">

## #4
Create a report that shows the number of records for each neighborhood and lotconfig pair. Alias the count of records to count_lotconfig. Order the results by neighborhood (A-Z), count_lotconfig (smallest-largest), and lotconfig (A-Z).

<img width="510" alt="4" src="https://github.com/romaoeh/HousingPrices/assets/131217181/3476b6f5-edfb-4cb0-8ee4-25bab61b4815">
<img width="555" alt="4 5" src="https://github.com/romaoeh/HousingPrices/assets/131217181/ec70380d-8c83-40bc-a950-ef7533d4d47c">

## #5
Write a query that returns the average saleprice of houses per yearbuilt — call this field avg_saleprice — rounded to the nearest whole number and sorted from newest to oldest.

Within the first line of the query, use the following code so that the proper data type is used to avoid results displaying in scientific notation:
ROUND(AVG(saleprice),0)::float

<img width="577" alt="5" src="https://github.com/romaoeh/HousingPrices/assets/131217181/accb419c-2b44-43f8-8e6a-95de4b44a816">

## #6
Write a query that shows the average number of cars for the column garagecars (using the alias avg_garage) per yearbuilt. Only include houses that have 1 or more garagecars in this average. Round the answer to the nearest whole number.

Within the first line of the query, use the following code so that the proper data type is used to avoid results displaying in scientific notation:
ROUND(AVG(garagecars),0)::float

<img width="575" alt="6" src="https://github.com/romaoeh/HousingPrices/assets/131217181/14272bb3-0a04-4847-b6d9-8fab859bf232">

## #7
Write a query that shows for each yearbuilt, how many houses had zero garages and the largest lotarea amount for that year.

<img width="572" alt="7" src="https://github.com/romaoeh/HousingPrices/assets/131217181/e9ba513c-82ba-4c2b-9655-f4aba63e1b47">

## #8
For each yearbuilt, find the average lotarea — call it avg_lot_per_year — and return only those results for which the average is smaller than 10,000, sorted high to low.

Within the first line of the query, use the following code so that the proper data type is used to avoid results displaying in scientific notation:
avg(lotarea)::float

<img width="580" alt="8" src="https://github.com/romaoeh/HousingPrices/assets/131217181/b42e8eaa-9a9a-4525-99a4-4810fa2a5d0a">

## #9
Write a query that shows, for each yearbuilt, how many houses had a lotarea between 10,000 and 15,000, inclusive. Finally, order it by yearbuilt from oldest to newest.

<img width="578" alt="9" src="https://github.com/romaoeh/HousingPrices/assets/131217181/7d7a104f-5a08-42ce-953a-32733035bfed">

## #10

Write a query that shows the average overall quality overallqual (rounded to 0 decimals and renamed as avg_quality) and the number of unique garage types (garagetype) renamed as garage_count for each neighborhood, sorted by neighborhood.

Within the first line of the query, use the following code so that the proper data type is used to avoid results displaying in scientific notation:
ROUND(AVG(overallqual),0)::integer

<img width="578" alt="10" src="https://github.com/romaoeh/HousingPrices/assets/131217181/8003ffd8-63d4-4a2a-a052-6a7575078c0e">
<img width="555" alt="10 5" src="https://github.com/romaoeh/HousingPrices/assets/131217181/fe904c57-3546-4b8c-b3e7-bf96d8430961">
