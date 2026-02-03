

# SnapchatPlatformData

Snapchat Public Profile API constraints:  **General Requirements:** - Snapchat requires a Public Profile to publish content - Media is required for all content types (no text-only posts) - Only one media item per post is supported - Media is automatically encrypted using AES-256-CBC before upload  **Content Types:** - **Story** (default): Ephemeral content visible for 24 hours. No caption/text supported. - **Saved Story**: Permanent story on your Public Profile. Uses post content as title (max 45 chars). - **Spotlight**: Video content for Snapchat's entertainment feed. Supports description (max 160 chars) with hashtags.  **Media Constraints:** - Images: max 20 MB, JPEG/PNG format - Videos: max 500 MB, MP4 format, 5-60 seconds duration, minimum 540x960px resolution - Aspect ratio: 9:16 recommended  **Analytics:** - Views, screenshots, shares, unique viewers, completion rate available - Analytics are fetched per content type (story/saved_story/spotlight) 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**contentType** | [**ContentTypeEnum**](#ContentTypeEnum) | Type of Snapchat content to publish: - &#x60;story&#x60; - Ephemeral snap visible for 24 hours (default) - &#x60;saved_story&#x60; - Permanent story saved to Public Profile - &#x60;spotlight&#x60; - Video posted to Spotlight (Snapchat&#39;s TikTok-like feed)  |  [optional] |



## Enum: ContentTypeEnum

| Name | Value |
|---- | -----|
| STORY | &quot;story&quot; |
| SAVED_STORY | &quot;saved_story&quot; |
| SPOTLIGHT | &quot;spotlight&quot; |



