

# GetInboxConversationMessages200ResponseMessagesInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**conversationId** | **String** |  |  [optional] |
|**accountId** | **String** |  |  [optional] |
|**platform** | **String** |  |  [optional] |
|**message** | **String** |  |  [optional] |
|**senderId** | **String** |  |  [optional] |
|**senderName** | **String** |  |  [optional] |
|**direction** | [**DirectionEnum**](#DirectionEnum) |  |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  [optional] |
|**attachments** | [**List&lt;GetInboxConversationMessages200ResponseMessagesInnerAttachmentsInner&gt;**](GetInboxConversationMessages200ResponseMessagesInnerAttachmentsInner.md) |  |  [optional] |
|**subject** | **String** | Reddit message subject |  [optional] |
|**storyReply** | **Boolean** | Instagram story reply |  [optional] |
|**isStoryMention** | **Boolean** | Instagram story mention |  [optional] |



## Enum: DirectionEnum

| Name | Value |
|---- | -----|
| INCOMING | &quot;incoming&quot; |
| OUTGOING | &quot;outgoing&quot; |



