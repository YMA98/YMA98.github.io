---
name: Vega-lite Plots with Python Analysis
tools: [Python, HTML, vega-lite, Altair]
image: assets/pngs/pythonanalysisvegaplot.png
description: Using Python for analysis, and vega-lite for interactive, online plotting.
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

<vegachart schema-url="{{ site.baseurl }}/assets/json/chart.json" style="width: 100%"></vegachart>


# 2. More complex Data Transforms (and mappable data) with the buildings dataset

We went through the steps to make a world map with responsive dot sizes for the number of corgis born as a function of year:

<vegachart schema-url="{{ site.baseurl }}/assets/json/corgis_dotchart_world.json" style="width: 100%"></vegachart>

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/blob/main/week11/prep_notebook_week11.ipynb" text="The Analysis" %}
</div>

