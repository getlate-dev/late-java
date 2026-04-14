

# AdTreeAdSet

Ad set (or ad group/line item depending on platform) with rolled-up metrics and child ads

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**platformAdSetId** | **String** |  |  [optional] |
|**adSetName** | **String** |  |  [optional] |
|**status** | **AdStatus** | Derived from child ad statuses |  [optional] |
|**adCount** | **Integer** |  |  [optional] |
|**budget** | [**AdBudget**](AdBudget.md) |  |  [optional] |
|**metrics** | [**AdMetrics**](AdMetrics.md) |  |  [optional] |
|**optimizationGoal** | **String** | Meta ad set optimization goal (e.g. OFFSITE_CONVERSIONS, VALUE, LEAD_GENERATION) |  [optional] |
|**bidStrategy** | **String** | Bid strategy for this ad set (overrides campaign level when set) |  [optional] |
|**promotedObject** | [**AdTreeAdSetPromotedObject**](AdTreeAdSetPromotedObject.md) |  |  [optional] |
|**ads** | [**List&lt;Ad&gt;**](Ad.md) | Individual ads within this ad set (capped at 100). Returns a subset of Ad fields from the aggregation (core fields like _id, name, platform, status, budget, metrics, creative, goal are included; targeting and schedule may be absent). |  [optional] |



