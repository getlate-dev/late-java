

# CreateStandaloneAdRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**accountId** | **String** |  |  |
|**adAccountId** | **String** |  |  |
|**name** | **String** |  |  |
|**goal** | [**GoalEnum**](#GoalEnum) | Required on legacy + multi-creative shapes. Inherited from the ad set on the attach shape. Available goals vary by platform. |  [optional] |
|**budgetAmount** | **BigDecimal** | Required on legacy + multi-creative shapes. Inherited on attach. |  [optional] |
|**budgetType** | [**BudgetTypeEnum**](#BudgetTypeEnum) | Required on legacy + multi-creative shapes. Inherited on attach. |  [optional] |
|**currency** | **String** |  |  [optional] |
|**headline** | **String** | Required on legacy + attach shapes (skip for multi-creative — use &#x60;creatives[].headline&#x60;). Max: Meta&#x3D;255, Google&#x3D;30, Pinterest&#x3D;100 |  [optional] |
|**longHeadline** | **String** | Google Display only |  [optional] |
|**body** | **String** | Required on legacy + attach shapes. Max: Google&#x3D;90, Pinterest&#x3D;500 |  [optional] |
|**callToAction** | [**CallToActionEnum**](#CallToActionEnum) | Required on legacy + attach shapes. Meta only. |  [optional] |
|**linkUrl** | **URI** | Required on legacy + attach shapes. Skip for multi-creative. |  [optional] |
|**imageUrl** | **URI** | Required on legacy + attach shapes. Not required for Google Search campaigns. |  [optional] |
|**creatives** | [**List&lt;CreateStandaloneAdRequestCreativesInner&gt;**](CreateStandaloneAdRequestCreativesInner.md) | Meta-only. When present, switches to the multi-creative shape: creates 1 campaign + 1 ad set + N ads (one per entry here). Top-level &#x60;headline&#x60; / &#x60;body&#x60; / &#x60;imageUrl&#x60; / &#x60;linkUrl&#x60; / &#x60;callToAction&#x60; are ignored in this mode. Mutually exclusive with &#x60;adSetId&#x60;.  |  [optional] |
|**adSetId** | **String** | Meta-only. When present, switches to the attach shape: adds one new ad to this existing ad set without creating a new campaign. Budget, targeting, goal, and schedule are inherited from the ad set on Meta. Mutually exclusive with &#x60;creatives[]&#x60;.  |  [optional] |
|**businessName** | **String** | Google Display only |  [optional] |
|**boardId** | **String** | Pinterest only. Board ID (auto-creates if not provided). |  [optional] |
|**countries** | **List&lt;String&gt;** |  |  [optional] |
|**ageMin** | **Integer** |  |  [optional] |
|**ageMax** | **Integer** |  |  [optional] |
|**interests** | [**List&lt;UpdateAdRequestTargetingInterestsInner&gt;**](UpdateAdRequestTargetingInterestsInner.md) | Interest objects from /v1/ads/interests. Each must include id and name. |  [optional] |
|**endDate** | **OffsetDateTime** | Required for lifetime budgets |  [optional] |
|**audienceId** | **String** | Custom audience ID for targeting |  [optional] |
|**campaignType** | [**CampaignTypeEnum**](#CampaignTypeEnum) | Google only |  [optional] |
|**keywords** | **List&lt;String&gt;** | Google Search only |  [optional] |
|**additionalHeadlines** | **List&lt;String&gt;** | Google Search RSA only. Extra headlines. |  [optional] |
|**additionalDescriptions** | **List&lt;String&gt;** | Google Search RSA only. Extra descriptions. |  [optional] |
|**advantageAudience** | [**AdvantageAudienceEnum**](#AdvantageAudienceEnum) | Meta only. Controls the Advantage audience feature (targeting_automation). 0 &#x3D; disabled (default), 1 &#x3D; enabled. Meta Marketing API requires this field on all ad set creation requests. |  [optional] |



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



## Enum: BudgetTypeEnum

| Name | Value |
|---- | -----|
| DAILY | &quot;daily&quot; |
| LIFETIME | &quot;lifetime&quot; |



## Enum: CallToActionEnum

| Name | Value |
|---- | -----|
| LEARN_MORE | &quot;LEARN_MORE&quot; |
| SHOP_NOW | &quot;SHOP_NOW&quot; |
| SIGN_UP | &quot;SIGN_UP&quot; |
| BOOK_TRAVEL | &quot;BOOK_TRAVEL&quot; |
| CONTACT_US | &quot;CONTACT_US&quot; |
| DOWNLOAD | &quot;DOWNLOAD&quot; |
| GET_OFFER | &quot;GET_OFFER&quot; |
| GET_QUOTE | &quot;GET_QUOTE&quot; |
| SUBSCRIBE | &quot;SUBSCRIBE&quot; |
| WATCH_MORE | &quot;WATCH_MORE&quot; |



## Enum: CampaignTypeEnum

| Name | Value |
|---- | -----|
| DISPLAY | &quot;display&quot; |
| SEARCH | &quot;search&quot; |



## Enum: AdvantageAudienceEnum

| Name | Value |
|---- | -----|
| NUMBER_0 | 0 |
| NUMBER_1 | 1 |



