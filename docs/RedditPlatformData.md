

# RedditPlatformData

Posts are either link (with URL/media) or self (text-only). If media is provided, the first item URL is used as the link; use forceSelf to override. Subreddit defaults to the account's configured one. Images over 20 MB are auto-compressed. Some subreddits require a flair; if missing, the first available flair is used as fallback.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**subreddit** | **String** | Target subreddit name (without \&quot;r/\&quot; prefix). Overrides the default subreddit configured on the account connection. Use GET /api/v1/accounts/{id}/reddit-subreddits to list available subreddits.  |  [optional] |
|**title** | **String** | Post title. Defaults to the first line of content, truncated to 300 characters. |  [optional] |
|**url** | **URI** | URL for link posts. If provided (and forceSelf is not true), creates a link post instead of a text post. |  [optional] |
|**forceSelf** | **Boolean** | When true, creates a text/self post even when a URL or media is provided. |  [optional] |
|**flairId** | **String** | Flair ID for the post. Required by some subreddits. Use GET /api/v1/accounts/{id}/reddit-flairs?subreddit&#x3D;name to list available flairs.  |  [optional] |



