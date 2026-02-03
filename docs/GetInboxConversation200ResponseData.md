

# GetInboxConversation200ResponseData


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**accountId** | **String** |  |  [optional] |
|**accountUsername** | **String** |  |  [optional] |
|**platform** | **String** |  |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) |  |  [optional] |
|**participantName** | **String** |  |  [optional] |
|**participantId** | **String** |  |  [optional] |
|**lastMessage** | **String** |  |  [optional] |
|**lastMessageAt** | **OffsetDateTime** |  |  [optional] |
|**updatedTime** | **OffsetDateTime** |  |  [optional] |
|**participants** | [**List&lt;UpdateFacebookPage200ResponseSelectedPage&gt;**](UpdateFacebookPage200ResponseSelectedPage.md) |  |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| ACTIVE | &quot;active&quot; |
| ARCHIVED | &quot;archived&quot; |



