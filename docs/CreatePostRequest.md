

# CreatePostRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**title** | **String** |  |  [optional] |
|**content** | **String** | Post caption/text content. Optional when media is attached (images, videos, etc.). Required for text-only posts. Can also be omitted if all platforms have customContent set.  |  [optional] |
|**mediaItems** | [**List&lt;CreatePostRequestMediaItemsInner&gt;**](CreatePostRequestMediaItemsInner.md) |  |  [optional] |
|**platforms** | [**List&lt;CreatePostRequestPlatformsInner&gt;**](CreatePostRequestPlatformsInner.md) |  |  [optional] |
|**scheduledFor** | **OffsetDateTime** |  |  [optional] |
|**publishNow** | **Boolean** |  |  [optional] |
|**isDraft** | **Boolean** |  |  [optional] |
|**timezone** | **String** |  |  [optional] |
|**tags** | **List&lt;String&gt;** | Tags/keywords for the post. YouTube-specific constraints: - No count limit; duplicates are automatically removed - Each tag must be ≤ 100 characters - Combined total across all tags ≤ 500 characters (YouTube&#39;s limit)  |  [optional] |
|**hashtags** | **List&lt;String&gt;** |  |  [optional] |
|**mentions** | **List&lt;String&gt;** |  |  [optional] |
|**crosspostingEnabled** | **Boolean** |  |  [optional] |
|**metadata** | **Map&lt;String, Object&gt;** |  |  [optional] |
|**tiktokSettings** | [**TikTokPlatformData**](TikTokPlatformData.md) | Root-level TikTok settings applied to all TikTok platforms in the request. This is a convenience shorthand. Settings here are merged into each TikTok platform&#39;s platformSpecificData, with platform-specific settings taking precedence.  |  [optional] |
|**queuedFromProfile** | **String** | Profile ID to schedule via queue.  When provided (without &#x60;scheduledFor&#x60;), the post will be automatically assigned to the next available slot from the profile&#39;s queue. The system uses distributed locking to prevent race conditions when multiple posts are scheduled concurrently. Do not call &#x60;/v1/queue/next-slot&#x60; and then use that time in &#x60;scheduledFor&#x60;. That bypasses the queue system and can cause duplicate slot assignments.  |  [optional] |
|**queueId** | **String** | Specific queue ID to use when scheduling via queue. Only used when queuedFromProfile is also provided. If omitted, uses the profile&#39;s default queue.  |  [optional] |



