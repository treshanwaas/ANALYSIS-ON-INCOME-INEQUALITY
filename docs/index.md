## SUMMARY PAPER 
*For indept analysis please go to the github repository 

## INTRODUCTION 
As the world becomes more global and the distribution of wealth continues to diminish, it is important to understand how the inequality of income has changed over time and space. We chose to use the World Income Inequality Database (WIID) to analyze the trends and patterns to determine whether income inequality exists in developing and developed nations alike despite the global economic growth and that the gap is diverging.
In order to validate our hypothesis, that income inequality does exist around the world, we decided to take a three pronged approach to investigate global wealth distribution over time, analyze income inequality over geographic regions as well as compare and contrast the top and bottom wealthiest populations within each country over time.
The basis of our analysis revolves around Gini coefficients calculated for each country in a specified year. The higher the value, the larger the inequality of income or wealth is and the lower the value, the lesser the inequality of income or wealth exists within that country. This can be calculated based on a few different resource types including consumption, net income and net/gross income.
In addition to the Gini coefficients, the group analyzed the share of per capita net and gross income among population among various geographic regions and subregions to demonstrate this inequality. This analysis highlights that the wealth/income controlled by the top 10% of the population in any given region is higher than the bottom 40% of the population in all areas and even greater in developing regions.

## KEY PARAMETERS
• Gini Coefficient – Measured from 1 – 100. Higher Gini coefficient means higher income inequality in a country and vice versa
• Gross domestic product (GDP) – used in this analysis as a proxy for wealth of a country
• Resource Share - % share of national resources (income, consumption earnings etc) for various population distributions (deciles: 1-10, quintiles: 1-5, top 5, bottom5) e.g. d10   represents the richest 10% of the population and q5 the richest 20%

## DATA SOURCES
The data source for inequality was extracted from the World Income Inequality Database (WIID) from the United Nations University World Institute of Development and Economic Research (UNU-WIDER).
https://www.wider.unu.edu/project/wiid-%E2%80%93-world-income-inequality-database
The WIID data is collected from various sources including the national statistical authorities. Luxembourg Income Study (LIS) is by far the highest quality comprehensive data source with wider coverage of all geographic regions. Since this data is reported by a statistical analysis body of each country or a research study at various inconsistent intervals some parts of our analysis supplemented GDP data from the World Bank GDP database.
https://data.worldbank.org/indicator/NY.GDP.MKTP.CD
The Gini coefficient has been reported through different studies over time. Different surveys may employ different methods of calculating household income and the reported Gini coefficients resulting in inconsistencies in the measurement standard. Our analysis has considered all studies despite their differences in calculation and have selected the highest quality of data available for each country in any given year. The data was filtered to reduce any biases and

## ANALYSIS 
### KEY CHALLENGES
The key challenges for the dataset were:
For a country in a particular year, it was observed that there were multiple data points as different studies (sources) would have reported different Gini coefficients. Therefore, sources were ranked, and highest quality data points were kept, and the rest were not used in our analysis. To prepare the data to eliminate any biases, filters were used on various fields. When considering Gini reported, the team ensured that the surveys covered entire population and all areas of the country.
The temporal distribution of many countries is not uniform, therefore, we had to select years that had a 50 or more countries reporting data and further classified the data into five-year bins so that each bin would have at least 100 countries represented. Furthermore, missing GDP data was supplemented from the World Bank GDP database to minimize data gaps.
When studying the resource types such as net income, gross income and earnings as well as equivalence scale i.e. per capita vs equivalized distribution, the team discovered that many data points were not reported for all countries each year and there were not enough records to analyze. Therefore, the detailed analysis of income distribution has been limited to per capita net and gross income distributions.

### TREND ANALYSIS
The analysis aimed to gleaninsights on 3 aspects ofincome inequality.
![image](https://user-images.githubusercontent.com/73985225/114605962-488c4580-9cb8-11eb-85e5-af5904040e60.png)

**Income  of  top 10%  with  bottom 40% ofpopulation  in  various  nations  across  the  world**
This analysis compared net income of top 10% income earners vs bottom 40% income earners. All regions had unbalanced distributions of income with the bottom 40% receiving close to 5% at some points. However, the income trend especially after 2013 is that income distribution for the top 10% is decreasing except for North America where the top 10% population is increasing their income and the bottom 40% is decreasing.

![image](https://user-images.githubusercontent.com/73985225/114606315-c2243380-9cb8-11eb-9a4a-eef8df4b09bf.png) ![image](https://user-images.githubusercontent.com/73985225/114606594-162f1800-9cb9-11eb-8843-2bb2e0f24862.png)

**Global wealth distribution over time and its correlation with income inequality**
Global wealth distribution analysis overtime includes grouping data in 5-year bins and taking the median of the Gini coefficient and GDP. Regionally, the Gini is improving as the economy grows. However, North America showed a worsening Gini, indicating increasing income disparity with economic growth. Other regions are exhibit strong and weak correlation of Gini improving (reduced income disparity) with the GDP growth

![image](https://user-images.githubusercontent.com/73985225/114606663-2cd56f00-9cb9-11eb-9486-d67d72dcf740.png)

**Income inequality by geographical region**
The analysis compared sub regions within each region to get an overview of the variation of income inequality within each region by taking a median of the past decade. The sub regions within African regions showed the largest variation of income inequality in comparison to each other.

### CONCLUSION
Income of top 10% with bottom 40% population in various nations across the world
• In Asia and Europe, Income distribution gap between the Top 10% vs Bottom 40% is closing. However, America, Africa and Oceania region income inequality has become more obvious and is increasing.
Global wealth distribution over time and its correlation with income inequality
• The income distribution is improving in many regions of the world with increasing wealth. However, North America region is further worsening despite a significant economic growth
Income inequality by geographical region
• African subregions are showing the largest range of income inequality when compared to each other while subregions Europe and Oceania are showing the smallest ranges of income inequality.

### DATA FILES 

1. WIID_19Dec2018.xlsx: Orginal WIID data file

2. revised_new_wiid.csv: filtered WIID data file shared among the team for ease of use

3. "GDP Data.xlsx" : GDP data gathered from the world bank resource

4. "Melted GDP Data.csv": external gdp data merged with the countries from #2 above; used only in use case#2.

5. wiid2.csv: the datafile used by one of the teams to perform geographic disparity analysis

### Python Notebooks 

6. DS1_G19_data_filters.ipynb : the python notebook used to filter WIID data and creating the filtered dataset.

7. G19_Project_q1_revised.ipynb: contains use case#1 analysis; studying the top 10% and bottom 40% of population.

8. Coding on wealth distribution and income inequality.ipynb : contains the analysis conducted for use case #2

9. GeographicAnalysis.ipynb : contains comparison of various geographic regions; use case #3

10. gdp melted code.ipynb : used to clean and merge GDP data downloaded from world bank source


