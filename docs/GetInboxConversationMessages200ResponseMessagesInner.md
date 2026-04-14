

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
|**senderVerifiedType** | [**SenderVerifiedTypeEnum**](#SenderVerifiedTypeEnum) | X/Twitter verified badge type. Only present for Twitter/X messages. |  [optional] |
|**direction** | [**DirectionEnum**](#DirectionEnum) |  |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  [optional] |
|**attachments** | [**List&lt;GetInboxConversationMessages200ResponseMessagesInnerAttachmentsInner&gt;**](GetInboxConversationMessages200ResponseMessagesInnerAttachmentsInner.md) |  |  [optional] |
|**subject** | **String** | Reddit message subject |  [optional] |
|**storyReply** | **Boolean** | Instagram story reply |  [optional] |
|**isStoryMention** | **Boolean** | Instagram story mention |  [optional] |
|**isEdited** | **Boolean** | True if the sender has edited this message at least once. |  [optional] |
|**editedAt** | **OffsetDateTime** | When the most recent edit happened. |  [optional] |
|**editCount** | **Integer** | Total number of edits applied. |  [optional] |
|**editHistory** | [**List&lt;GetInboxConversationMessages200ResponseMessagesInnerEditHistoryInner&gt;**](GetInboxConversationMessages200ResponseMessagesInnerEditHistoryInner.md) | Every prior version of the message, oldest first. |  [optional] |
|**isDeleted** | **Boolean** | True if the sender has deleted (unsent) this message. The original message and attachments fields remain populated. |  [optional] |
|**deletedAt** | **OffsetDateTime** |  |  [optional] |
|**deliveryStatus** | [**DeliveryStatusEnum**](#DeliveryStatusEnum) | Lifecycle status for outgoing messages. Not all platforms emit every state (see webhook support matrix). |  [optional] |
|**deliveredAt** | **OffsetDateTime** |  |  [optional] |
|**readAt** | **OffsetDateTime** |  |  [optional] |
|**sentAt** | **OffsetDateTime** | Original send time for outgoing messages (used for Messenger watermark queries). |  [optional] |
|**deliveryError** | [**GetInboxConversationMessages200ResponseMessagesInnerDeliveryError**](GetInboxConversationMessages200ResponseMessagesInnerDeliveryError.md) |  |  [optional] |



## Enum: SenderVerifiedTypeEnum

| Name | Value |
|---- | -----|
| BLUE | &quot;blue&quot; |
| GOVERNMENT | &quot;government&quot; |
| BUSINESS | &quot;business&quot; |
| NONE | &quot;none&quot; |



## Enum: DirectionEnum

| Name | Value |
|---- | -----|
| INCOMING | &quot;incoming&quot; |
| OUTGOING | &quot;outgoing&quot; |



## Enum: DeliveryStatusEnum

| Name | Value |
|---- | -----|
| SENT | &quot;sent&quot; |
| DELIVERED | &quot;delivered&quot; |
| READ | &quot;read&quot; |
| FAILED | &quot;failed&quot; |
| DELETED | &quot;deleted&quot; |



