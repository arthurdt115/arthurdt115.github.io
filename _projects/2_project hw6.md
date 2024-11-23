---
name: HW6 Project
tools: [Python, HTML, vega-lite, Altair]
image: assets/pngs/barufo.png
description: This is a "showcase" project that uses Jekyll!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Homework 6

We can use a vegachart HTML tag like so:

```
<vegachart schema-url="{{ site.baseurl }}/assets/json/Chart01.json" style="width: 100%"></vegachart>
```

## Visualization 1


<vegachart schema-url="{{ site.baseurl }}/assets/json/Chart01.json" style="width: 100%"></vegachart>

## Visualization 2
<vegachart schema-url="{{ site.baseurl }}/assets/json/Chart02.json" style="width: 100%"></vegachart>

### Visualization 1 Description:
In the first visualization, I focus on the trends of UFO sightings over the years.
 The line chart visualizes the number of sightings each year,
  with points marking individual years to highlight specific data points. 
  The x-axis represents the year, and the y-axis shows the count of sightings. 
  I used a line chart because it effectively highlights the trend over time, 
  helping viewers easily spot significant increases or decreases in sightings. 
  The color blue was chosen for visual clarity and to maintain consistency throughout the visualizations. I also added the tooltip for the interactivity so viewer can interact with each points on the plot. I did not change anything from HW5 for the chart 1.

### Visualization 2 Description:
The second visualization explores the distribution of UFO sightings by shape. 
I used a bar chart to display the frequency of various shapes lited in the dataset. 
The x-axis represents the shape of the UFO, while the y-axis shows the count of sightings for each shape. I chose to color the bars based on the shape itself to make it easier for viewers to distinguish
between the different categories. I am no longer using the logarithmic scale for chart 2, and that is only what I change from HW 5, because for some reason if I used log scale the bar won't show up.


<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/UIUC-iSchool-DataViz/is445_data/raw/main/ufo-scrubbed-geocoded-time-standardized-00.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/arthurdt115/arthurdt115.github.io/blob/main/python_notebooks/nb.ipynb" text="The Analysis" %}
</div>

