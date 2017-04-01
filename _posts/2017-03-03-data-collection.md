---
layout: post
title:  "Data Collection"
date:   2017-03-03 10:57:00 +0000
categories: interaction design
---

Initially we aimed to use the “they work for you” api to gain access to political data, in particular information on debates and attendance. We then wanted to compare this data to changes throughout the UK to understand weather debating about any one topic in parliament could make a noticeable change in the topic debated. Through test it became apparent however, that the only way we could query the debate data was through key words. This made it difficult to accurately represent the number of debates on any one topic. Even representing the direction and outcomes of one debate could become misleading if all speakers and comments are not accounted for. Attendance was another issue in this initial idea as we quickly found out that parliament is not legally required to publish attendance, so they don’t.

This lead us to look for a new source of data. One that we hope would be equally important to the public. We had several ideas as to what data could be good to use but wanted to ask people for there opinions on which direction to take the project. Narrowed down from a small list of possible datasets, the most popular comparison choices were pollution and housing prices.

Through the bristol open data project we were able to acquire a large set of data on pollution. Sensors have been placed throughout the city and have been collecting information on three different pollution types over the past year. Climate change and pollution is one of the largest and often most controversial topic of our time. With such a large data set we felt it would be easy to accurately represent and compare pollution from across the city of bristol.

To compliment bristols pollution data we wanted to find at least a years worth of data on housing price fluctuation. Initially we looked at the national office of statistics for this information although there service was difficult to navigate and understand. This was most likely due to there large and varying amount of data from all areas of data collection in the UK. To gain a more specific set of data for just housing we looked at estate agents. Both rightmove and zoopla provided api’s though after testing both, Zoopla was far more user friendly allowing us to query both current averages and averages going back several years.
