

# AdTreeCampaign

Campaign with nested ad sets and rolled-up metrics

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**platformCampaignId** | **String** |  |  [optional] |
|**platform** | [**PlatformEnum**](#PlatformEnum) |  |  [optional] |
|**campaignName** | **String** |  |  [optional] |
|**status** | **AdStatus** | Derived from child ad statuses |  [optional] |
|**adCount** | **Integer** | Total ads across all ad sets |  [optional] |
|**adSetCount** | **Integer** |  |  [optional] |
|**budget** | [**AdBudget**](AdBudget.md) |  |  [optional] |
|**metrics** | [**AdMetrics**](AdMetrics.md) |  |  [optional] |
|**platformAdAccountId** | **String** |  |  [optional] |
|**accountId** | **String** |  |  [optional] |
|**profileId** | **String** |  |  [optional] |
|**platformObjective** | **String** | Raw Meta campaign objective (e.g. OUTCOME_SALES, OUTCOME_LEADS, OUTCOME_TRAFFIC) |  [optional] |
|**optimizationGoal** | **String** | Meta optimization goal shared across ad sets, or comma-separated values when ad sets differ (e.g. OFFSITE_CONVERSIONS, VALUE, LEAD_GENERATION) |  [optional] |
|**bidStrategy** | **String** | Campaign-level bid strategy (e.g. LOWEST_COST_WITHOUT_CAP, COST_CAP, LOWEST_COST_WITH_MIN_ROAS) |  [optional] |
|**promotedObject** | [**AdTreeCampaignPromotedObject**](AdTreeCampaignPromotedObject.md) |  |  [optional] |
|**adSets** | [**List&lt;AdTreeAdSet&gt;**](AdTreeAdSet.md) |  |  [optional] |



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



