# Statistic-and-visualize-COVID-19-data
Statistics and visualize COVID19 data from Worldometer (www.worldometers.info)
## Requirement:
From about the end of 2019 until now, a pandemic has spread terribly around the world.
Every day thousands of people are infected and tens to hundreds of people die. Organization
Worldometer (www.worldometers.info) has collected statistical data from many sources and from many countries
daily reports to aggregate into a table in Figure 1. In the website, the organization
Worldmeter also makes graphs to show the visual change of the epidemic situation
sick. However, we do not use it.

![Figure1](https://user-images.githubusercontent.com/62047983/162554742-2f4a700c-5beb-45d7-849f-7db1bb415e3d.png)

You are mandated by the country to understand this data as between data fields that are related.
What is the relationship, is there any inconstant in the data as the country report differs from the data
synthesis, anomalies in data jumping, .... Apply knowledge of statistics and
data visualization to make sense of existing data

Specifically in this lab, you are required to perform the following tasks:
* Collect daily statistics from Worldmeter site.
  * You can choose to work on a specified date. Because the Worldometer page only shows the date
today and yesterday so you should collect as many days to be able to get better
statistics and visualization.
  * You can manually copy the data and store it in standard .CSV format or use
use code to crawl data (recommended)
  * You can preprocess the data before moving on to the next phase but need to report
Report this issue in the `Data Preprocessing section`. Original data and adjusted data
should be saved and included with the submission.
* Use comments, code/algorithms to show statistics, visually the relationships between
data fields
  * Statistics about data need to be described the meaning, what has been derived from it.
  * Discuss and select data fields for visual representation with different types of graphs
have learned before.
  * The selection of the chart should be explained why it is suitable with the data field properties. May
use more than 1 chart type for the data field but need to explain why.
  * The representation of the relationship must be gradually integrated i.e. from simple to complex, from
a single field to the relationship between many fields, …
  * In addition to independence realtionship, it is necessary to consider whether there is a cause-and-effect relationship in the data.
  *  For example, can there be a relationship between the increased infection rate and the number of cases?
dead, … Need to prove through data visualizations.
  * The minimum number of visual charts is 6 charts. Note this is the minimum number and hit
price may just stop at 60%
## Approach: 
Full report: <a href="https://github.com/Phbhan/Statistic-and-visualize-COVID-19-data/blob/main/Report.pdf">Link</a>

### Crawl data: <a href="https://github.com/Phbhan/Statistic-and-visualize-COVID-19-data/blob/main/Crawl_data.ipynb">Crawl_data.ipynb</a>
Using Selenium and BeutifulSoup to crawl data from https://www.worldometers.info/coronavirus/ in 8 days and save to `csv` file.
The properties include: `Country/Other`, `Total cases`, `New cases`, `Total deaths`, `New deaths`, `Total recovered`, `New recovered`, 
`Active cases`, `Serious, Critical`, `Tot Cases/1M pop`, `Deaths/1M pop`, `Total tests`, `Test/1M pop`, `Population`, `Continent`.
### Statistics and Visualization: <a href="https://github.com/Phbhan/Statistic-and-visualize-COVID-19-data/blob/main/Ex_02.ipynb">Ex_02.ipynb</a>
Preprocessing and checking the data anomalies. After that, I did statisctics and visualization for:
1. Distribution of Tot Cases/1M pop
2. Distribution of Deaths/1M pop
3. Distribution of Test/1M pop
4. Relationship between: Total Cases – Total Test
5. Relationship between: New recovered – New deaths
6. Relationship between: Total cases – Population
7. Relationship between: Tot case/1M pop – Population
8. Relationship between: Total cases/1M pop – Test/1M pop – Continent
9. Relationship between: Deaths/1M pop – Test/1M pop – Continent
10. Mortality rate by Continent
11. Number of Cases, Deaths, Recovered by continent
12. Number of New Cases, Deaths, Recovered by continent
13. Case by Continent

