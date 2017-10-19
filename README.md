# Assignment #1, DATA-512-A1, Gary Gregg, University of Washington, Autumn 2017

Goal: The goal of this project is to construct, analyze, and publish a dataset of monthly traffic on English language Wikipedia from January 1, 2008 through September 30, 2017.

License of the source data is provided at: https://creativecommons.org/licenses/by-sa/3.0/
Terms of use provided at: https://wikimediafoundation.org/wiki/Terms_of_Use/en

API documentation is provided at:
https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts

and:
https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews

The code produces a CSV formatted file with the following fields:
year -					Year of the measurement
month -					Month of the measurement
pagecount_all_views -			Count of all pagecount accesses
pagecount_desktop_views -		Count of pagecount accesses from desktop clients only
pagecount_mobile_views -		Count of pagecount accesses from mobile clients only
pageview_all_views -			Count of all pageview accesses
pageview_desktop_views -		Count of pageview accesses from desktop clients only
pageview_mobile_views -			Count of pageview accesses from mobile clients only

Special considerations: The pagecount API is a legacy API that does not differentiate between spiders/crawlers and user accesses.  The pageview API does make this distinction, and here we exclude spider/crawler page accesses.

