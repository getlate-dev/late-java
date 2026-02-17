

# RedditPlatformData

Posts are either link (with URL/media) or self (text-only). Use forceSelf to override. Subreddit defaults to the account's configured one. Some subreddits require a flair.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**subreddit** | **String** | Target subreddit name (without \&quot;r/\&quot; prefix). Overrides the default. Use GET /v1/accounts/{id}/reddit-subreddits to list options. |  [optional] |
|**title** | **String** | Post title. Defaults to the first line of content, truncated to 300 characters. |  [optional] |
|**url** | **URI** | URL for link posts. If provided (and forceSelf is not true), creates a link post instead of a text post. |  [optional] |
|**forceSelf** | **Boolean** | When true, creates a text/self post even when a URL or media is provided. |  [optional] |
|**flairId** | **String** | Flair ID for the post. Required by some subreddits. Use GET /v1/accounts/{id}/reddit-flairs?subreddit&#x3D;name to list flairs. |  [optional] |



