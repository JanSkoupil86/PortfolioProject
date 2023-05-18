# PortfolioProjectSQL
In the provided code, you are performing data exploration on Covid-19 data using SQL. Here's an overview of the operations and the SQL skills utilized:

Selecting Data:

Selecting all columns from the CovidDeaths table in the PorfolioProjectSQL1.dbo database where the continent is not null.
Ordering the results by the third and fourth columns.
Total Cases vs Total Deaths:

Comparing the total cases and total deaths in each location and calculating the death percentage.
Filtering records where the location includes 'states' and the continent is not null.
Ordering the results by location and date.
Total Cases vs Population:

Comparing the total cases with the population in each location and calculating the percentage of population infected.
Ordering the results by location and date.
Countries with Highest Infection Rate compared to Population:

Grouping records by location and population to find the highest infection count and the percentage of population infected.
Ordering the results by the percentage of population infected in descending order.
Countries with Highest Death Count per Population:

Grouping records by location to find the maximum total death count.
Ordering the results by the total death count in descending order.
Breaking Things Down by Continent:

Grouping records by continent to find the maximum total death count per population.
Ordering the results by the total death count in descending order.
Global Numbers:

Calculating the sum of new cases, total deaths, and the death percentage on a global level.
Grouping the results by date.
Ordering the results by the total cases and total deaths.
Total Population vs Vaccinations:

Joining the CovidDeaths and CovidVaccinations tables on location and date.
Calculating the rolling sum of new vaccinations per location.
Ordering the results by location and date.
Using CTE to Perform Calculation:

Utilizing a Common Table Expression (CTE) to perform calculations on the partitioned data from the previous query.
Calculating the percentage of population vaccinated by dividing the rolling sum of vaccinations by the population.
Temp Table:

Creating a temporary table #PercentPopulationVaccinated to store the results of the vaccination analysis.
Inserting data into the temporary table using a similar query as the previous step.
Creating a View:

Creating a view named PercentPopulationVaccinated to store the data for later visualizations.
The view includes columns for continent, location, date, population, new_vaccinations, and the rolling sum of vaccinations.
Selecting from the View:

Querying the PercentPopulationVaccinated view to retrieve all records.


The SQL skills used in this code include joins, Common Table Expressions (CTEs), temporary tables, window functions, aggregate functions, creating views, and converting data types
