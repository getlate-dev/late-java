

# WebhookPayloadMessageSentMessage


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** | Internal message ID |  |
|**conversationId** | **String** | Internal conversation ID |  |
|**platform** | [**PlatformEnum**](#PlatformEnum) |  |  |
|**platformMessageId** | **String** | Platform&#39;s message ID |  |
|**direction** | [**DirectionEnum**](#DirectionEnum) |  |  |
|**text** | **String** | Message text content |  |
|**attachments** | [**List&lt;WebhookPayloadMessageMessageAttachmentsInner&gt;**](WebhookPayloadMessageMessageAttachmentsInner.md) |  |  |
|**sender** | [**WebhookPayloadMessageSentMessageSender**](WebhookPayloadMessageSentMessageSender.md) |  |  |
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



