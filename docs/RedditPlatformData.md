

# RedditPlatformData

Reddit post settings: - Posts are either \"link\" (with URL/media) or \"self\" (text-only) - If media is provided, the first media item's URL is used as the link - Use forceSelf to override and create a text post with the URL in the body - Subreddit defaults to the account's configured subreddit if omitted - Use the same accountId multiple times with different subreddit values in platformSpecificData to post to multiple subreddits - Images are automatically compressed if they exceed Reddit's 20MB limit 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**subreddit** | **String** | Target subreddit name (without \&quot;r/\&quot; prefix). Overrides the default subreddit configured on the account connection. Use GET /api/v1/accounts/{id}/reddit-subreddits to list available subreddits.  |  [optional] |
|**title** | **String** | Post title. Defaults to the first line of content, truncated to 300 characters. |  [optional] |
|**url** | **URI** | URL for link posts. If provided (and forceSelf is not true), creates a link post instead of a text post. |  [optional] |
|**forceSelf** | **Boolean** | When true, creates a text/self post even when a URL or media is provided. |  [optional] |



