# **The effect of energy consumption on non-communicable disease mortality and life expectancy in nations with the highest renewable energy consumption growth from 2000 to 2015** 

*Daniel Brilliant*

*Data Science Master's Student, UMBC*

*March 11, 2022*

Human civilization is defined by decisions that produce beneficial and harmful outcomes. One of the most major impacts for humanity that falls into both categories is industrialization. Industrialization has made processes such as manufacturing and transportation much easier than before, but that does not come without a cost. The modified processes produced during the industrial revolution are often fueled by non-renewable resources such as coal, oil, and natural gas, also known as fossil fuels. The aftereffects have caused changes to air quality, water purity, and the ozone layer due to increases in the emission of carbon dioxide (CO<sub>2</sub>).

The effect of CO<sub>2</sub> emissions also showed a direct impact on quality of life, whether this be through breathing in polluted air, prolonged exposure to carcinogens, and access to drinkable water sources. The direct results of these environmental changes can be measured in a variety of statistics, but two that have clear implications on human life are mortality rates from diseases and life expectancies. There are two major questions we can ask about these relationships:
  1. How do CO<sub>2</sub> emissions relate to both mortality rates from disease and life expectancy at birth? 
  2. Does an increase in renewable energy usage cause positive changes to mortality rates from disease and life expectancy? 

These can be answered by analyzing the ten countries with the highest renewable energy consumption percent growth rates between the years 2000 and 2015.

## **1. Analysis Strategy and Approach**

