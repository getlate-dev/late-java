

# SendInboxMessageRequest1


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**accountId** | **String** | Social account ID |  |
|**message** | **String** | Message text (optional when sending attachment) |  [optional] |
|**attachment** | **File** | File attachment (images, videos, documents). Supported formats: JPEG, PNG, GIF, MP4, AAC, WAV. Max 25MB. |  [optional] |
|**quickReplies** | **String** | JSON string of quick replies array (same schema as application/json body) |  [optional] |
|**buttons** | **String** | JSON string of buttons array (same schema as application/json body) |  [optional] |
|**template** | **String** | JSON string of template object (same schema as application/json body) |  [optional] |
|**replyMarkup** | **String** | JSON string of replyMarkup object (same schema as application/json body) |  [optional] |
|**messagingType** | **String** | Messaging type (Facebook only). RESPONSE, UPDATE, or MESSAGE_TAG. |  [optional] |
|**messageTag** | **String** | Message tag (requires messagingType MESSAGE_TAG) |  [optional] |
|**replyTo** | **String** | Platform message ID to quote-reply to. For WhatsApp, pass the wamid (available in message.platformMessageId from webhooks). For Telegram, pass the Telegram message ID. |  [optional] |



