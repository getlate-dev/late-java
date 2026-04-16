

# WebhookPayloadCommentComment


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** | Platform comment ID |  |
|**postId** | **String** | Internal post ID (null for posts not published through Zernio) |  |
|**platformPostId** | **String** | Platform&#39;s post ID |  |
|**platform** | [**PlatformEnum**](#PlatformEnum) |  |  |
|**text** | **String** | Comment text content |  |
|**author** | [**WebhookPayloadCommentCommentAuthor**](WebhookPayloadCommentCommentAuthor.md) |  |  |
|**createdAt** | **OffsetDateTime** |  |  |
|**isReply** | **Boolean** | Whether this is a reply to another comment |  |
|**parentCommentId** | **String** | Parent comment ID if this is a reply |  |



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



