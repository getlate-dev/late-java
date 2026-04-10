

# AccountWithFollowerStats


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**platform** | [**PlatformEnum**](#PlatformEnum) |  |  [optional] |
|**profileId** | [**SocialAccountProfileId**](SocialAccountProfileId.md) |  |  [optional] |
|**username** | **String** |  |  [optional] |
|**displayName** | **String** |  |  [optional] |
|**profileUrl** | **String** | Full profile URL for the connected account on its platform. |  [optional] |
|**isActive** | **Boolean** |  |  [optional] |
|**followersCount** | **BigDecimal** | Follower count (only included if user has analytics add-on) |  [optional] |
|**followersLastUpdated** | **OffsetDateTime** | Last time follower count was updated (only included if user has analytics add-on) |  [optional] |
|**parentAccountId** | **String** | Reference to the parent posting SocialAccount. Set for ads accounts that share or derive from a posting account&#39;s OAuth token. null for standalone ads (Google Ads) and all posting accounts.  |  [optional] |
|**enabled** | **Boolean** | Whether the user explicitly activated this account. false means the account was created as a side effect (e.g., posting account auto-created when user connected ads first). Posting UI and scheduler ignore accounts with enabled: false.  |  [optional] |
|**adsStatus** | [**AdsStatusEnum**](#AdsStatusEnum) | **Deprecated.** With the new ads account model, ads accounts are separate SocialAccount documents. Check for accounts with ads platform values (metaads, linkedinads, pinterestads, tiktokads, xads, googleads) instead.  Legacy behavior: - &#x60;connected&#x60;: Ads are ready to use (same-token platforms like Meta/LinkedIn, or separate ads token is present). - &#x60;not_connected&#x60;: Platform supports ads but requires a separate ads OAuth. Use &#x60;GET /v1/connect/{platform}/ads&#x60; to connect. - &#x60;not_available&#x60;: Platform does not support ads (e.g., YouTube, Reddit, Bluesky).  |  [optional] |
|**metadata** | **Object** | Platform-specific metadata. Fields vary by platform. For WhatsApp accounts, includes: - &#x60;qualityRating&#x60;: Phone number quality rating from Meta (&#x60;GREEN&#x60;, &#x60;YELLOW&#x60;, &#x60;RED&#x60;, or &#x60;UNKNOWN&#x60;) - &#x60;nameStatus&#x60;: Display name review status (&#x60;APPROVED&#x60;, &#x60;PENDING_REVIEW&#x60;, &#x60;DECLINED&#x60;, or &#x60;NONE&#x60;). Messages cannot be sent until the display name is approved by Meta. - &#x60;messagingLimitTier&#x60;: Maximum unique business-initiated conversations per 24h rolling window (&#x60;TIER_250&#x60;, &#x60;TIER_1K&#x60;, &#x60;TIER_10K&#x60;, &#x60;TIER_100K&#x60;, or &#x60;TIER_UNLIMITED&#x60;). Scales automatically as quality rating improves. - &#x60;verifiedName&#x60;: Meta-verified business display name - &#x60;displayPhoneNumber&#x60;: Formatted phone number (e.g., \&quot;+1 555-123-4567\&quot;) - &#x60;wabaId&#x60;: WhatsApp Business Account ID - &#x60;phoneNumberId&#x60;: Meta phone number ID  |  [optional] |
|**profilePicture** | **String** |  |  [optional] |
|**currentFollowers** | **BigDecimal** | Current follower count |  [optional] |
|**lastUpdated** | **OffsetDateTime** |  |  [optional] |
|**growth** | **BigDecimal** | Follower change over period |  [optional] |
|**growthPercentage** | **BigDecimal** | Percentage growth |  [optional] |
|**dataPoints** | **BigDecimal** | Number of historical snapshots |  [optional] |
|**accountStats** | [**AccountWithFollowerStatsAllOfAccountStats**](AccountWithFollowerStatsAllOfAccountStats.md) |  |  [optional] |



## Enum: PlatformEnum

| Name | Value |
|---- | -----|
| TIKTOK | &quot;tiktok&quot; |
| INSTAGRAM | &quot;instagram&quot; |
| FACEBOOK | &quot;facebook&quot; |
| YOUTUBE | &quot;youtube&quot; |
| LINKEDIN | &quot;linkedin&quot; |
| TWITTER | &quot;twitter&quot; |
| THREADS | &quot;threads&quot; |
| PINTEREST | &quot;pinterest&quot; |
| REDDIT | &quot;reddit&quot; |
| BLUESKY | &quot;bluesky&quot; |
| GOOGLEBUSINESS | &quot;googlebusiness&quot; |
| TELEGRAM | &quot;telegram&quot; |
| SNAPCHAT | &quot;snapchat&quot; |
| WHATSAPP | &quot;whatsapp&quot; |
| LINKEDINADS | &quot;linkedinads&quot; |
| METAADS | &quot;metaads&quot; |
| PINTERESTADS | &quot;pinterestads&quot; |
| TIKTOKADS | &quot;tiktokads&quot; |
| XADS | &quot;xads&quot; |
| GOOGLEADS | &quot;googleads&quot; |



## Enum: AdsStatusEnum

| Name | Value |
|---- | -----|
| CONNECTED | &quot;connected&quot; |
| NOT_CONNECTED | &quot;not_connected&quot; |
| NOT_AVAILABLE | &quot;not_available&quot; |