- **Data Source:** World Development Explorer ([worlddev.xyz](https://))
- **Countries Analyzed:** Comoros, Denmark, Finland, Hungary, Iceland, Moldova, North Korea (referred to here as Democratic People's Republic of Korea), Sweden, Uruguay, and Zimbabwe
- **Timespan of Data:** 2000-2015
- **Topics & Indicators:**
  - **Environment- Renewable energy consumption (% of total final energy consumption):** the share of renewable energy in the total final energy consumption.
  - **Environment- CO<sub>2</sub> emissions (kt):** emissions of carbon dioxide stemming from the burning of fossil fuels and the manufacture of cement. These can include CO<sub>2</sub> produced during consumption of solid, liquid, and gas fuels and gas flaring.
  - **Health- Cause of death, by non-communicable diseases (% of total):** Cause of death is the share of all deaths at all ages due to underlying causes. Non-communicable diseases include cancer, diabetes mellitus, cardiovascular diseases, digestive diseases, skin diseases, musculoskeletal diseases, and congenital anomalies.
  - **Health- Cause of death, by communicable diseases and maternal, prenatal and nutrition conditions (% of total):** Cause of death is the share of all deaths at all ages due to underlying causes. Communicable diseases and maternal, prenatal, and nutrition conditions include infectious and parasitis diseases, respiratory infections, and nutritional deficiencies such as underweight and stunting.
  - **Health- Life expectancy at birth, total (years):** The number of years a newborn infant would live if prevailing mortality patterns at time of birth remain the same throughout life.

## **2. How do CO<sub>2</sub> emissions relate to life expectancy and mortality rates from communicable and non-communicable disease?**

### **CO<sub>2</sub> emission time series**

![](https://github.com/DanB1421/world_development_explorer/blob/2c1966066c7734a0b627bd1c23da6fe573c6a4d7/charts/CO2%20emissions%20time%20series.png)

### **Non-communicable disease mortality time series**
![](https://github.com/DanB1421/world_development_explorer/blob/2c1966066c7734a0b627bd1c23da6fe573c6a4d7/charts/Noncommunicable%20disease%20time%20series.png)

### **Communicable disease mortality time series**
![](https://github.com/DanB1421/world_development_explorer/blob/2c1966066c7734a0b627bd1c23da6fe573c6a4d7/charts/Communicable%20disease%20time%20series.png)

### **Life expectancy time series**
![](https://github.com/DanB1421/world_development_explorer/blob/2c1966066c7734a0b627bd1c23da6fe573c6a4d7/charts/Life%20Expectancy%20time%20series.png)

### **Relationship between CO<sub>2</sub> emissions, life expectancy, and non-communicable disease mortality in 2000 and 2015 (x axis = non-communicable disease mortality, y axis = life expectancy, z axis = CO<sub>2</sub> emissions)**
![](https://github.com/DanB1421/world_development_explorer/blob/2c1966066c7734a0b627bd1c23da6fe573c6a4d7/charts/2000%20noncommunicable%20disease%20scatterplot.png)
![](https://github.com/DanB1421/world_development_explorer/blob/2c1966066c7734a0b627bd1c23da6fe573c6a4d7/charts/2015%20noncommunicable%20disease%20scatterplot.png)

### **Relationship between CO<sub>2</sub> emissions, life expectancy, and communicable disease mortality in 2000 and 2015 (x axis = communicable disease mortality, y axis = life expectancy, z axis = CO<sub>2</sub> emissions)**
![](https://github.com/DanB1421/world_development_explorer/blob/2c1966066c7734a0b627bd1c23da6fe573c6a4d7/charts/2000%20communicable%20disease%20scatterplot.png)
![](https://github.com/DanB1421/world_development_explorer/blob/2c1966066c7734a0b627bd1c23da6fe573c6a4d7/charts/2015%20communicable%20disease%20scatterplot.png)

- The general trends shown in the time series were that for the majority of these countries between 2000 and 2015, CO<sub>2</sub> emissions decreased or flatlined, life expectancy increased, communicable disease mortality decreased, and non-communicable disease mortality increased. 
- Analysis of the three-dimensional scatterplots showed that North Korea, Denmark, and Uruguay had the most positive relationships between decreasing CO<sub>2</sub> emissions and life expectancy
- The three-dimensional scatterplots also showed that the general disease trends were a decrease in communicable disease mortality and an increase in non-communicable disease mortality with positive changes in life expectancy and negative changes in CO<sub>2</sub> emissions between 2000 and 2015

## **3. Does an increase in renewable energy usage cause significant changes to mortality rates from disease and life expectancy?**

### **Renewable Energy Shares in Each Country in 2000 and 2015**
![](https://github.com/DanB1421/world_development_explorer/blob/2c1966066c7734a0b627bd1c23da6fe573c6a4d7/charts/2000%20Renewable%20Energy%20bar%20graph.png)
![](https://github.com/DanB1421/world_development_explorer/blob/2c1966066c7734a0b627bd1c23da6fe573c6a4d7/charts/2015%20Renewable%20Energy%20bar%20graph.png)

### **Correlation Heatmap between Renewable Energy Usage, Life Expectancy, and Non-Communicable Disease Mortality in 2015**

Indicator IDs:
- EG.FEC.RNEW.ZS- Renewable Energy Usage
- SH.DTH.NCOM.ZS- Non-Communicable Disease Mortality
- SP.DYN.LE00.IN- Life Expectancy

![](https://github.com/DanB1421/world_development_explorer/blob/2c1966066c7734a0b627bd1c23da6fe573c6a4d7/charts/2015%20Noncommunicable%20Disease%20Heatmap.png)

### **Correlation Heatmap between Renewable Energy Usage, Life Expectancy, and Communicable Disease Mortality in 2015**

Indicator IDs:
- EG.FEC.RNEW.ZS- Renewable Energy Usage
- SH.DTH.COMM.ZS- Communicable Disease Mortality
- SP.DYN.LE00.IN- Life Expectancy

![](https://github.com/DanB1421/world_development_explorer/blob/2c1966066c7734a0b627bd1c23da6fe573c6a4d7/charts/2015%20Communicable%20Disease%20Heatmap.png)

- As shown in the bar graphs, the countries chosen each had significant increases in renewable energy usage between 2000 and 2015
- The correlation heatmaps showed that there was a moderate to  strong negative correlation betwen noncommunicable disease mortality and renewable energy usage, and the opposite was true for communicable disease mortality rates.
- Both heatmaps showed insignificant negative correlation between renewable energy usage and life expectancy, which shows that life expectancy is less significantly related to renewable energy usage than non-communicable and communicable disease mortalities.

## 4. **Conclusions**

This data on its own does not tell a complete story of how CO<sub>2</sub> emissions and renewable energy are a factor in disease mortality and life expectancy. However, there are a few preliminary conclusions that can be made from the analyzed data trends.

- The relationship between CO<sub>2</sub> emissions, life expectancy, and disease mortality rates over time showed that with a negative trend in CO<sub>2</sub> emissions comes an increase in life expectancy and non-communicable disease mortality and a decrease in communicable disease mortality
- The relationship between renewable energy usage and disease mortality is more significant than the relationship between renewable energy usage and life expectancy. Communicable disease mortality appeared to have positive correlation with renewable energy usage, and the opposite was true for non-communicable disease mortality.

Interestingly, the results of both comparisons show divergent results. Decreases in CO<sub>2</sub> emissions should result in the same trends for disease as an increase in renewable energy usage when it comes to disease and life expectancy, but the disease trends are opposed and the life expectancy trends are insignificant. This shows a necessity to investigate environmental factors and human health in a more detailed fashion, with more indicators present to show a stronger significance in the relationship.
