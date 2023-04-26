---
name: Crime Analysis on Los Angeles City
tools: [Python, HTML, Vega-lite, Altair]
image: assets/pngs/la.png
description: Using Python, Vega-lite and Altair to analyze and draw plots
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# Introduction

Today, we'll be working through some more complex examples that use Python for data analysis and transformation, and vega-lite as the output engine to save to our Jekyll pages.

# 1. Data transformations with the buildings dataset

We firstly chose features ‘Year Constructed’ and ‘Square Footage‘ to show the relationship between the area and the constructed year:

<vegachart schema-url="{{ site.baseurl }}/assets/json/dash.json" style="width: 100%"></vegachart>


# 2. More complex Data Transforms with the buildings dataset

We draw a graph to show the relationship between Average Square Footage and Year Constructed and then linked to the Building Status Data which has a interactivity that you can get the building classification as time past:

<vegachart schema-url="{{ site.baseurl }}/assets/json/building_inventory_1.json" style="width: 100%"></vegachart>

# 3. More complex Data Transforms with the buildings dataset

We draw a graph to show the relationship between Average Square Footage and Year Constructed and then linked to the Building Status Data which has a interactivity that you can get the building classification as time past:

<vegachart schema-url="{{ site.baseurl }}/assets/json/building_inventory_1.json" style="width: 100%"></vegachart>

<div class="left">
{% include elements/button.html link="https://github.com/YMA98/YMA98.github.io/blob/main/_data/la_crime_2023.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

