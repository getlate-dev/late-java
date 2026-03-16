

# AnalyticsListResponsePostsInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**latePostId** | **String** | Original Late post ID if scheduled via Late |  [optional] |
|**content** | **String** |  |  [optional] |
|**scheduledFor** | **OffsetDateTime** |  |  [optional] |
|**publishedAt** | **OffsetDateTime** |  |  [optional] |
|**status** | **String** |  |  [optional] |
|**analytics** | [**PostAnalytics**](PostAnalytics.md) |  |  [optional] |
|**platforms** | [**List&lt;PlatformAnalytics&gt;**](PlatformAnalytics.md) |  |  [optional] |
|**platform** | **String** |  |  [optional] |
|**platformPostUrl** | **URI** |  |  [optional] |
|**isExternal** | **Boolean** |  |  [optional] |
|**profileId** | **String** |  |  [optional] |
|**thumbnailUrl** | **URI** |  |  [optional] |
|**mediaType** | [**MediaTypeEnum**](#MediaTypeEnum) |  |  [optional] |
|**mediaItems** | [**List&lt;AnalyticsSinglePostResponseMediaItemsInner&gt;**](AnalyticsSinglePostResponseMediaItemsInner.md) | All media items for this post. Carousel posts contain one entry per slide. |  [optional] |



## Enum: MediaTypeEnum

| Name | Value |
|---- | -----|
| IMAGE | &quot;image&quot; |
| VIDEO | &quot;video&quot; |
| GIF | &quot;gif&quot; |
| DOCUMENT | &quot;document&quot; |
| CAROUSEL | &quot;carousel&quot; |
| TEXT | &quot;text&quot; |



