

# WebhookPayloadCommentComment


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** | Platform comment ID |  [optional] |
|**postId** | **String** | Internal post ID |  [optional] |
|**platformPostId** | **String** | Platform&#39;s post ID |  [optional] |
|**platform** | [**PlatformEnum**](#PlatformEnum) |  |  [optional] |
|**text** | **String** | Comment text content |  [optional] |
|**author** | [**WebhookPayloadCommentCommentAuthor**](WebhookPayloadCommentCommentAuthor.md) |  |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  [optional] |
|**isReply** | **Boolean** | Whether this is a reply to another comment |  [optional] |
|**parentCommentId** | **String** | Parent comment ID if this is a reply |  [optional] |



## Enum: PlatformEnum

| Name | Value |
|---- | -----|
| INSTAGRAM | &quot;instagram&quot; |
| FACEBOOK | &quot;facebook&quot; |
| TWITTER | &quot;twitter&quot; |
| YOUTUBE | &quot;youtube&quot; |
| LINKEDIN | &quot;linkedin&quot; |
| BLUESKY | &quot;bluesky&quot; |
| REDDIT | &quot;reddit&quot; |



