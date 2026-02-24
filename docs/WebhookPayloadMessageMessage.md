

# WebhookPayloadMessageMessage


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** | Internal message ID |  [optional] |
|**conversationId** | **String** | Internal conversation ID |  [optional] |
|**platform** | [**PlatformEnum**](#PlatformEnum) |  |  [optional] |
|**platformMessageId** | **String** | Platform&#39;s message ID |  [optional] |
|**direction** | [**DirectionEnum**](#DirectionEnum) |  |  [optional] |
|**text** | **String** | Message text content |  [optional] |
|**attachments** | [**List&lt;WebhookPayloadMessageMessageAttachmentsInner&gt;**](WebhookPayloadMessageMessageAttachmentsInner.md) |  |  [optional] |
|**sender** | [**WebhookPayloadMessageMessageSender**](WebhookPayloadMessageMessageSender.md) |  |  [optional] |
|**sentAt** | **OffsetDateTime** |  |  [optional] |
|**isRead** | **Boolean** |  |  [optional] |



## Enum: PlatformEnum

| Name | Value |
|---- | -----|
| INSTAGRAM | &quot;instagram&quot; |
| FACEBOOK | &quot;facebook&quot; |
| TELEGRAM | &quot;telegram&quot; |
| BLUESKY | &quot;bluesky&quot; |
| REDDIT | &quot;reddit&quot; |



## Enum: DirectionEnum

| Name | Value |
|---- | -----|
| INCOMING | &quot;incoming&quot; |



