

# GetMediaPresignedUrlRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**filename** | **String** | Name of the file to upload |  |
|**contentType** | [**ContentTypeEnum**](#ContentTypeEnum) | MIME type of the file |  |
|**size** | **Integer** | Optional file size in bytes for pre-validation (max 5GB) |  [optional] |



## Enum: ContentTypeEnum

| Name | Value |
|---- | -----|
| IMAGE_JPEG | &quot;image/jpeg&quot; |
| IMAGE_JPG | &quot;image/jpg&quot; |
| IMAGE_PNG | &quot;image/png&quot; |
| IMAGE_WEBP | &quot;image/webp&quot; |
| IMAGE_GIF | &quot;image/gif&quot; |
| VIDEO_MP4 | &quot;video/mp4&quot; |
| VIDEO_MPEG | &quot;video/mpeg&quot; |
| VIDEO_QUICKTIME | &quot;video/quicktime&quot; |
| VIDEO_AVI | &quot;video/avi&quot; |
| VIDEO_X_MSVIDEO | &quot;video/x-msvideo&quot; |
| VIDEO_WEBM | &quot;video/webm&quot; |
| VIDEO_X_M4V | &quot;video/x-m4v&quot; |
| APPLICATION_PDF | &quot;application/pdf&quot; |



