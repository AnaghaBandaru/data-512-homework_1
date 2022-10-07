#Professionalism & Reproducibility

##Goal

The goal of this assignment is to construct, analyze, and publish a dataset of monthly article traffic for a select subset of dinosaur related pages from English Wikipedia from July 1, 2015 through September 30, 2022. The main aim is to follow the best practices for open documentation and reproducibility of the work.

##Data Source
The Pageviews API provides access to desktop, mobile web, and mobile app traffic data from July 2015 through the previous complete month. This API is developed and maintained by the Wikipedia Foundation.

Link to the API documentation : https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews 
Link to the API endpoint : https://wikimedia.org/api/rest_v1/#/Pageviews_data/get_metrics_pageviews_aggregate_project_access_agent_granularity_start_end

##Project Structure

data-512-homework_1
├── data
│   ├── dinosaur_genera.cleaned.SEPT.2022.csv
│   ├── dino_monthly_desktop_201501-202209.json
│   ├── dino_monthly_mobile_201501-202209.json
│   └── dino_monthly_cumulative_201501-202209.json
├── results
│   ├── maximum_minimum_average.png
│   ├── top_ten_peaks.png
│   └── fewest_months.png
├── source
│   ├── data_acquisition.ipynb
│   └── data analysis.ipynb
├── LICENSE
└── README.md