

# InstagramPlatformData

Feed posts require aspect ratio 0.8-1.91; images outside this range must use contentType story. Carousels up to 10 items. Stories require media, no captions. User tag coordinates 0.0-1.0 from top-left. Images over 8 MB and videos over 100 MB (stories) or 300 MB (reels) are auto-compressed.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**contentType** | [**ContentTypeEnum**](#ContentTypeEnum) | Set to &#39;story&#39; to publish as a Story. Default posts become Reels or feed depending on media. |  [optional] |
|**shareToFeed** | **Boolean** | For Reels only. When true (default), the Reel appears on both the Reels tab and your main profile feed. Set to false to post to the Reels tab only. |  [optional] |
|**collaborators** | **List&lt;String&gt;** | Up to 3 Instagram usernames to invite as collaborators (feed/Reels only) |  [optional] |
|**firstComment** | **String** | Optional first comment to add after the post is created (not applied to Stories) |  [optional] |
|**trialParams** | [**InstagramPlatformDataTrialParams**](InstagramPlatformDataTrialParams.md) |  |  [optional] |
|**userTags** | [**List&lt;InstagramPlatformDataUserTagsInner&gt;**](InstagramPlatformDataUserTagsInner.md) | Tag Instagram users in photos by username and position. Not supported for stories or videos. For carousels, use mediaIndex to target specific slides (defaults to 0). Tags on video items are silently skipped. |  [optional] |
|**audioName** | **String** | Custom name for original audio in Reels. Replaces the default \&quot;Original Audio\&quot; label. Can only be set once. |  [optional] |
|**thumbOffset** | **Integer** | Millisecond offset from video start for the Reel thumbnail. Ignored if a custom thumbnail URL is provided. Defaults to 0. |  [optional] |



## Enum: ContentTypeEnum

| Name | Value |
|---- | -----|
| STORY | &quot;story&quot; |



