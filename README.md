<p align="center">
  <img src="https://images.pexels.com/photos/3799205/pexels-photo-3799205.jpeg?auto=compress&cs=tinysrgb&w=315&h=187&dpr=1" alt="Urban Sounds">
</p>

# Urban Sounds: Musical Contrasts Between North American Cities

## Overview

This dataset represents music consumption data from a streaming platform that studied music consumption in the cities of Shelbyville and Springfield. It consists of 7 columns: `User_ID`, `Track` (song name), `Artist`, `Genre` (song genre), `Hour_of_Play` (time of play), `City` (where it was played), and `Day_of_Week` (when it was played).

## Initial Data Review and Cleaning

We started by reviewing the original dataset and identified several initial inconsistencies. There were numerous null values in the `Track`, `Artist`, and `Genre` columns, which we filled with "Unknown". Format issues in both columns and records were also corrected. Implicit duplicates in the `Genre` column, where genres were written differently but meant the same, were standardized. We also removed duplicate records where the same user listened to the same song at the same time, as this was logically inconsistent.

## In-Depth Analysis

We conducted a detailed analysis of the dataset focusing on top users, most played songs, artists, and genres. We found that 69.78% of the records were from Springfield, leading us to analyze percentages rather than absolute values. Upon examining consumption times and days, we discovered biases in the data: consumption hours were limited to 9 hours a day with zero activity outside these hours, which is illogical. Similarly, records only covered Mondays, Wednesdays, and Fridays, without clarity on whether they spanned multiple weeks or were isolated occurrences.

## Conclusion

Despite the biases and issues identified in the dataset, this project is valuable as it highlights and addresses dataset errors. Once corrected, future updates to the database will yield useful insights. The project showcases strong skills in Pandas data manipulation and matplotlib visualization, chosen for its efficiency in handling lightweight data objects.

It's important to note that due to insufficient numerical information, deeper analysis or machine learning tasks couldn't be fully explored in this project. Nevertheless, the project concludes satisfactorily given the available data.
