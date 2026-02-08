

# CreatePostRequestPlatformsInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**platform** | **String** |  |  [optional] |
|**accountId** | **String** |  |  [optional] |
|**customContent** | **String** | Platform-specific text override. When set, this content is used instead of the top-level post content for this platform. Useful for tailoring captions per platform (e.g. keeping tweets under 280 characters). |  [optional] |
|**customMedia** | [**List&lt;CreatePostRequestMediaItemsInner&gt;**](CreatePostRequestMediaItemsInner.md) |  |  [optional] |
|**scheduledFor** | **OffsetDateTime** | Optional per-platform scheduled time override. When omitted, the top-level scheduledFor is used. |  [optional] |
|**platformSpecificData** | [**CreatePostRequestPlatformsInnerPlatformSpecificData**](CreatePostRequestPlatformsInnerPlatformSpecificData.md) |  |  [optional] |



