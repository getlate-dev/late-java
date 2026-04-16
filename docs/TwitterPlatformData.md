

# TwitterPlatformData

X (Twitter) geo-restriction applies at the media level. Media in geo-restricted tweets will be hidden for users outside the specified countries; the tweet text itself remains visible globally. Requires media to be attached (ignored for text-only tweets). 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**replyToTweetId** | **String** | ID of an existing tweet to reply to. The published tweet will appear as a reply in that tweet&#39;s thread. For threads, only the first tweet replies to the target; subsequent tweets chain normally. |  [optional] |
|**replySettings** | [**ReplySettingsEnum**](#ReplySettingsEnum) | Controls who can reply to the tweet. \&quot;following\&quot; allows only people you follow, \&quot;mentionedUsers\&quot; allows only mentioned users, \&quot;subscribers\&quot; allows only subscribers, \&quot;verified\&quot; allows only verified users. Omit for default (everyone can reply). For threads, applies to the first tweet only. Cannot be combined with replyToTweetId. |  [optional] |
|**threadItems** | [**List&lt;TwitterPlatformDataThreadItemsInner&gt;**](TwitterPlatformDataThreadItemsInner.md) | Complete sequence of tweets in a thread. The first item becomes the root tweet, subsequent items are chained as replies. When threadItems is provided, the top-level content field is used only for display and search purposes, it is NOT published. You must include your first tweet as threadItems[0].  |  [optional] |
|**poll** | [**TwitterPlatformDataPoll**](TwitterPlatformDataPoll.md) |  |  [optional] |
|**longVideo** | **Boolean** | Enable long video uploads (over 140 seconds) using amplify_video media category. Requires the connected X account to have an active X Premium subscription. When true, videos are uploaded with the amplify_video category which supports longer durations (up to 10 minutes via API). When false or omitted, the standard tweet_video category is used (140 second limit). Note that not all Premium accounts have API long-video access, as X may require separate allowlisting. |  [optional] |
|**geoRestriction** | [**GeoRestriction**](GeoRestriction.md) |  |  [optional] |



## Enum: ReplySettingsEnum

| Name | Value |
|---- | -----|
| FOLLOWING | &quot;following&quot; |
| MENTIONED_USERS | &quot;mentionedUsers&quot; |
| SUBSCRIBERS | &quot;subscribers&quot; |
| VERIFIED | &quot;verified&quot; |



