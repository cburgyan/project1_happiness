
# Project 1: Great Places To Visit And Invest
### A Data Analysis of Great Places To Visit And Invest

#### By Karoly Burgyan, Shayla Badeaux, Christian Cantu
 This project investigates which countries would be good for investment from the perspective of a United States based real estate company or travel agency that is ready to go international in their investments. The project asks the 5 following questions: 

 
### Research Questions to Answer:
1. Is there a correlation between Happiness and Safety?<br>
2. Is there a correlation between Happiness and Cost of Living?<br>
3. Is there a correlation between Happiness and Purchasing Power?<br>
4. Which countries satisfy the priorities of the customer best-- does the customer value happiness, purchasing power, or safety most?<br>
5. Which countries on the priority lists have the most developed infrastructure using GDP as a proxy for infrastructure development?<br>


#### Collaborators:<br>
Karoly Burgyan<br>
Shayla Badeaux<br>
Christian Cantu


#### Sources:
1. World Happiness Report up to 2022. (2022, March 19). Kaggle. https://www.kaggle.com/datasets/mathurinache/world-happiness-report
2. Cost of Living Index 2022. (2022, May 28). Kaggle. https://www.kaggle.com/datasets/ankanhore545/cost-of-living-index-2022
3.  World capitals gps. (2018). Kaggle. https://www.kaggle.com/datasets/nikitagrec/world-capitals-gps
4. World Crime Index. (2022, November 8). Kaggle. https://www.kaggle.com/datasets/ahmadjalalmasood123/world-crime-index
5. AI Global Index. (2023, April 26). Kaggle. https://www.kaggle.com/datasets/katerynameleshenko/ai-index
6. Stack Overflow - Where Developers Learn, Share, & Build Careers. (n.d.). Stack Overflow. https://stackoverflow.com/
7. https://chat.openai.com/: used to help debug problematic code




### Summary

To answer these five questions, 5 datasets on 1) happiness, 2) cost of living (which included purchasing power), 3) crime (safety), 4)city and country latitudes and longitudes, and 5) gross domestic product were combined to reach the conclusions that there are 17 excellent country choices for investment: Australia, Austria, Bahrain, Canada, Denmark, Estonia, Finland, Germany, Israel, Japan, Netherlands, New Zealand, Suadi Arabia, Singapore, Slovenia, Sweden, and United Arab Emirates. And of these, the top 5 are Saudi Arabia, Israel, Slovenia, United Arab Emirates, and Austria.

#### Gathering, Exploring, and Analyzing the Data
1. Datasets for happiness, cost of living (which included purchasing power), and crime (safety) were merged together producing one large merged dataset.<br>
2. The safety index across each country was stated by city and so, to get a rough estimation of the country-wide safety index, the safety index across all the cities in a country were combined into an averaged for the country.
3. The statistical outliers of the merged dataset for the values of happiness, cost of living, purchasing power, and safety were presumed to be errors in measurement and were removed from the dataset.<br>
4. Correlations between happiness and safety, happiness and cost of living, and happiness and purchasing power were calculated using linear regressions. These correlations were 0.35, 0.74, and 0.74 respectively.<br>
5. Because purchasing power had the same correlation to happiness as cost of living and it has more salience in terms of investing from the perspective of real estate companies and travel agencies, the cost of living was determined to be less useful and perhaps redundant in the presence of purchasing power.<br>
6. Z-scores were calculated for the happiness, safety, and purchasing power to assess whether the values varied sufficiently to assess the importance of each metric. If the z-scores were small (e.g. less than 1 standard deviation) for a metric, then it could be assumed that the metric was less relevant in comparison to the other two metrics.<br>
7. 3D plots were created to visualize the z-scores and assess their variability. It turned out that all three metrics varied well beyond 1 standard deviation and, thereby, suggesting that each metric represented a tangible difference across the countries that shouldn't be discarded.<br>
8. From the 3 metrics happiness, safety, and purchasing power, the following 7 different prioritization combinations were considered and a histogram for each prioritization was created:<br>
&emsp;&emsp;i. Equally weighted happiness, safety, and purchasing power<br>
&emsp;&emsp;ii. Prioritized happiness, safety, then purchasing power<br>
&emsp;&emsp;iii. Prioritized happiness, purchasing power, then safety<br>
&emsp;&emsp;iv. Prioritized safety, happiness, then purchasing power<br>
&emsp;&emsp;v. Prioritized safety, purchasing power, then happiness<br>
&emsp;&emsp;vi. Prioritized purchasing power, safety, then happiness<br>
&emsp;&emsp;vii. Prioritized purchasing power, happiness, then safety<br>

