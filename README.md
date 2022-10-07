# Professionalism & Reproducibility

## Goal

The goal of this assignment is to construct, analyze, and publish a dataset of monthly article traffic for a select subset of dinosaur related pages from English Wikipedia from July 1, 2015 through September 30, 2022. The main aim is to follow the best practices for open documentation and reproducibility of the work.

## Data Source
The Pageviews API provides access to desktop, mobile web, and mobile app traffic data from July 2015 through the previous complete month. This API is developed and maintained by the Wikipedia Foundation.

Link to the API documentation : https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews 
Link to the API endpoint : https://wikimedia.org/api/rest_v1/#/Pageviews_data/get_metrics_pageviews_aggregate_project_access_agent_granularity_start_end

## Project Structure

```bash
data-512-homework_1
├── data
│   ├── dinosaur_genera.csv
│   ├── dino_monthly_desktop_201507-202209.json
│   ├── dino_monthly_mobile_201507-202209.json
│   └── dino_monthly_cumulative_201507-202209.json
│   └── all_access_data.json
├── output
│   ├── maximum_minimum_average.png
│   ├── top_ten_peak_page_views.png
│   └── fewest_month_views.png
├── source
│   ├── DataAcquisitionAndAnalysis.ipnyb
├── LICENSE
└── README.md
 ```

## File Descriptions

**data** : 

- *dinosaur_genera.csv* : A CSV file containing the list of Dinosaurs and the corresponding articles from Wikipedia.
- *dino_monthly_desktop_201507-202209.json* : This file is generated in the DataAcquisitionAndAnalysis.ipnyb notebook and contains monthly data for desktop access type.
- *dino_monthly_mobile_201507-202209.json* : This file is generated in the DataAcquisitionAndAnalysis.ipnyb notebook and contains monthly data for mobile-app and mobile-web access type.
- *dino_monthly_cumulative_201507-202209.json* : This file is generated in the DataAcquisitionAndAnalysis.ipnyb notebook and contains monthly data of all the access types with a cumulative sum of the page traffic.
- *all_access_data.json* : This file is generated in the DataAcquisitionAndAnalysis.ipnyb notebook and is an intermediary data file that contains all access data from 2015-07 to 2022-09 before calculating the cumulative sum of page traffic.

**output** :

- *maximum_minimum_average.png* : Time series graph for the dinosaur articles that have the highest average page requests and the lowest average page requests for desktop and mobile access type.
- *top_ten_peak_page_views.png* : Time series graph for the top 10 dinosaur articles by peak page views for the given time period by access type.
- *fewest_month_views.png* : Time series graph to show dinosaur articles that have the fewest months of page traffic data.

**source**:

- *DataAcquisitionAndAnalysis.ipnyb* : In this notebook, First the data is acquired using the pageviews API. and then the required visual analysis is done for the Dinosaur articles subset for desktop and mobile access type.
