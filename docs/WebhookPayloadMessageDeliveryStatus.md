

# WebhookPayloadMessageDeliveryStatus

Shared payload for message.delivered, message.read, and message.failed events. Fires when the platform reports a new delivery state for an outgoing message.  Platform support:   * message.delivered — WhatsApp, Facebook Messenger.   * message.read      — WhatsApp, Facebook Messenger, Instagram.   * message.failed    — WhatsApp only (other platforms don't expose     per-message failure via webhook). 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  |
|**event** | [**EventEnum**](#EventEnum) |  |  |
|**message** | [**InboxWebhookMessage**](InboxWebhookMessage.md) |  |  |
|**statusAt** | **OffsetDateTime** | When the platform reported this status. |  |
|**error** | [**WebhookPayloadMessageDeliveryStatusError**](WebhookPayloadMessageDeliveryStatusError.md) |  |  [optional] |
|**conversation** | [**InboxWebhookConversation**](InboxWebhookConversation.md) |  |  |
|**account** | [**InboxWebhookAccount**](InboxWebhookAccount.md) |  |  |
|**timestamp** | **OffsetDateTime** |  |  |



## Enum: EventEnum

| Name | Value |
|---- | -----|
| MESSAGE_DELIVERED | &quot;message.delivered&quot; |
| MESSAGE_READ | &quot;message.read&quot; |
| MESSAGE_FAILED | &quot;message.failed&quot; |



