

# BlueskyPlatformData

Bluesky post settings. Supports text posts with up to 4 images or a single video. threadItems creates a reply chain (Bluesky thread). Images exceeding 1MB are automatically compressed. Alt text supported via mediaItem properties. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**threadItems** | [**List&lt;TwitterPlatformDataThreadItemsInner&gt;**](TwitterPlatformDataThreadItemsInner.md) | Complete sequence of posts in a Bluesky thread. The first item becomes the root post, subsequent items are chained as replies. When threadItems is provided, the top-level content field is used only for display and search purposes, it is NOT published. You must include your first post as threadItems[0].  |  [optional] |



