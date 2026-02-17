

# CreatePostRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**title** | **String** |  |  [optional] |
|**content** | **String** | Post caption/text. Optional when media is attached or all platforms have customContent. Required for text-only posts. |  [optional] |
|**mediaItems** | [**List&lt;CreatePostRequestMediaItemsInner&gt;**](CreatePostRequestMediaItemsInner.md) |  |  [optional] |
|**platforms** | [**List&lt;CreatePostRequestPlatformsInner&gt;**](CreatePostRequestPlatformsInner.md) |  |  [optional] |
|**scheduledFor** | **OffsetDateTime** |  |  [optional] |
|**publishNow** | **Boolean** |  |  [optional] |
|**isDraft** | **Boolean** |  |  [optional] |
|**timezone** | **String** |  |  [optional] |
|**tags** | **List&lt;String&gt;** | Tags/keywords. YouTube constraints: each tag max 100 chars, combined max 500 chars, duplicates auto-removed. |  [optional] |
|**hashtags** | **List&lt;String&gt;** |  |  [optional] |
|**mentions** | **List&lt;String&gt;** |  |  [optional] |
|**crosspostingEnabled** | **Boolean** |  |  [optional] |
|**metadata** | **Map&lt;String, Object&gt;** |  |  [optional] |
|**tiktokSettings** | [**TikTokPlatformData**](TikTokPlatformData.md) | Root-level TikTok settings applied to all TikTok platforms. Merged into each platform&#39;s platformSpecificData, with platform-specific settings taking precedence. |  [optional] |
|**queuedFromProfile** | **String** | Profile ID to schedule via queue. When provided without scheduledFor, the post is auto-assigned to the next available slot. Do not call /v1/queue/next-slot and use that time in scheduledFor, as that bypasses queue locking. |  [optional] |
|**queueId** | **String** | Specific queue ID to use when scheduling via queue. Only used when queuedFromProfile is also provided. If omitted, uses the profile&#39;s default queue.  |  [optional] |



