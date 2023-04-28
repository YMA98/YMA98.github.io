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
# Exploring Crime in Los Angeles City

### Group 12: Yifan Wang, Carol Lu, Rocky Ma

## Introduction

Crime is a significant issue that affects communities worldwide, and the city of Los Angeles is no exception. According to the Los Angeles Police Department (LAPD), there were over 210,000 reported crimes in the city in 2020 alone, ranging from theft and robbery to assault and homicide. The impact of crime on communities is far-reaching, from personal trauma to economic costs, and it is crucial to understand its distribution and trends to address it effectively.

To this end, our team has undertaken a data visualization project on crime in Los Angeles City, utilizing a dataset representing the incidents of crime in the city dating back to 2020. To make the data more manageable, we narrowed our focus to the years 2023 and beyond, reducing the number of rows from 700,000 to 60,000. Through our project, we aim to provide insights into the distribution and patterns of crime in LA City, allowing for better decision-making and policy implementation.

## Dashboard

Our dashboard comprises two main components: the left section showcases a plot that displays the age, descent, and sex of victims population, while the right section presents the count of criminal records grouped by area names of the city.

The left section of the dashboard focuses on the demographics of crime victims, providing an insight into who is most vulnerable to crime with different colors representing different demographic groups. By selecting a particular area, users can view the specific number of criminal records connected to the selected victim group, and distributions in different areas. This interactivity makes it easier to compare the demographics of victims in different ages, descent, gender between different regions of the city.

<vegachart schema-url="{{ site.baseurl }}/assets/json/dash.json" style="width: 100%"></vegachart>

## Contextual Data Analysis

This dataset contains information on all shooting incidents that have taken place in New York City from 2006 until the end of the previous calendar year. The data is collected quarterly and reviewed by the Office of Management Analysis and Planning before being made available on the NYPD website. Each record in the dataset represents a specific shooting incident and includes details about when and where it occurred. It also includes information about the demographics of both the victim and the suspect. This dataset can be used by the public to gain insights into patterns and trends related to criminal activity involving firearms. 

We have two plots below. The first one is also interactive and contains two parts. The heat map shows the relationship between victims and perpetrators and categorize them in different race. When you click the square, it show the area of the incidents happening. The second one shows the number of shootings from 2006 to 2022 by areas in New York City.

<vegachart schema-url="{{ site.baseurl }}/assets/json/nyc_dash.json" style="width: 100%"></vegachart>

<vegachart schema-url="{{ site.baseurl }}/assets/json/nyc_year_chart.json" style="width: 100%"></vegachart>

## Conclusion

When people are thinking where to live, safety is usually considered to be one of the most important factors. So, we found out a way to evaluate whether a city is dangerous or not through crime data. We chose LA city data as an example to make an interactive visualization plot showing the crime situation of the city. The result showed many useful information and let us learn the importance of data visualization in real world.

## Citation
Crime Data from 2020 to Present: Los Angeles - Open Data Portal
https://data.lacity.org/Public-Safety/Crime-Data-from-2020-to-Present/2nrs-mtv8

NYPD Shooting Incident Data (Historic): NYC Open Data
https://data.cityofnewyork.us/Public-Safety/NYPD-Shooting-Incident-Data-Historic-/833y-fsy8


<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/YMA98/YMA98.github.io/main/_data/la_crime_2023.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/YMA98/YMA98.github.io/blob/main/python_notebooks/Final_Proj_part2.ipynb" text="The Analysis" %}
</div>

