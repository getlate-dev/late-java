

# SocialAccount


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**platform** | **String** |  |  [optional] |
|**profileId** | [**SocialAccountProfileId**](SocialAccountProfileId.md) |  |  [optional] |
|**username** | **String** |  |  [optional] |
|**displayName** | **String** |  |  [optional] |
|**profileUrl** | **String** | Full profile URL for the connected account. Available for all platforms: - Twitter/X: https://x.com/{username} - Instagram: https://instagram.com/{username} - TikTok: https://tiktok.com/@{username} - YouTube: https://youtube.com/@{handle} or https://youtube.com/channel/{id} - LinkedIn Personal: https://www.linkedin.com/in/{vanityName}/ - LinkedIn Organization: https://www.linkedin.com/company/{vanityName}/ - Threads: https://threads.net/@{username} - Pinterest: https://pinterest.com/{username} - Reddit: https://reddit.com/user/{username} - Bluesky: https://bsky.app/profile/{handle} - Facebook: https://facebook.com/{username} or https://facebook.com/{pageId} - Google Business: Google Maps URL for the business location  |  [optional] |
|**isActive** | **Boolean** |  |  [optional] |
|**followersCount** | **BigDecimal** | Follower count (only included if user has analytics add-on) |  [optional] |
|**followersLastUpdated** | **OffsetDateTime** | Last time follower count was updated (only included if user has analytics add-on) |  [optional] |



