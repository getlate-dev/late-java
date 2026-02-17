

# MediaItem

Media referenced in posts. URLs must be publicly reachable over HTTPS by the destination platforms. When using third-party storage, ensure signed links remain valid until upload completes.  **Uploading Media:** Use `POST /v1/media/presign` to get a presigned URL, then upload your file directly to cloud storage. Supports files up to 5GB. See the `/v1/media/presign` endpoint documentation for details.  **Automatic Media Compression:** Late automatically compresses images and videos that exceed platform limits. Compression happens server-side during publishing. Videos larger than 200 MB may not be compressed due to server timeout constraints. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**type** | [**TypeEnum**](#TypeEnum) |  |  [optional] |
|**url** | **URI** |  |  [optional] |
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



