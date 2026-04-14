

# Ad


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**name** | **String** |  |  [optional] |
|**platform** | [**PlatformEnum**](#PlatformEnum) |  |  [optional] |
|**status** | **AdStatus** |  |  [optional] |
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
|**platformObjective** | **String** | Raw Meta campaign objective (e.g. OUTCOME_SALES, OUTCOME_LEADS, OUTCOME_TRAFFIC). Only present for Meta ads. |  [optional] |
|**optimizationGoal** | **String** | Meta ad set optimization goal (e.g. OFFSITE_CONVERSIONS, VALUE, LEAD_GENERATION, LINK_CLICKS). Only present for Meta ads. |  [optional] |
|**bidStrategy** | **String** | Bid strategy (e.g. LOWEST_COST_WITHOUT_CAP, COST_CAP, LOWEST_COST_WITH_MIN_ROAS). Ad set level overrides campaign level. Only present for Meta ads. |  [optional] |
|**promotedObject** | [**AdPromotedObject**](AdPromotedObject.md) |  |  [optional] |
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



