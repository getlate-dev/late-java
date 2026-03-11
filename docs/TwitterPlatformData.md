

# TwitterPlatformData


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**replyToTweetId** | **String** | ID of an existing tweet to reply to. The published tweet will appear as a reply in that tweet&#39;s thread. For threads, only the first tweet replies to the target; subsequent tweets chain normally. |  [optional] |
|**replySettings** | [**ReplySettingsEnum**](#ReplySettingsEnum) | Controls who can reply to the tweet. \&quot;following\&quot; allows only people you follow, \&quot;mentionedUsers\&quot; allows only mentioned users, \&quot;subscribers\&quot; allows only subscribers, \&quot;verified\&quot; allows only verified users. Omit for default (everyone can reply). For threads, applies to the first tweet only. Cannot be combined with replyToTweetId. |  [optional] |
|**threadItems** | [**List&lt;TwitterPlatformDataThreadItemsInner&gt;**](TwitterPlatformDataThreadItemsInner.md) | Sequence of tweets in a thread. First item is the root tweet. |  [optional] |



## Enum: ReplySettingsEnum

| Name | Value |
|---- | -----|
| FOLLOWING | &quot;following&quot; |
| MENTIONED_USERS | &quot;mentionedUsers&quot; |
| SUBSCRIBERS | &quot;subscribers&quot; |
| VERIFIED | &quot;verified&quot; |



