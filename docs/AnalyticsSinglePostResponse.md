

# AnalyticsSinglePostResponse


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**postId** | **String** |  |  [optional] |
|**latePostId** | **String** | Original Late post ID if scheduled via Late |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) | Overall post status. \&quot;partial\&quot; when some platforms published and others failed. |  [optional] |
|**content** | **String** |  |  [optional] |
|**scheduledFor** | **OffsetDateTime** |  |  [optional] |
|**publishedAt** | **OffsetDateTime** |  |  [optional] |
|**analytics** | [**PostAnalytics**](PostAnalytics.md) |  |  [optional] |
|**platformAnalytics** | [**List&lt;PlatformAnalytics&gt;**](PlatformAnalytics.md) |  |  [optional] |
|**platform** | **String** |  |  [optional] |
|**platformPostUrl** | **URI** |  |  [optional] |
|**isExternal** | **Boolean** |  |  [optional] |
|**syncStatus** | [**SyncStatusEnum**](#SyncStatusEnum) | Overall sync state across all platforms |  [optional] |
|**message** | **String** | Human-readable status message for pending, partial, or failed states |  [optional] |
|**thumbnailUrl** | **URI** |  |  [optional] |
|**mediaType** | [**MediaTypeEnum**](#MediaTypeEnum) |  |  [optional] |
|**mediaItems** | [**List&lt;AnalyticsSinglePostResponseMediaItemsInner&gt;**](AnalyticsSinglePostResponseMediaItemsInner.md) | All media items for this post. Carousel posts contain one entry per slide. |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| PUBLISHED | &quot;published&quot; |
| FAILED | &quot;failed&quot; |
| PARTIAL | &quot;partial&quot; |



## Enum: SyncStatusEnum

| Name | Value |
|---- | -----|
| SYNCED | &quot;synced&quot; |
| PENDING | &quot;pending&quot; |
| PARTIAL | &quot;partial&quot; |
| UNAVAILABLE | &quot;unavailable&quot; |



## Enum: MediaTypeEnum

| Name | Value |
|---- | -----|
| IMAGE | &quot;image&quot; |
| VIDEO | &quot;video&quot; |
| CAROUSEL | &quot;carousel&quot; |
| TEXT | &quot;text&quot; |