9. From those 7 prioritizations, a total of 17 unique countries were collected.<br>
10. A new dataset of Gross Domestic Product by country by year was introduced as a proxy for a comparison of growth of infrastructure among the 17 unique countries.<br>
11. A line plot showing the last 5 years of the top 17 countries revealed that the top 5 growing countries were Saudi Arabia, Israel, Slovenia, United Arab Emirates, and Austria.<br>

### Conclusion
1. Is there a correlation between Happiness and Safety?<br>
Yes, there is a positive correlation between happiness and safety with a Person's R coefficient of 0.35.

2. Is there a correlation between Happiness and Cost of Living?<br>
Yes, there is a positive correlation between happiness and safety with a Person's R coefficient of 0.74.

3. Is there a correlation between Happiness and Purchasing Power?<br>
Yes, there is a positive correlation between happiness and purchasing power with a Person's R coefficient of 0.74.<br>

4. Which countries satisfy the priorities of the customer best-- does the customer value happiness, purchasing power, or safety most?
The answer to this depends on the priorities of the customer that's being served. For :<br>

&emsp;&emsp;i. Equally weighted happiness, safety, and purchasing power: the top 10 countries of interest would be Switzerland, Denmark, Finland, United Arab Emirates, Iceland, Netherlands, Germany, Norway, Austria, Australia.<br>
&emsp;&emsp;ii. Prioritized happiness, safety, then purchasing power: the top 10 countries of interest would be Switzerland, Finland, Denmark, Iceland, Netherlands, Norway, Israel, Austria, United Arab Emirates, Sweden.<br>
&emsp;&emsp;iii. Prioritized happiness, purchasing power, then safety: the top 10 countries of interest would be Switzerland, Finland, Denmark, Sweden, Iceland, Netherlands, Australia, Norway, Germany, Israel.<br>
&emsp;&emsp;iv. Prioritized safety, happiness, then purchasing power: the top 10 countries of interest would be Switzerland, United Arab Emirates, Denmark, Iceland, Finland, Bahrain, Netherlands, Slovenia, Austria, Estonia.<br>
&emsp;&emsp;v. Prioritized safety, purchasing power, then happiness: the top 10 countries of interest would be Switzerland, United Arab Emirates, Denmark, Iceland, Finland, Netherlands, Bahrain, Singapore, Slovenia, Estonia.<br>
&emsp;&emsp;vi. Prioritized purchasing power, safety, then happiness: the top 10 countries of interest would be Switzerland, Denmark, United Arab Emirates, Germany, Australia, Finland, Singapore, Saudi Arabia, Netherlands, Sweden.<br>
&emsp;&emsp;vii. Prioritized purchasing power, happiness, then safety: the top 10 countries of interest would be Switzerland, Denmark, Australia, Germany, Finland, Sweden, Netherlands, United Arab Emirates, Saudi Arabia, Norway.<br>

5. Which countries on the priority lists have the most developed infrastructure using GDP as a proxy for infrastructure development?
Of the top 17 countries discovered in the priority lists above, the top 5 in GDP and thereby presumably infrastructure are Saudi Arabia, Israel, Slovenia, United Arab Emirates, and Austria.<br>

#### The Next Steps
The investment advice to for a real estate company drawn from the results above that's about to go international is to investigate further into the countries listed above in following manner:<br>
investigate the population trends of the country's cities, the real estate trends already present in the cities (for competitive awareness), industry and manufacturing capabilities, cultural and technical institutes and industries. 

The investment advice to for a travel agency drawn from the results above that's about to go international is to investigate further into the countries listed above in following manner:<br>
exchange rates, tourist attractions, civilian attractions (hotels, restaurants, parks, bars, hospitals), and flight costs.
