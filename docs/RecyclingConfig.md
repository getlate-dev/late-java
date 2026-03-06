

# RecyclingConfig

Configure automatic post recycling (reposting at regular intervals). After the post is published, the system creates new scheduled copies at the specified interval until expiration conditions are met. Supports weekly or monthly intervals. Maximum 10 active recycling posts per account. YouTube and TikTok platforms are excluded from recycling. Content variations are recommended for Twitter and Pinterest to avoid duplicate flags. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**enabled** | **Boolean** | Set to false to disable recycling on this post |  [optional] |
|**gap** | **Integer** | Number of interval units between each repost. Required when enabling recycling. |  [optional] |
|**gapFreq** | [**GapFreqEnum**](#GapFreqEnum) | Interval unit for the gap. Defaults to &#39;month&#39;. |  [optional] |
|**startDate** | **OffsetDateTime** | When to start the recycling cycle. Defaults to the post&#39;s scheduledFor date. |  [optional] |
|**expireCount** | **Integer** | Stop recycling after this many copies have been created |  [optional] |
|**expireDate** | **OffsetDateTime** | Stop recycling after this date, regardless of count |  [optional] |
|**contentVariations** | **List&lt;String&gt;** | Array of content variations for recycled copies. On each recycle, the next variation is used in round-robin order. Recommended for Twitter and Pinterest to avoid duplicate content flags. If omitted, the original post content is used for all recycled copies. Send an empty array [] to clear existing variations. Must have 2+ entries when setting variations. Platform-level customContent still overrides the base content per platform.  |  [optional] |



## Enum: GapFreqEnum

| Name | Value |
|---- | -----|
| WEEK | &quot;week&quot; |
| MONTH | &quot;month&quot; |



