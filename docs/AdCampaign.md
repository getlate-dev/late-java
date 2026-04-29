

# AdCampaign


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**platformCampaignId** | **String** |  |  [optional] |
|**platform** | [**PlatformEnum**](#PlatformEnum) |  |  [optional] |
|**campaignName** | **String** |  |  [optional] |
|**status** | **AdStatus** | Delivery status derived from child ad statuses. Distinct from &#x60;reviewStatus&#x60;. |  [optional] |
|**reviewStatus** | [**ReviewStatusEnum**](#ReviewStatusEnum) | Platform-side review state of the campaign. See AdTreeCampaign.reviewStatus for the full description. |  [optional] |
|**platformCampaignStatus** | **String** | Raw platform-level campaign status (Meta &#x60;effective_status&#x60;). |  [optional] |
|**campaignIssuesInfo** | **List&lt;Object&gt;** | Platform-reported campaign issues (Meta &#x60;issues_info[]&#x60;). |  [optional] |
|**adCount** | **Integer** |  |  [optional] |
|**budget** | [**AdCampaignBudget**](AdCampaignBudget.md) |  |  [optional] |
|**campaignBudget** | [**AdCampaignCampaignBudget**](AdCampaignCampaignBudget.md) |  |  [optional] |
|**budgetLevel** | [**BudgetLevelEnum**](#BudgetLevelEnum) | Canonical CBO/ABO indicator. See AdTreeCampaign.budgetLevel. |  [optional] |
|**isBudgetScheduleEnabled** | **Boolean** | Meta-only. Mirrors Campaign.is_budget_schedule_enabled. |  [optional] |
|**currency** | **String** | ISO 4217 currency code for all budget amounts. Budgets are NOT normalized to USD. |  [optional] |
|**metrics** | [**AdMetrics**](AdMetrics.md) |  |  [optional] |
|**platformAdAccountId** | **String** |  |  [optional] |
|**accountId** | **String** |  |  [optional] |
|**profileId** | **String** |  |  [optional] |
|**platformObjective** | **String** | Raw Meta campaign objective (e.g. OUTCOME_SALES, OUTCOME_LEADS, OUTCOME_TRAFFIC) |  [optional] |
|**optimizationGoal** | **String** | Meta optimization goal shared across ad sets, or comma-separated values when ad sets differ (e.g. OFFSITE_CONVERSIONS, VALUE, LEAD_GENERATION) |  [optional] |
|**bidStrategy** | **BidStrategy** | Campaign-level bid strategy. Ad sets inherit this unless they override. |  [optional] |
|**bidAmount** | **BigDecimal** | Representative bid cap from the top-spending ad set (whole currency units). Populated when bidStrategy is LOWEST_COST_WITH_BID_CAP or COST_CAP. |  [optional] |
|**roasAverageFloor** | **BigDecimal** | Representative ROAS floor from the top-spending ad set. Decimal multiplier (2.0 &#x3D; 2.0x). |  [optional] |
|**promotedObject** | [**AdTreeCampaignPromotedObject**](AdTreeCampaignPromotedObject.md) |  |  [optional] |
|**earliestAd** | **OffsetDateTime** |  |  [optional] |
|**latestAd** | **OffsetDateTime** |  |  [optional] |



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



## Enum: ReviewStatusEnum

| Name | Value |
|---- | -----|
| IN_REVIEW | &quot;in_review&quot; |
| APPROVED | &quot;approved&quot; |
| REJECTED | &quot;rejected&quot; |
| WITH_ISSUES | &quot;with_issues&quot; |



## Enum: BudgetLevelEnum

| Name | Value |
|---- | -----|
| CAMPAIGN | &quot;campaign&quot; |
| ADSET | &quot;adset&quot; |



