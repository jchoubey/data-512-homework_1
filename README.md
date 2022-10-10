# data-512-homework_1
Documentation for Week 1 Homework assignment in DATA 512 Fall 2022 course

## Goal
The goal of this assignment is to construct, analyze, and publish a dataset of monthly article traffic for a select set of pages from English Wikipedia from January 1, 2015 through September 30, 2022. The purpose of the assignment is to develop and follow best practices for open scientific research.

## Dataset Description
In order to measure article traffic from 2015-2022, data has been collected from the Pageviews API. The Pageviews API (documentation, endpoint) provides access to desktop, mobile web, and mobile app traffic data from July 2015 through the previous complete month in machine-readable formats.

Source Links:
1. https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews (documentation) 
2. https://wikimedia.org/api/rest_v1/ (endpoint)

## Project Structure

'''bash
data-512-homework_1
├── data
│   ├── dinosaur.csv
│   ├── dino_monthly_desktop_201507-202209.json
│   ├── dino_monthly_mobile_201507-202209.json
│   └── dino_monthly_cumulative_201507-202209.json
│   └── all_access_data.json
├── output
│   ├── maximum_minimum_average.png
│   ├── top_ten_peak_page_views.png
│   └── fewest_month_views.png
├── code
│   ├── wikipedia_article_traffic_analysis.ipnyb
├── LICENSE
└── README.md
'''
