

# Ad


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**name** | **String** |  |  [optional] |
|**platform** | [**PlatformEnum**](#PlatformEnum) |  |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) |  |  [optional] |
|**adType** | [**AdTypeEnum**](#AdTypeEnum) |  |  [optional] |
|**goal** | [**GoalEnum**](#GoalEnum) |  |  [optional] |
|**isExternal** | **Boolean** | True for ads synced from platform ad managers |  [optional] |
|**budget** | [**AdBudget**](AdBudget.md) |  |  [optional] |
|**metrics** | [**AdMetrics**](AdMetrics.md) |  |  [optional] |
|**platformAdId** | **String** |  |  [optional] |
|**platformAdAccountId** | **String** |  |  [optional] |
|**platformCampaignId** | **String** |  |  [optional] |
|**platformAdSetId** | **String** |  |  [optional] |
|**campaignName** | **String** |  |  [optional] |
|**adSetName** | **String** |  |  [optional] |
|**creative** | [**AdCreative**](AdCreative.md) |  |  [optional] |
|**targeting** | **Object** |  |  [optional] |
|**schedule** | [**AdSchedule**](AdSchedule.md) |  |  [optional] |
|**rejectionReason** | **String** |  |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  [optional] |
|**updatedAt** | **OffsetDateTime** |  |  [optional] |



## Enum: PlatformEnum

| Name | Value |
|---- | -----|
| FACEBOOK | &quot;facebook&quot; |
| INSTAGRAM | &quot;instagram&quot; |
| TIKTOK | &quot;tiktok&quot; |
| LINKEDIN | &quot;linkedin&quot; |
| PINTEREST | &quot;pinterest&quot; |
| GOOGLE | &quot;google&quot; |
| TWITTER | &quot;twitter&quot; |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| ACTIVE | &quot;active&quot; |
| PAUSED | &quot;paused&quot; |
| PENDING_REVIEW | &quot;pending_review&quot; |
| REJECTED | &quot;rejected&quot; |
| COMPLETED | &quot;completed&quot; |
| CANCELLED | &quot;cancelled&quot; |
| ERROR | &quot;error&quot; |



## Enum: AdTypeEnum

| Name | Value |
|---- | -----|
| BOOST | &quot;boost&quot; |
| STANDALONE | &quot;standalone&quot; |



## Enum: GoalEnum

| Name | Value |
|---- | -----|
| ENGAGEMENT | &quot;engagement&quot; |
| TRAFFIC | &quot;traffic&quot; |
| AWARENESS | &quot;awareness&quot; |
| VIDEO_VIEWS | &quot;video_views&quot; |



