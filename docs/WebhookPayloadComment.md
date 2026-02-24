

# WebhookPayloadComment

Webhook payload for comment received events (Instagram, Facebook, Twitter/X, YouTube, LinkedIn, Bluesky, Reddit)

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**event** | [**EventEnum**](#EventEnum) |  |  [optional] |
|**comment** | [**WebhookPayloadCommentComment**](WebhookPayloadCommentComment.md) |  |  [optional] |
|**post** | [**WebhookPayloadCommentPost**](WebhookPayloadCommentPost.md) |  |  [optional] |
|**account** | [**WebhookPayloadCommentAccount**](WebhookPayloadCommentAccount.md) |  |  [optional] |
|**timestamp** | **OffsetDateTime** |  |  [optional] |



## Enum: EventEnum

| Name | Value |
|---- | -----|
| COMMENT_RECEIVED | &quot;comment.received&quot; |



