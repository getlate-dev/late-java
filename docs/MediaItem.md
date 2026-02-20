

# MediaItem

Media referenced in posts. URLs must be publicly reachable over HTTPS. Use POST /v1/media/presign for uploads up to 5GB. Late auto-compresses images and videos that exceed platform limits (videos over 200 MB may not be compressed).

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**type** | [**TypeEnum**](#TypeEnum) |  |  [optional] |
|**url** | **URI** |  |  [optional] |
|**title** | **String** | Optional title for the media item. Used as the document title for LinkedIn PDF/carousel posts. If omitted, falls back to the post title, then the filename. |  [optional] |
|**filename** | **String** |  |  [optional] |
|**size** | **Integer** | Optional file size in bytes |  [optional] |
|**mimeType** | **String** | Optional MIME type (e.g. image/jpeg, video/mp4) |  [optional] |
|**thumbnail** | **URI** | Optional thumbnail image URL for videos |  [optional] |
|**instagramThumbnail** | **URI** | Optional custom cover image URL for Instagram Reels |  [optional] |
|**tiktokProcessed** | **Boolean** | Internal flag indicating the image was resized for TikTok |  [optional] |



## Enum: TypeEnum

| Name | Value |
|---- | -----|
| IMAGE | &quot;image&quot; |
| VIDEO | &quot;video&quot; |
| GIF | &quot;gif&quot; |
| DOCUMENT | &quot;document&quot; |



