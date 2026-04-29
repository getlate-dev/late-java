

# BoostPostRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**postId** | **String** | Zernio post ID (provide this or platformPostId) |  [optional] |
|**platformPostId** | **String** | Platform post ID (alternative to postId) |  [optional] |
|**accountId** | **String** | Social account ID |  |
|**adAccountId** | **String** | Platform ad account ID |  |
|**name** | **String** |  |  |
|**goal** | [**GoalEnum**](#GoalEnum) | Available goals vary by platform. Meta (Facebook/Instagram) and TikTok support all 7. LinkedIn supports all except app_promotion. Twitter/X supports engagement, traffic, awareness, video_views, app_promotion. Pinterest and Google Ads support only engagement, traffic, awareness, video_views. |  |
|**budget** | [**BoostPostRequestBudget**](BoostPostRequestBudget.md) |  |  |
|**currency** | **String** |  |  [optional] |
|**schedule** | [**BoostPostRequestSchedule**](BoostPostRequestSchedule.md) |  |  [optional] |
|**targeting** | [**BoostPostRequestTargeting**](BoostPostRequestTargeting.md) |  |  [optional] |
|**bidStrategy** | **BidStrategy** | Meta bid strategy applied to the ad set. On TikTok, mapped to &#x60;bid_type&#x60; / &#x60;bid_price&#x60; / &#x60;deep_bid_type&#x60; automatically.  |  [optional] |
|**bidAmount** | **BigDecimal** | Bid cap in WHOLE currency units (USD: 5 &#x3D; $5.00; JPY: 100 &#x3D; ¥100). Required when &#x60;bidStrategy&#x60; is &#x60;LOWEST_COST_WITH_BID_CAP&#x60; or &#x60;COST_CAP&#x60;. Backward-compat: providing &#x60;bidAmount&#x60; without &#x60;bidStrategy&#x60; is treated as &#x60;LOWEST_COST_WITH_BID_CAP&#x60;.  |  [optional] |
|**roasAverageFloor** | **BigDecimal** | Minimum ROAS as a decimal multiplier (e.g. 2.0 &#x3D; 2.0x ROAS). Required when &#x60;bidStrategy&#x60; is &#x60;LOWEST_COST_WITH_MIN_ROAS&#x60;. Sent to Meta as &#x60;bid_constraints.roas_average_floor&#x60; × 10000 (Meta uses fixed-point integers).  |  [optional] |
|**tracking** | [**BoostPostRequestTracking**](BoostPostRequestTracking.md) |  |  [optional] |
|**specialAdCategories** | [**List&lt;SpecialAdCategoriesEnum&gt;**](#List&lt;SpecialAdCategoriesEnum&gt;) | Meta only. Required for housing, employment, credit, or political ads. |  [optional] |
|**linkUrl** | **URI** | TikTok-only. Custom destination URL for the Spark Ad. Without this, TikTok Spark Ads have no clickable destination — required for traffic / conversion objectives. Maps to &#x60;landing_page_url&#x60; on the creative entry of /v2/ad/create/ (TikTok SDK &#x60;AdcreateCreatives.landing_page_url&#x60;). Ignored on Meta / LinkedIn / Pinterest / X / Google (those infer the destination from the boosted post).  |  [optional] |
|**callToAction** | **String** | TikTok-only. Call-to-action button label on the Spark Ad creative (e.g. &#x60;LEARN_MORE&#x60;, &#x60;SHOP_NOW&#x60;, &#x60;DOWNLOAD_NOW&#x60;, &#x60;SIGN_UP&#x60;, &#x60;WATCH_NOW&#x60;). Maps to &#x60;call_to_action&#x60; on the creative entry of /v2/ad/create/. Pass-through — the platform validates the value. See TikTok&#39;s \&quot;Enumeration - Call-to-Action\&quot; reference for the full list.  |  [optional] |
|**sparkAuthCode** | **String** | TikTok-only. Spark Code (creator&#39;s &#x60;auth_code&#x60;) authorizing cross-creator Spark Ads — the advertiser can boost a video owned by a DIFFERENT TikTok account. Without this, boosts are limited to videos owned by the same account running the ads (same-BC creators only). The creator generates the code in their TikTok app&#39;s Promote settings and shares it with the advertiser. Maps to &#x60;auth_code&#x60; on the creative entry of /v2/ad/create/.  |  [optional] |
|**dsaBeneficiary** | **String** | Name of the legal entity benefiting from the ad. Required by Meta when targeting EU users (DSA Article 26). Not enforced at schema level; enforced server-side when targeting intersects EU member states.  |  [optional] |
|**dsaPayor** | **String** | Name of the legal entity paying for the ad. Required by Meta when targeting EU users (DSA Article 26). Note Meta API spelling: dsa_payor (not dsa_payer).  |  [optional] |



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



## Enum: List&lt;SpecialAdCategoriesEnum&gt;

| Name | Value |
|---- | -----|
| HOUSING | &quot;HOUSING&quot; |
| EMPLOYMENT | &quot;EMPLOYMENT&quot; |
| CREDIT | &quot;CREDIT&quot; |
| ISSUES_ELECTIONS_POLITICS | &quot;ISSUES_ELECTIONS_POLITICS&quot; |



