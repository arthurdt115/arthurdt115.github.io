---
name: Final Project, "Driving the Future"
tools: [Python, HTML, vega-lite, Altair]
image: assets/pngs/visualization3.png
description: This is a project that aim to explore the relationship between electric vehicle makes and their associated models' electric ranges.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Driving the Future: Trends and Insights into Electric Vehicles in Washington State
##### By: Arthur Darma

--- 
&nbsp;
### Central Interactive Visualization
###### *Click on an individual bar on the left to view the detailed mean electric range for each model of a specific make.

&nbsp;

<vegachart schema-url="{{ site.baseurl }}/assets/json/hbar.json" style="width: 100%"></vegachart>
** This visualization represents a filtered dataset of electric vehicles population data. The data has been cleaned by removing entries with missing values (NaN) and includes only the top 10 makes by vehicle count due to ensure the visualization remains clear and interpretable. Additionally, only models with an electric range greater than 0 miles are included to ensure meaningful representation of electric vehicle performance.

### Contextual Visualization
&nbsp;
<vegachart schema-url="{{ site.baseurl }}/assets/json/line.json" style="width: 100%"></vegachart>
This line chart visualizes the total number of electric vehicles per year in Washington State from 2017 to 2024. The red line represents the upward trend in electric vehicle adoption over time, with blue points marking the specific values for each year. The data shows a steady and significant growth in the total number of electric vehicles, surpassing 1.8 million by 2024. The x-axis represents the years, while the y-axis displays the total number of electric vehicles.
<vegachart schema-url="{{ site.baseurl }}/assets/json/bar.json" style="width: 100%"></vegachart>
This bar chart depicts the percentage of electric vehicles in Washington State from 2017 to 2024. The chart shows a steady increase in the adoption rate of electric vehicles over the years, with the percentage surpassing 3% of all vehicles by 2024. The x-axis represents the years, while the y-axis displays the percentage of electric vehicles as part of the total vehicle population. The consistent growth highlights a significant shift toward electric mobility within the state over the observed period.

** These carts specifically represents Washington State as of 2024 and may not align with national trends. This visualization is not intended to generalize or misrepresent the broader U.S. market conditions since The electric vehicle market in 2024 appears to be stalling.

---
&nbsp;
### Connective Information:
&nbsp;

The dashboard visualization serves as the central focus of this analysis, exploring the relationship between electric vehicle makes and their associated models' electric ranges. By isolating the top 10 electric vehicle makes, the driver plot breaks down the distribution of vehicle types into plug-in hybrid electric vehicles (PHEV) and battery electric vehicles (BEV). This allows viewers to see the relative popularity of each type for a specific make in Washington state. Upon interacting with the driver plot, the driven plot dynamically updates to show the mean electric range of models associated with the selected make. This interactivity highlights the diversity in electric ranges among different models, offering insights for viewers about which model of a certain make would fulfill various consumer needs.

The first contextual visualization, "Total Number of Electric Vehicles Per Year in Washington State" provides a historical perspective on the growth of electric vehicles (EVs) over time. This line chart illustrates a significant upward trend in EV adoption, reflecting the increasing consumer shift towards sustainable transportation. By understanding this trend, viewers can contextualize the popularity of specific makes and models in the dashboard, linking the rise in EV ownership to the car industry growth captured in the historical data.

The second contextual visualization, "Electric Vehicles Percentage Per Year in Washington State" complements the historical growth data by focusing on the proportion of electric vehicles within the overall vehicle market. This bar chart demonstrates increase in the percentage of EVs, offering insights into the pace of market penetration relative to traditional vehicles. By understanding this one could infer from the central dashboard, that if the trend continues the PHEV and traditional vehicle will gradually be a history and everything will only be BEV.


---

To view the datasets and analysis utilized in this project:

1. **Dataset for the Central Interactive Visualization**: [Electric Vehicle Population Data](https://catalog.data.gov/dataset/electric-vehicle-population-data/resource/fa51be35-691f-45d2-9f3e-535877965e69)  
2. **Dataset for Contextual Visualization**: [Electric Vehicle Population Size History by County](https://catalog.data.gov/dataset/electric-vehicle-population-size-history-by-county/resource/de0258e2-3542-4703-aad4-dcebd9d1f195)  
3. **Analysis Jupyter Notebook**: [Workbook Final Project](https://github.com/arthurdt115/arthurdt115.github.io/blob/main/python_notebooks/Workbook_Final_Project.ipynb)  

Alternatively, you can access all of these resources using the buttons below.
<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://catalog.data.gov/dataset/electric-vehicle-population-data/resource/fa51be35-691f-45d2-9f3e-535877965e69" text="The First Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://catalog.data.gov/dataset/electric-vehicle-population-size-history-by-county/resource/de0258e2-3542-4703-aad4-dcebd9d1f195" text="The Second Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/arthurdt115/arthurdt115.github.io/blob/main/python_notebooks/Workbook_Final_Project.ipynb" text="The Analysis" %}
</div>

