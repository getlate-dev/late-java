

# ListInboxConversations200ResponseDataInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**platform** | **String** |  |  [optional] |
|**accountId** | **String** |  |  [optional] |
|**accountUsername** | **String** |  |  [optional] |
|**participantId** | **String** |  |  [optional] |
|**participantName** | **String** |  |  [optional] |
|**participantPicture** | **String** |  |  [optional] |
|**lastMessage** | **String** |  |  [optional] |
|**updatedTime** | **OffsetDateTime** |  |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) |  |  [optional] |
|**unreadCount** | **Integer** | Number of unread messages |  [optional] |
|**url** | **String** | Direct link to open the conversation on the platform (if available) |  [optional] |
|**instagramProfile** | [**ListInboxConversations200ResponseDataInnerInstagramProfile**](ListInboxConversations200ResponseDataInnerInstagramProfile.md) |  |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| ACTIVE | &quot;active&quot; |
| ARCHIVED | &quot;archived&quot; |



