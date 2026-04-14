

# CreateStandaloneAdRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**accountId** | **String** |  |  |
|**adAccountId** | **String** |  |  |
|**name** | **String** |  |  |
|**goal** | [**GoalEnum**](#GoalEnum) |  |  |
|**budgetAmount** | **BigDecimal** |  |  |
|**budgetType** | [**BudgetTypeEnum**](#BudgetTypeEnum) |  |  |
|**currency** | **String** |  |  [optional] |
|**headline** | **String** | Required for most platforms. Max: Meta&#x3D;255, Google&#x3D;30, Pinterest&#x3D;100 |  [optional] |
|**longHeadline** | **String** | Google Display only |  [optional] |
|**body** | **String** | Max: Google&#x3D;90, Pinterest&#x3D;500 |  |
|**callToAction** | [**CallToActionEnum**](#CallToActionEnum) | Meta only |  [optional] |
|**linkUrl** | **URI** |  |  [optional] |
|**imageUrl** | **URI** | Image URL (or video URL for TikTok). Not required for Google Search campaigns. |  [optional] |
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



## Enum: GoalEnum

| Name | Value |
|---- | -----|
| ENGAGEMENT | &quot;engagement&quot; |
| TRAFFIC | &quot;traffic&quot; |
| AWARENESS | &quot;awareness&quot; |
| VIDEO_VIEWS | &quot;video_views&quot; |



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



