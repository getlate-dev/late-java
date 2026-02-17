

# SnapchatPlatformData

Snapchat requires a Public Profile. Media is required for all content types (single item only, auto-encrypted before upload).  **Content types:** Story (ephemeral 24h, no caption), Saved Story (permanent, title max 45 chars), Spotlight (video, description max 160 chars).  **Media limits:** Images max 20 MB (JPEG/PNG), videos max 500 MB (MP4, 5-60s, min 540x960px, 9:16 recommended). 

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



