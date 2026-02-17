

# FacebookPlatformData

Up to 10 images for feed posts, cannot mix videos and images. Stories require single image or video (ephemeral 24h, no captions). Use pageId for multi-page posting.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**contentType** | [**ContentTypeEnum**](#ContentTypeEnum) | Set to &#39;story&#39; to publish as a Facebook Page Story (24-hour ephemeral content). Requires media. |  [optional] |
|**firstComment** | **String** | Optional first comment to post immediately after publishing (feed posts only, not stories) |  [optional] |
|**pageId** | **String** | Target Facebook Page ID for multi-page posting. If omitted, uses the default page. Use GET /v1/accounts/{id}/facebook-page to list pages. |  [optional] |



## Enum: ContentTypeEnum

| Name | Value |
|---- | -----|
| STORY | &quot;story&quot; |



