

# WebhookPayloadMessageEdited

Webhook payload for message.edited events. Fires when the sender edits a previously-sent message. Supported platforms: Instagram, Facebook Messenger, Telegram. The message object reflects the LATEST state; editHistory contains every prior version in order (oldest first), so the last entry is the version immediately before the current content. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  |
|**event** | [**EventEnum**](#EventEnum) |  |  |
|**message** | [**InboxWebhookMessage**](InboxWebhookMessage.md) |  |  |
|**editHistory** | [**List&lt;WebhookPayloadMessageEditedEditHistoryInner&gt;**](WebhookPayloadMessageEditedEditHistoryInner.md) | Prior versions of the message, oldest first. |  |
|**editCount** | **Integer** | Total number of edits applied to this message. |  |
|**editedAt** | **OffsetDateTime** | When the most recent edit happened. |  |
|**conversation** | [**InboxWebhookConversation**](InboxWebhookConversation.md) |  |  |
|**account** | [**InboxWebhookAccount**](InboxWebhookAccount.md) |  |  |
|**timestamp** | **OffsetDateTime** |  |  |



## Enum: EventEnum

| Name | Value |
|---- | -----|
| MESSAGE_EDITED | &quot;message.edited&quot; |



