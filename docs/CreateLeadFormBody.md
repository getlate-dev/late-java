

# CreateLeadFormBody


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**accountId** | **String** | Facebook social account ID (Late SocialAccount _id). |  |
|**name** | **String** |  |  |
|**questions** | [**List&lt;LeadGenFormQuestion&gt;**](LeadGenFormQuestion.md) |  |  |
|**privacyPolicyUrl** | **URI** | Required by Meta. Must be reachable from Meta&#39;s crawler. |  |
|**privacyPolicyLinkText** | **String** |  |  [optional] |
|**followUpActionUrl** | **URI** |  |  [optional] |
|**locale** | **String** |  |  [optional] |
|**thankYouTitle** | **String** |  |  [optional] |
|**thankYouBody** | **String** |  |  [optional] |
|**thankYouButtonText** | **String** |  |  [optional] |
|**thankYouButtonType** | **String** | Meta enum (e.g. VIEW_WEBSITE, CALL_BUSINESS, DOWNLOAD) |  [optional] |
|**thankYouWebsiteUrl** | **URI** |  |  [optional] |
|**isOptimizedForQuality** | **Boolean** |  |  [optional] |
|**contextCard** | [**CreateLeadFormBodyContextCard**](CreateLeadFormBodyContextCard.md) |  |  [optional] |
|**legalContent** | [**CreateLeadFormBodyLegalContent**](CreateLeadFormBodyLegalContent.md) |  |  [optional] |
|**trackingParameters** | **Map&lt;String, String&gt;** | Up to 20 key/value pairs surfaced on every lead for attribution. |  [optional] |
|**questionPageCustomHeadline** | **String** |  |  [optional] |
|**allowOrganicLead** | **Boolean** |  |  [optional] |
|**blockDisplayForNonTargetedViewer** | **Boolean** |  |  [optional] |



