

# WebhookPayloadMessageDeleted

Webhook payload for `message.deleted` events. Fires when the sender deletes (unsends) a message. Supported platforms: Instagram (incoming unsend) and WhatsApp (when the business deletes an outgoing message via the Cloud API).  The `message.text` and `message.attachments` fields retain the content that existed before the delete. The Zernio dashboard UI does not show this content, but authorized API consumers may access it for moderation, compliance, or archival use cases. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  |
|**event** | [**EventEnum**](#EventEnum) |  |  |
|**message** | [**WebhookPayloadMessageMessage**](WebhookPayloadMessageMessage.md) |  |  |
|**deletedAt** | **OffsetDateTime** |  |  |
|**conversation** | [**WebhookPayloadMessageConversation**](WebhookPayloadMessageConversation.md) |  |  |
|**account** | [**WebhookPayloadMessageAccount**](WebhookPayloadMessageAccount.md) |  |  |
|**timestamp** | **OffsetDateTime** |  |  |



## Enum: EventEnum

| Name | Value |
|---- | -----|
| MESSAGE_DELETED | &quot;message.deleted&quot; |



