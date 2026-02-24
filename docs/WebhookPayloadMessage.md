

# WebhookPayloadMessage

Webhook payload for message received events (DMs from Instagram, Facebook, Telegram, Bluesky, Reddit)

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**event** | [**EventEnum**](#EventEnum) |  |  [optional] |
|**message** | [**WebhookPayloadMessageMessage**](WebhookPayloadMessageMessage.md) |  |  [optional] |
|**conversation** | [**WebhookPayloadMessageConversation**](WebhookPayloadMessageConversation.md) |  |  [optional] |
|**account** | [**WebhookPayloadMessageAccount**](WebhookPayloadMessageAccount.md) |  |  [optional] |
|**metadata** | [**WebhookPayloadMessageMetadata**](WebhookPayloadMessageMetadata.md) |  |  [optional] |
|**timestamp** | **OffsetDateTime** |  |  [optional] |



## Enum: EventEnum

| Name | Value |
|---- | -----|
| MESSAGE_RECEIVED | &quot;message.received&quot; |



