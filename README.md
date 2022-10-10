# data-512-homework_1
Documentation for Week 1 Homework assignment in DATA 512 Fall 2022 course

## Project Goal
The goal of this assignment is to construct, analyze, and publish a dataset of monthly article traffic for a select set of pages from English Wikipedia from January 1, 2015 through September 30, 2022. The purpose of the assignment is to develop and follow best practices for open scientific research.

## Data Source
In order to measure article traffic from 2015-2022, data has been collected from the Pageviews API. The Pageviews API (documentation, endpoint) provides access to desktop, mobile web, and mobile app traffic data from July 2015 through the previous complete month in machine-readable formats.

Source Links:
1. https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews (documentation) 
2. https://wikimedia.org/api/rest_v1/ (endpoint)

## Project Structure

```bash
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
```

## Dataset Description

data :
1. Raw Data -> dinosaur.csv : A CSV file containing the list of Dinosaur names and the corresponding articles url link from Wikipedia.
   Link: https://docs.google.com/spreadsheets/d/1zfBNKsuWOFVFTOGK8qnTr2DmHkYK4mAACBKk1sHLt_k/edit

Below datasets are generated from source code in jupyter notebook for analysis.
2. Intermediate Data -> all_access_data.json : An intermediary data file that contains all access data from 2015-07 to 2022-09 before calculating the cumulative sum of page traffic.

3. Output Data ->
    a. dino_monthly_desktop_201507-202209.json : Generated from the jupyter notebook, it constitutes monthly data for desktop access type.
    b. dino_monthly_mobile_201507-202209.json : Generated from the jupyter notebook, it constitutes monthly data for mobile-app and mobile-web access type.
    c. dino_monthly_cumulative_201507-202209.json : Generated from the jupyter notebook, it constitutes monthly data of all the access types with a cumulative sum of the page traffic.

output :
1. maximum_minimum_average.png : Time series graph for the dinosaur articles that have the highest average page requests and the lowest average page requests for desktop and mobile access type.
2. top_ten_peak_page_views.png : Time series graph for the top 10 dinosaur articles by peak page views for the given time period by access type.
3. fewest_month_views.png : Time series graph to show dinosaur articles that have the fewest months of page traffic data.
source:

code:
wikipedia_article_traffic_analysis.ipnyb : The jupyter notebook illustrating the entire source code and description of the analysis in step-by-step process. Starting from data acquisition using Pageviews API to cleaning the data and finally performing the needed analysis to generate the graphical plots.
