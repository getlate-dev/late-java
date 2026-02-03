

# InstagramPlatformData

Constraints: - Feed posts require images with aspect ratio between 0.8 (4:5 portrait) and 1.91 (1.91:1 landscape). - Images outside this range (e.g., 9:16 Stories/TikTok format) must use contentType 'story'. - Validation happens at post creation; invalid images are rejected immediately with helpful error messages. - Carousels support up to 10 media items. - Stories require media; no captions are published with Stories. - User tags: coordinates range from 0.0 to 1.0 representing position from top-left corner. Tagged users receive notifications.  **Automatic Compression (similar to Bluesky):** - All images (story, post, carousel, thumbnails) exceeding 8 MB are automatically compressed using quality reduction and resizing. - Story videos exceeding 100 MB are automatically compressed. - Reel videos exceeding 300 MB are automatically compressed. - Compression uses Sharp (images) and FFmpeg (videos) to maintain quality while meeting size limits. - Original files are preserved; compressed versions are uploaded to blob storage automatically. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**contentType** | [**ContentTypeEnum**](#ContentTypeEnum) | Set to &#39;story&#39; to publish as a Story. Default posts become Reels or feed depending on media. |  [optional] |
|**shareToFeed** | **Boolean** | For Reels only. When true (default), the Reel appears on both the Reels tab and your main profile feed. Set to false to post to the Reels tab only. |  [optional] |
|**collaborators** | **List&lt;String&gt;** | Up to 3 Instagram usernames to invite as collaborators (feed/Reels only) |  [optional] |
|**firstComment** | **String** | Optional first comment to add after the post is created (not applied to Stories) |  [optional] |
|**trialParams** | [**InstagramPlatformDataTrialParams**](InstagramPlatformDataTrialParams.md) |  |  [optional] |
|**userTags** | [**List&lt;InstagramPlatformDataUserTagsInner&gt;**](InstagramPlatformDataUserTagsInner.md) | Tag Instagram users in photos by username and position coordinates. Only works for single image posts and the first image of carousel posts. Not supported for stories or videos. |  [optional] |
|**audioName** | **String** | Custom name for the original audio in Reels. Replaces the default \&quot;Original Audio\&quot; label. Only applies to Reels (video posts). Can only be set once - either during creation or later from the Instagram audio page in the app.  |  [optional] |
|**thumbOffset** | **Integer** | Millisecond offset from the start of the video to use as the Reel thumbnail. Only applies to Reels (video posts). If a custom thumbnail URL (instagramThumbnail in mediaItems) is provided, it takes priority and this offset is ignored. Defaults to 0 (first frame).  |  [optional] |



## Enum: ContentTypeEnum

| Name | Value |
|---- | -----|
| STORY | &quot;story&quot; |



