

# GetInboxPostComments200ResponseCommentsInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**message** | **String** |  |  [optional] |
|**createdTime** | **OffsetDateTime** |  |  [optional] |
|**from** | [**GetInboxPostComments200ResponseCommentsInnerFrom**](GetInboxPostComments200ResponseCommentsInnerFrom.md) |  |  [optional] |
|**likeCount** | **Integer** |  |  [optional] |
|**replyCount** | **Integer** |  |  [optional] |
|**platform** | **String** | The platform this comment is from |  [optional] |
|**url** | **String** | Direct link to the comment on the platform (if available) |  [optional] |
|**replies** | **List&lt;Object&gt;** |  |  [optional] |
|**canReply** | **Boolean** |  |  [optional] |
|**canDelete** | **Boolean** |  |  [optional] |
|**canHide** | **Boolean** | Whether this comment can be hidden (Facebook |  [optional] |
|**canLike** | **Boolean** | Whether this comment can be liked (Facebook |  [optional] |
|**isHidden** | **Boolean** | Whether the comment is currently hidden |  [optional] |
|**isLiked** | **Boolean** | Whether the current user has liked this comment |  [optional] |
|**likeUri** | **String** | Bluesky like URI for unliking |  [optional] |
|**cid** | **String** | Bluesky content identifier |  [optional] |
|**parentId** | **String** | Parent comment ID for nested replies |  [optional] |
|**rootUri** | **String** | Bluesky root post URI |  [optional] |
|**rootCid** | **String** | Bluesky root post CID |  [optional] |



