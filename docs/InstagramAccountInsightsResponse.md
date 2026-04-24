

# InstagramAccountInsightsResponse

Shared account-insights response envelope used by every platform-level analytics endpoint (/v1/analytics/{facebook|instagram|youtube|linkedin|tiktok}/_*). The name is historical - the shape was first shipped for Instagram and every new platform endpoint reuses it for response-shape consistency. The platform field echoes back which platform served the response. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**success** | **Boolean** |  |  [optional] |
|**accountId** | **String** | The Zernio SocialAccount ID |  [optional] |
|**platform** | [**PlatformEnum**](#PlatformEnum) | Platform that served this response. |  [optional] |
|**dateRange** | [**InstagramAccountInsightsResponseDateRange**](InstagramAccountInsightsResponseDateRange.md) |  |  [optional] |
|**metricType** | [**MetricTypeEnum**](#MetricTypeEnum) |  |  [optional] |
|**breakdown** | **String** | Breakdown dimension used (only present when breakdown was requested) |  [optional] |
|**metrics** | [**Map&lt;String, InstagramAccountInsightsResponseMetricsValue&gt;**](InstagramAccountInsightsResponseMetricsValue.md) | Object keyed by metric name. For time_series: each metric has \&quot;total\&quot; (number) and \&quot;values\&quot; (array of {date, value}). For total_value: each metric has \&quot;total\&quot; (number) and optionally \&quot;breakdowns\&quot; (array of {dimension, value}).  |  [optional] |
|**dataDelay** | **String** |  |  [optional] |



## Enum: PlatformEnum

| Name | Value |
|---- | -----|
| FACEBOOK | &quot;facebook&quot; |
| INSTAGRAM | &quot;instagram&quot; |
| YOUTUBE | &quot;youtube&quot; |
| LINKEDIN | &quot;linkedin&quot; |
| TIKTOK | &quot;tiktok&quot; |



## Enum: MetricTypeEnum

| Name | Value |
|---- | -----|
| TIME_SERIES | &quot;time_series&quot; |
| TOTAL_VALUE | &quot;total_value&quot; |



