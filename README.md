# Education Comparison of U.S. Counties by Political Affiliation and Secondary Completion of African Countries

## What is it?
* An analytical snapshot of educational performance across US counties and their relation to the 2016 presidential election.
* Examination of education growth in high performing African nations.
* Comparisons of Africa’s highest secondary completion rates by median income.
* A small (and my first published python!) project inspired by POTUS’s recent comment. 

## What tools were used?
* Python in a Notebook environment
* The following packages: Pandas, Matplotlib, Seaborn
* The Quandl API to pull World Bank Data


## Methodology
The code was written in three parts, based on the data sets used. The scripts can be found in the consolidated GitHub files.
1. U.S. Census education county data was cross referenced with the election results to classify “Trump” and “Clinton” counties. This data was analyzed and visualized, comparing education levels and candidate affiliation.
2. UNESCO Education data was cross reference with 2011 World Bank poverty information to assign income and secondary education values to available African nations. The Quandl API was used to extract World Bank secondary enrollment rates, and five African nations, ranked by highest secondary completion, were compared to the secondary enrollment rate of the United States from 2000 to 2015.
3. Finally, the two analyses were compiled together. A visualization was created to compare 10 African nations with the highest secondary completion rate found against 10 U.S. counties with the least amount of high school graduates which voted for Hillary Clinton and a similar grouping of 10 counties which voted for Donald Trump in 2016. 

## Summary

#### U.S. County Education Data by 2016 Presidential Election Results

This data was pulled from 2014 U.S. Census estimates. Here’s some interesting tidbits:

* After the available education data was cross-referenced with the available election data, a dataset of 3,108 U.S. counties was produced. 2,625 of these counties voted for Trump and 486 of these counties voted for Clinton. 
* Averaging the county data, it was found that the population in the average  “Trump county” consisted of 88.6% high school graduates. The average “Clinton county” was made up of 95.7% high school graduates.

![Imgur](https://i.imgur.com/zubnKge.png)

* Furthermore, the average “Trump county” consisted of 16.8% Bachelor degree holders whereas the average “Clinton county” was found with 51.9% Bachelor degree holders. 

![Imgur](https://i.imgur.com/GuvGZf9.png)

* Unlike the education values, the average “Trump county” skewed a higher median income at $41,988 with the “Clinton counties” averaging a median income of $34,702.

![Imgur](https://i.imgur.com/y3w9yfu.png)

* An aggregate visualization of all county data compiled with relation between the Bachelor education and median income showed overall correlation between higher education and higher income. It also becomes clear that highest earning counties were the ones which voted for Clinton.

![Imgur](https://i.imgur.com/YT3APmC.png)

#### Education and Income Data by African Nation

The available data for each African country was noticeably more incomplete. Information was not available for every African nation, and when it came to cross-referencing income and education data, the available pool became even smaller. 

* UNESCO data was used to determine upper secondary completion rates for available countries. The three nations with the highest completion rates were Egypt (70%), South Africa (50%), and Nigeria(49%).
* World Bank data analyzed by the Center for Global Development was used to determine annual median countries for available African nations. Notably, Egypt’s median income was not available in this data set. The countries with the highest median incomes were found to be in Seychelles ($13,687.50), Mauritius ($9,909.75), and Tunisia ($8322)

![Imgur](https://i.imgur.com/PgN6gMU.png)

#### Comparing Education Data

Comparisons were then made between the highest performing African nations in education and the United States. 

* Upper secondary enrollment rate data over time was pulled from World Bank Education Statistics. The United States was compared to the five African nations with the highest enrollment rates. 

![Imgur](https://i.imgur.com/vZ9cxIW.png)

* The 10 African nations with the highest secondary completion rates were then compared to the 10 “Trump counties”  and the 10 “Clinton counties” with the lowest high school graduation rates.

![Imgur](https://i.imgur.com/vZctrhz.png)

## Data Sources
* [2014 estimates from the U.S. Census Bureau’s 2012-2016 American Community Survey 5-Year Estimates](https://factfinder.census.gov/faces/tableservices/jsf/pages/productview.xhtml?pid=ACS_16_5YR_S1501&prodType=table) 
* [UNICEF global statistics on secondary education](https://data.unicef.org/topic/education/secondary-education/) 
* [2016 presidential election results by county from Kaggle](https://www.kaggle.com/stevepalley/2016uspresidentialvotebycounty)
* [World Bank Education Statistics](https://www.quandl.com/data/WEDU-World-Bank-Education-Statistics)
* [Income values from the World Bank as analyzed by the Center for Global Development](https://www.cgdev.org/blog/world-bank-poverty-statistics-lack-median-income-data-so-we-filled-gap-ourselves-download-available) 
