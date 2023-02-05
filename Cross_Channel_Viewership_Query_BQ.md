
# Cross_Channel_Viewership_Query_BQ

This is simple a starter query to get you started with your data pull in Gogle BigQuery. Feel free to modify as needed!


## Usage/Examples

```javascript
SELECT
   fullVisitorId AS fullVisitorId,
   -- trafficMedium,
   -- device,
   channelGrouping,
   SUM(pageviews) AS pageviews


 FROM (
   SELECT
     fullVisitorId,
     trafficSource.medium AS trafficMedium,
     -- device,
     channelGrouping,
     totals.pageviews AS pageviews


   FROM
     `bigquery-public-data.google_analytics_sample.ga_sessions_*` AS SESS
      WHERE _TABLE_SUFFIX BETWEEN '20170101' AND '20170831')
      
 GROUP BY 1,2
 HAVING (pageviews >0 )
 ORDER BY fullVisitorId DESC;
}
```



