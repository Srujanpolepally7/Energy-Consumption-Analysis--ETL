# ETL : Extract, Transform, Load Project:
__Extract:__ read the data, often from mupltiple sources/formats.

__Transform:__ clean and structure the data to suit business needs.

__Load:__ load the data into a database for storage that can be used for future analysis or business use.


#### Members:  __[Kristen,](https://github.com/KCDataVis)__ __[Mary,](https://github.com/marygong75)__ __[Michael](https://github.com/mkung8889)__

__[Project Repo](https://github.com/mkung8889/etl_project)__


###  Objective: 
##### Each of us chose (2) data sources to analyze different international energy sources consumed annually over the years.

#### Discussion Questions & Answers:

1. Data sources:

1) __[UN Data Total Electicity Consumption](http://data.un.org/Default.aspx)__ 

2) __[EIA Electricity Consumption By State](https://www.eia.gov)__ 

3) __[EIA Natural Gas Consumption](https://www.eia.gov)__

4) __[UN Data Natural Gas Consumption](http://data.un.org/Default.aspx)__

5) __[Enerdata World Oil Consumption](https://yearbook.enerdata.net/oil-products/world-oil-domestic-consumption-statistics.html)__

6) __[EIA International Coal Consumption](https://www.eia.gov/beta/international/data/browser/#/?pa=0000000000000000000000000000000000000000000000000000000000g&c=ruvvvvvfvtvnvv1vrvvvvfvvvvvvfvvvou20evvvvvvvvvvvvuvs&ct=0&vs=INTL.4411-2-AFG-QBTU.A&vo=0&v=H&start=1990&end=2016)__

All data extracted were in CSV format

2. Decisions you made to do cleanup (transform) and join (transform)

- Wrote a function to get the list of countries from UN database, it creates a country ID for unique countries, and this is used for joining purpose. 

- Renaming column names since SQL columns cannot start with an integer

- drop rows that contained ‘NA’ data

- converting string to nummeric


3. How you decided on database tech to store, and schema to store

All of our data were in a CSV format, so we went with SQL to store the data.



4. Potential analysis to do on the newly formed dataset

Compare energy consumption based on countries and year, create bar chart to see the trend of increasing energy usage, conduct analysis on why certain countries may consume more energy compare to other – this will require other data sets (country population for example).


5. Challenges you overcame:

- finding data that can be used for the project (relatable to what everyone else were finding year wise)

- finding data based on countries instead of areas/continents

- dropping unnecessary data and renaming columns in order to input it into SQL database

- converting values from string to numeric data type

- creating table in relation to SQL and jupyter notebook

- learned how to use lambda


