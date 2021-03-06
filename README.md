# Project-11---Explanatory-Data-Analysis-and-Seaborn-Visualization-Olympic-Games-
The purpose of this project is to gather Olympic data to analyze(explanatory data analysis), clean, merge and visualize with Seaborn.

__The main questions this project will focus on are__: 
1) What countries have been given the most medals in the Winter and Summer Olympics? 
2) What countries have the highest rankings? 
3) Why are some countries more successful than other countries? 

__Method__:
1)Import the data / First Inspection
2)Merging and concatenating
3)Data cleaning
4) visualize data 

Results 

1) Import Data / First Inspection 

- Missing values from countries due to name changes or countries do not exist anymore. Country codes also have changed or become outdated. 
- Both summer and winter datasets use the same columns (easy to concatenate later)
- Some athlete data is pending 
- Data types are correct for given values 


2) Merging and Concatenating 

- Vertical concatenate
- Left join

Concatenating points:
- Summer and Winter data have the same 9 columns which make it easy to concatenate.


3) Data Cleaning 
- Rename column labels as there are blank spaces between labels and unintuitive labels 
- Update missing values with appropriate country names
- Filter out missing values 


Q: What are the most succsseful countries?

United States     5238
Soviet Union      2489
United Kingdom    1799
Germany           1665
France            1548
Italy             1488
Sweden            1477
Canada            1274
Australia         1204
Hungary           1091


- USA is the highest ranking country collectivaly with 14% overall winnings of medals.
- Soviet Union is 2nd ranked country collectivaly with 6% overall winnings of medals.
- USA has the most gold, silver and bronze medals won(winter / summer medals combined) than any other country. 
- Some countries perform well in the Summer games but poorly in the winter games (refer to graphs for further inspection)

Q: Do GPD, Population and Politics matter?
(Since each country has its own unique situation with population, GDP and politics do these factors influence countries success rate?)

Hypothesis:
- Higher the GDP the more successful the athletes
- Larger population leads to more medals
- Countries that have been participating longer in the games are more successful


__Statistical Analysis and Hypothesis Testing with Scipy__
 -Testing the relationships between countries GDP, population and political stability.

__Method__:
 - Test correlation methods Pearson / Spearman

__Perform hypothesis test with Scipy__
 - Hypothesis 1: There is no relationship between Total Medals and Population.
 - Reject Hypothesis 1 -> There is a significant (positive) relationship between Total Medals and Population.
 
 - Hypothesis 2: There is no relationship between Total Medals and GDP per Capita.
 - Reject Hypothesis 2 -> There is a significant(positive) relationship between Total Medals and GDP Capita.
 
 - Hypothesis 3: There is no relationship between Total Medals and Participations.
 - Reject Hypothesis 3 -> there is a significant (positive) relationship between Total Medals and Participations.
 
 __Aggregating and Ranking__:  
 Heatmap displays which country are more successful and for Summer or Winter games and displays the amount of medals each gender has won:

- Differentiate between Summer and Winter game medals for each country 
a: Countries where winter is more promiment tend to do better in winter games than summer games. 
- What gender has more medals?
a: Genrally males are have a higher success rate due to participations are more males.    


__Summer vs Winter Games - Does Geographical Location Matter?__
- Geographical and climatical location has a big impact on the overall success of a country in the Winter/Summer games.
- Some countries are exposed to both hot and cold climates allowing them to participate in both games more successfully (USA, South Korea, East Germany).
- Climate can influence what games that country focuses on.

__Do Traditions matter?__
- Some countries have a long history of sports that are more traditionally played in that country.
a: Each country has sports that are better performed/ traditonally practiced. For example, Taekwondo is the national sport of South Korea and perfroms well at the olympics. Whereas USA it is not and has a very low ranking in that sport category.
Must take into account what each country hold as a traditional sport n their own country and compare it to its ranking of success.

