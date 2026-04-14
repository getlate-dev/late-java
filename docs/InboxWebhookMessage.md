

# InboxWebhookMessage

The message object included in inbox webhook payloads.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** | Internal message ID |  |
|**conversationId** | **String** | Internal conversation ID |  |
|**platform** | [**PlatformEnum**](#PlatformEnum) |  |  |
|**platformMessageId** | **String** | Platform&#39;s message ID |  |
|**direction** | [**DirectionEnum**](#DirectionEnum) |  |  |
|**text** | **String** | Message text content (retained on deleted messages for API consumers; Zernio dashboard UI hides this) |  |
|**attachments** | [**List&lt;InboxWebhookMessageAttachmentsInner&gt;**](InboxWebhookMessageAttachmentsInner.md) |  |  |
|**sender** | [**InboxWebhookMessageSender**](InboxWebhookMessageSender.md) |  |  |
|**sentAt** | **OffsetDateTime** |  |  |
|**isRead** | **Boolean** |  |  |



## Enum: PlatformEnum

| Name | Value |
|---- | -----|
| INSTAGRAM | &quot;instagram&quot; |
| FACEBOOK | &quot;facebook&quot; |
| TELEGRAM | &quot;telegram&quot; |
| WHATSAPP | &quot;whatsapp&quot; |



## Enum: DirectionEnum

| Name | Value |
|---- | -----|
| INCOMING | &quot;incoming&quot; |
| OUTGOING | &quot;outgoing&quot; |



