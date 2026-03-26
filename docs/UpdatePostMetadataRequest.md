

# UpdatePostMetadataRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**platform** | [**PlatformEnum**](#PlatformEnum) | The platform to update metadata on |  |
|**videoId** | **String** | YouTube video ID (required for direct mode, ignored for post-based mode) |  [optional] |
|**accountId** | **String** | Zernio social account ID (required for direct mode, ignored for post-based mode) |  [optional] |
|**title** | **String** | New video title (max 100 characters for YouTube) |  [optional] |
|**description** | **String** | New video description |  [optional] |
|**tags** | **List&lt;String&gt;** | Array of keyword tags (max 500 characters combined for YouTube) |  [optional] |
|**categoryId** | **String** | YouTube video category ID |  [optional] |
|**privacyStatus** | [**PrivacyStatusEnum**](#PrivacyStatusEnum) | Video privacy setting |  [optional] |



## Enum: PlatformEnum

| Name | Value |
|---- | -----|
| YOUTUBE | &quot;youtube&quot; |



## Enum: PrivacyStatusEnum

| Name | Value |
|---- | -----|
| PUBLIC | &quot;public&quot; |
| PRIVATE | &quot;private&quot; |
| UNLISTED | &quot;unlisted&quot; |



