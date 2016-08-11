Problem 3
===
Create a page to display list of colleges.

#### Step 1
Create a rake task to scrape top colleges data from [US News college page](http://colleges.usnews.rankingsandreviews.com/best-colleges/rankings/national-universities/data) (all pages)

The scraped data needs to stored in a json file in this structure

```
[
  {
    "name" : "Example college/school name",
    "rank" : 1,
    "tuition_fees" : "$5000",
    "total_enrollment" : 50000,
    "acceptance_rate" : "50%",
    "average_retention_rates" : "98%",
    "graduation_rate" : "98%"
  }
]
```
#### Step 2
Once you have the json file, create a html page to display the data in a tablular format with paging (10 records per page)
