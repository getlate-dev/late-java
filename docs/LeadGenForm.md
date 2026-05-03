

# LeadGenForm

A Meta Lead Gen (Instant) Form definition.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**name** | **String** |  |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) |  |  [optional] |
|**locale** | **String** |  |  [optional] |
|**createdTime** | **OffsetDateTime** |  |  [optional] |
|**leadsCount** | **Integer** | Total leads (real + organic). |  [optional] |
|**organicLeadsCount** | **Integer** |  |  [optional] |
|**expiredLeadsCount** | **Integer** |  |  [optional] |
|**questions** | [**List&lt;LeadGenFormQuestion&gt;**](LeadGenFormQuestion.md) |  |  [optional] |
|**privacyPolicyUrl** | **String** |  |  [optional] |
|**followUpActionUrl** | **String** |  |  [optional] |
|**thankYouPage** | **Object** |  |  [optional] |
|**contextCard** | **Object** |  |  [optional] |
|**questionPageCustomHeadline** | **String** |  |  [optional] |
|**isOptimizedForQuality** | **Boolean** |  |  [optional] |
|**pageId** | **String** |  |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| ACTIVE | &quot;ACTIVE&quot; |
| ARCHIVED | &quot;ARCHIVED&quot; |
| DELETED | &quot;DELETED&quot; |
| DRAFT | &quot;DRAFT&quot; |



