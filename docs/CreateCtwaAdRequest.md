

# CreateCtwaAdRequest

In addition to the `required` list, **exactly one of `imageUrl` or `video` must be supplied** (mutually exclusive). The route enforces this at the Zod boundary; OpenAPI's `required` cannot express OR-required cleanly. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**accountId** | **String** | Facebook or Instagram SocialAccount ID. |  |
|**adAccountId** | **String** | Meta ad account ID, e.g. &#x60;act_123456789&#x60;. |  |
|**name** | **String** | Ad display name. Used to derive campaign / ad set names. |  |
|**headline** | **String** |  |  |
|**body** | **String** | Primary text shown above the image / video. |  |
|**imageUrl** | **URI** | Image asset for image creatives. Mutually exclusive with &#x60;video&#x60;. Required if &#x60;video&#x60; is not supplied.  |  [optional] |
|**video** | [**CreateCtwaAdRequestVideo**](CreateCtwaAdRequestVideo.md) |  |  [optional] |
|**budgetAmount** | **BigDecimal** | Budget amount in the ad account&#39;s currency major units (e.g. dollars for USD, not cents). Must be positive.  |  |
|**budgetType** | [**BudgetTypeEnum**](#BudgetTypeEnum) |  |  |
|**currency** | **String** | ISO 4217 currency code matching the ad account&#39;s currency (e.g. &#x60;USD&#x60;). Optional — Meta infers from the ad account when omitted.  |  [optional] |
|**endDate** | **OffsetDateTime** | ISO 8601 datetime. Required when &#x60;budgetType&#x60; is &#x60;lifetime&#x60;.  |  [optional] |
|**countries** | **List&lt;String&gt;** | ISO 3166-1 alpha-2 country codes. Defaults to &#x60;[\&quot;US\&quot;]&#x60;. |  [optional] |
|**ageMin** | **Integer** |  |  [optional] |
|**ageMax** | **Integer** |  |  [optional] |
|**interests** | [**List&lt;CreateCtwaAdRequestInterestsInner&gt;**](CreateCtwaAdRequestInterestsInner.md) |  |  [optional] |
|**audienceId** | **String** | Custom audience ID to target. |  [optional] |
|**advantageAudience** | [**AdvantageAudienceEnum**](#AdvantageAudienceEnum) | Meta&#39;s Advantage+ audience expansion. &#x60;0&#x60; (default) keeps targeting strict; &#x60;1&#x60; lets Meta expand beyond the supplied targeting when its delivery system finds better matches. Always sent on CREATE (Meta requires it).  |  [optional] |
|**objective** | [**ObjectiveEnum**](#ObjectiveEnum) | Defaults to &#x60;OUTCOME_ENGAGEMENT&#x60; (the broadly-supported CTWA objective). &#x60;OUTCOME_SALES&#x60; and &#x60;OUTCOME_LEADS&#x60; require additional account configuration (Dataset linked to the WABA for sales) and may be rejected by Meta if missing.  |  [optional] |



## Enum: BudgetTypeEnum

| Name | Value |
|---- | -----|
| DAILY | &quot;daily&quot; |
| LIFETIME | &quot;lifetime&quot; |



## Enum: AdvantageAudienceEnum

| Name | Value |
|---- | -----|
| NUMBER_0 | 0 |
| NUMBER_1 | 1 |



## Enum: ObjectiveEnum

| Name | Value |
|---- | -----|
| OUTCOME_ENGAGEMENT | &quot;OUTCOME_ENGAGEMENT&quot; |
| OUTCOME_SALES | &quot;OUTCOME_SALES&quot; |
| OUTCOME_LEADS | &quot;OUTCOME_LEADS&quot; |



