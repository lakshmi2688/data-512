# data-512-

**********************************************
Goal of this project
**********************************************
The goal of this project is to construct, analyze, and publish a dataset of monthly traffic on English Wikipedia from January 1 2008 through August 30 2020.
We combine the data from two different API endpoints, the Legacy Pagecounts API and the Pageviews API and perform analysis of the combined data by plotting a time series plot.

***********************************************
License of the source data
***********************************************
Unless otherwise specified in the endpoint documentation below, content accessed via the 2 APIS is licensed under the CC-BY-SA 3.0 and GFDL licenses, and you irrevocably agree to release modifications or additions made through this API under these licenses. More details are available in the link to the Wikimedia Foundation REST API terms of use: https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions (Links to an external site)

**********************************************
Link to all relevant API documentation:
**********************************************
In order to measure Wikipedia traffic from 2008-2020, you will need to collect data from two different API endpoints, the Legacy Pagecounts API and the Pageviews API.

1)The Legacy Pagecounts API (documentation and endpoint links below) provides access to desktop and mobile traffic data from December 2007 through July 2016. https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts https://wikimedia.org/api/rest_v1/#/Pagecounts_data_(legacy)/get_metrics_legacy_pagecounts_aggregate_project_access_site_granularity_start_end

2)The Pageviews API (documentation and endpoint links below) provides access to desktop, mobile web, and mobile app traffic data from July 2015 through last month. 
https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews https://wikimedia.org/api/rest_v1/#/Pageviews_data/get_metrics_pageviews_aggregate_project_access_agent_granularity_start_end

*******************************************************************************
Description of fields in the data file en-wikipedia_traffic_200712-202008.csv
*******************************************************************************
year	  - year in the format YYYY 
month	  - month in the format MM
pagecount_all_views	- number of views from pagecount API that has combined traffic from mobile and desktop 
pagecount_desktop_views	- number of views from pagecount API that has combined traffic from desktop only
pagecount_mobile_views	- number of views from pagecount API that has combined traffic from mobile only 
pageview_all_views	- number of views from pageview API that has combined traffic from mobile and desktop 
pageview_desktop_views - number of views from pageview API that has combined traffic from desktop only
pageview_mobile_views - number of views from pageview API that has combined traffic from mobile only 

***************************
Known issues/considerations
***************************
Data from the Pageview API excludes spiders/crawlers, while data from the Pagecounts API does not.

