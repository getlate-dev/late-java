

# TwitterPlatformData


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**replySettings** | [**ReplySettingsEnum**](#ReplySettingsEnum) | Controls who can reply to the tweet. \&quot;following\&quot; allows only people you follow, \&quot;mentionedUsers\&quot; allows only mentioned users, \&quot;subscribers\&quot; allows only subscribers. Omit for default (everyone can reply). For threads, applies to the first tweet only. |  [optional] |
|**threadItems** | [**List&lt;TwitterPlatformDataThreadItemsInner&gt;**](TwitterPlatformDataThreadItemsInner.md) | Sequence of tweets in a thread. First item is the root tweet. |  [optional] |



## Enum: ReplySettingsEnum

| Name | Value |
|---- | -----|
| FOLLOWING | &quot;following&quot; |
| MENTIONED_USERS | &quot;mentionedUsers&quot; |
| SUBSCRIBERS | &quot;subscribers&quot; |



