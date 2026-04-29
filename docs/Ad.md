

# Ad


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**name** | **String** |  |  [optional] |
|**platform** | [**PlatformEnum**](#PlatformEnum) |  |  [optional] |
|**status** | **AdStatus** |  |  [optional] |
|**adType** | [**AdTypeEnum**](#AdTypeEnum) |  |  [optional] |
|**goal** | [**GoalEnum**](#GoalEnum) | Available goals vary by platform. Meta (Facebook/Instagram) and TikTok support all 7. LinkedIn supports all except app_promotion. Twitter/X supports engagement, traffic, awareness, video_views, app_promotion. Pinterest and Google Ads support only engagement, traffic, awareness, video_views. |  [optional] |
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
|**bidStrategy** | **BidStrategy** | Ad-set bid strategy (overrides campaign level on Meta). Populated for Meta and TikTok. TikTok&#39;s native &#x60;bid_type&#x60; is normalized to the cross-platform Meta enum: &#x60;BID_TYPE_NO_BID&#x60; -&gt; &#x60;LOWEST_COST_WITHOUT_CAP&#x60;, &#x60;BID_TYPE_CUSTOM&#x60; -&gt; &#x60;LOWEST_COST_WITH_BID_CAP&#x60;, deep_bid_type&#x3D;MIN_ROAS or roas_bid&gt;0 -&gt; &#x60;LOWEST_COST_WITH_MIN_ROAS&#x60;, &#x60;BID_TYPE_MAX_CONVERSION&#x60; -&gt; &#x60;LOWEST_COST_WITHOUT_CAP&#x60;.  |  [optional] |
|**bidAmount** | **BigDecimal** | Bid cap in WHOLE currency units of the ad account (USD: 5 &#x3D; $5.00; JPY: 100 &#x3D; ¥100). Populated when bidStrategy is &#x60;LOWEST_COST_WITH_BID_CAP&#x60; or &#x60;COST_CAP&#x60;. &#x60;null&#x60; for auto-bid (&#x60;LOWEST_COST_WITHOUT_CAP&#x60;).  - Meta source: &#x60;bid_amount&#x60; on the ad set (smallest-denomination int, decoded here). - TikTok source: priority order &#x60;bid_price&#x60; -&gt; &#x60;conversion_bid_price&#x60; -&gt; &#x60;deep_cpa_bid&#x60;   (whichever is set on the ad group). TikTok stores all three in whole currency units.  Source: facebook-business-sdk-codegen api_specs/specs/AdSet.json (&#x60;bid_amount&#x60;).  |  [optional] |
|**roasAverageFloor** | **BigDecimal** | Minimum ROAS as a decimal multiplier (2.0 &#x3D; 2.0x ROAS). Populated when bidStrategy is &#x60;LOWEST_COST_WITH_MIN_ROAS&#x60;.  - Meta source: decoded from &#x60;bid_constraints.roas_average_floor&#x60; (Meta stores as   fixed-point int × 10000; we return the decimal). - TikTok source: &#x60;roas_bid&#x60; on the ad group (already a decimal).  Source: facebook-business-sdk-codegen api_specs/specs/AdCampaignBidConstraint.json.  |  [optional] |
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
| LEAD_GENERATION | &quot;lead_generation&quot; |
| CONVERSIONS | &quot;conversions&quot; |
| APP_PROMOTION | &quot;app_promotion&quot; |



