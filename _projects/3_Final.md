---
name: Final Project "Electric Range"
tools: [Python, HTML, vega-lite, Altair]
image: assets/pngs/visualization3.png
description: This is a project that aim to showcase different electric range that a certain car brand model's has! Created By Arthur Darma
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Electric Range



## Visualization

<vegachart schema-url="{{ site.baseurl }}/assets/json/hbar.json" style="width: 100%"></vegachart>

<vegachart schema-url="{{ site.baseurl }}/assets/json/line.json" style="width: 100%"></vegachart>
<vegachart schema-url="{{ site.baseurl }}/assets/json/bar.json" style="width: 100%"></vegachart>

### Visualization 2 Description:
The dashboard visualization serves as the central focus of this analysis, exploring the relationship between electric vehicle makes and their associated models' electric ranges. By isolating the top 10 electric vehicle makes, the driver plot breaks down the distribution of vehicle types into plug-in hybrid electric vehicles (PHEV) and battery electric vehicles (BEV). This allows viewers to see the relative popularity of each type for a specific make. Upon interacting with the driver plot, the driven plot dynamically updates to show the mean electric range of models associated with the selected make. This interactivity highlights the diversity in electric ranges among different models, offering insights into how manufacturers cater to various consumer needs.

The first contextual visualization, "Total Number of Electric Vehicles Per Year (Up to 2023)," provides a historical perspective on the growth of electric vehicles (EVs) over time. This line chart illustrates a significant upward trend in EV adoption, reflecting the increasing consumer shift towards sustainable transportation. By understanding this trend, viewers can contextualize the popularity of specific makes and models in the dashboard, linking the rise in EV ownership to the broader industry growth captured in the historical data.

The second contextual visualization, "Average Percent Electric Vehicles Per Year (Up to 2023)," complements the historical growth data by focusing on the proportion of electric vehicles within the overall vehicle market. This bar chart demonstrates fluctuations in the percentage of EVs, offering insights into the pace of market penetration relative to traditional vehicles. By comparing this with the central dashboard, one can infer how the market share of EVs affects the variety and electric range of models produced by top manufacturers.


<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://catalog.data.gov/dataset/electric-vehicle-population-data/resource/fa51be35-691f-45d2-9f3e-535877965e69" text="The First Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://catalog.data.gov/dataset/electric-vehicle-population-size-history-by-county" text="The Second Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/arthurdt115/arthurdt115.github.io/blob/main/python_notebooks/Workbook_Final_Project.ipynb" text="The Analysis" %}
</div>

