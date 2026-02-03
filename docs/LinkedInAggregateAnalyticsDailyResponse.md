

# LinkedInAggregateAnalyticsDailyResponse

Response for DAILY aggregation (time series breakdown)

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**accountId** | **String** |  |  [optional] |
|**platform** | **String** |  |  [optional] |
|**accountType** | **String** |  |  [optional] |
|**username** | **String** |  |  [optional] |
|**aggregation** | [**AggregationEnum**](#AggregationEnum) |  |  [optional] |
|**dateRange** | [**LinkedInAggregateAnalyticsTotalResponseDateRange**](LinkedInAggregateAnalyticsTotalResponseDateRange.md) |  |  [optional] |
|**analytics** | [**LinkedInAggregateAnalyticsDailyResponseAnalytics**](LinkedInAggregateAnalyticsDailyResponseAnalytics.md) |  |  [optional] |
|**skippedMetrics** | **List&lt;String&gt;** | Metrics that were skipped due to API limitations |  [optional] |
|**note** | **String** |  |  [optional] |
|**lastUpdated** | **OffsetDateTime** |  |  [optional] |



## Enum: AggregationEnum

| Name | Value |
|---- | -----|
| DAILY | &quot;DAILY&quot; |



