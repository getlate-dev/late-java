

# UpdateAdSetRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**platform** | [**PlatformEnum**](#PlatformEnum) |  |  |
|**budget** | [**UpdateAdSetRequestBudget**](UpdateAdSetRequestBudget.md) |  |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) | Omit if not toggling delivery state |  [optional] |
|**bidStrategy** | **BidStrategy** | Ad-set-level bid strategy. Overrides the campaign-level default. Supported on Meta (facebook, instagram) and TikTok. On TikTok the Meta-style enum is mapped to bid_type / bid_price / deep_bid_type automatically. Other platforms (linkedin, pinterest, google, twitter) return 501 Not Implemented when bidStrategy is set.  |  [optional] |
|**bidAmount** | **BigDecimal** | Bid cap in WHOLE currency units (USD: 5 &#x3D; $5.00; JPY: 100 &#x3D; ¥100). Required when bidStrategy is LOWEST_COST_WITH_BID_CAP or COST_CAP. Internally converted to Meta&#39;s smallest-denomination integer.  |  [optional] |
|**roasAverageFloor** | **BigDecimal** | Minimum ROAS as a decimal multiplier (2.0 &#x3D; 2.0x). Required when bidStrategy is LOWEST_COST_WITH_MIN_ROAS. Sent to Meta as &#x60;bid_constraints.roas_average_floor&#x60; × 10000.  |  [optional] |



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



