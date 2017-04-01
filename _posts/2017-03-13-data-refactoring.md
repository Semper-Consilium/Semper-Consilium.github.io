---
layout: post
title:  "Data Refactoring"
date:   2017-03-13 11:19:00 +0000
categories: interaction design
---

The pollution data was initially quite large with over 360,000 readings from multiple locations over the past year. This data was also provided in csv (comma separated value) format. Both of which meant that the data needed to be heavily re-factored for use in this project.

The first step was the write a small php script converting the data from csv into 6 xml files. These files separated the data by constituency and removed some of the redundant location data, reducing the data sets size. As the data was now in xml rather than csv a stream parser could be used to further manipulate the data into something far more usable.

Currently the data displayed readings by hour, sometimes taking multiple readings throughout the hour depending on location. As we wanted to display this data for each month we needed to consolidate the hourly readings into monthly averages.

This was done with another php script that looped through each xml file adding all the readings by month, constituency and pollution type into a multidimensional arrays. All pollution readings that had the same month, constituency  and pollution type were then added together and divided by the total number of readings for that pollution type. Providing the average pollution levels for each constituency, for each month in the past year. This php file also converted the data from an xml format to a json format which allowed us to more easily handle the data as the rest of the project was built with javascript.

In comparison there was very little refactoring needed with the housing price data. Zoopla provides a simple and usable api in both xml and json. Although the json was poorly structured in comparison to the xml version. It did not take long to adjust the data structure to suit our project.
