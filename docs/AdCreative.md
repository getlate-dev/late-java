

# AdCreative

Platform-specific creative data. Fields vary by platform.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**thumbnailUrl** | **String** | Primary thumbnail/image URL |  [optional] |
|**imageUrl** | **String** | Alternative image URL |  [optional] |
|**videoId** | **String** | Meta video ID for VIDEO-type ads. Null for non-video ads. Callers that need an embeddable MP4 can call GET /{videoId}?fields&#x3D;source with the page access token. |  [optional] |
|**videoUrl** | **String** | Public Facebook watch URL for VIDEO-type ads (https://www.facebook.com/watch/?v&#x3D;{videoId}). Null for non-video ads. |  [optional] |
|**objectType** | **String** | Meta creative object_type (e.g. SHARE, VIDEO, PRIVACY_CHECK_FAIL, POST_DELETED). Use this to render state-aware previews — when Meta moderation strips image/video fields, only thumbnailUrl at 64x64 is available. |  [optional] |
|**mediaUrls** | **List&lt;String&gt;** | All media URLs for this ad (carousel images, multiple assets). Populated for Meta (carousel child_attachments), Google Ads (responsive display marketing_images), and LinkedIn (multi-image posts). |  [optional] |
|**body** | **String** | Ad copy/text |  [optional] |
|**googleHeadline** | **String** | Google Ads headline |  [optional] |
|**googleDescription** | **String** | Google Ads description |  [optional] |
|**linkUrl** | **String** | Destination URL |  [optional] |
|**pinterestImageUrl** | **String** |  |  [optional] |
|**pinterestTitle** | **String** |  |  [optional] |
|**pinterestDescription** | **String** |  |  [optional] |



