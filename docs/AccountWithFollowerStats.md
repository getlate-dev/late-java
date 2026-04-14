

# AccountWithFollowerStats


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**platform** | [**PlatformEnum**](#PlatformEnum) |  |  [optional] |
|**profileId** | [**SocialAccountProfileId**](SocialAccountProfileId.md) |  |  [optional] |
|**username** | **String** |  |  [optional] |
|**displayName** | **String** |  |  [optional] |
|**profilePicture** | **String** | URL to the account&#39;s profile picture on the platform. May be null if the platform does not provide one. |  [optional] |
|**profileUrl** | **String** | Full profile URL for the connected account on its platform. |  [optional] |
|**isActive** | **Boolean** |  |  [optional] |
|**followersCount** | **BigDecimal** | Follower count (only included if user has analytics add-on) |  [optional] |
|**followersLastUpdated** | **OffsetDateTime** | Last time follower count was updated (only included if user has analytics add-on) |  [optional] |
|**parentAccountId** | **String** | Reference to the parent posting SocialAccount. Set for ads accounts that share or derive from a posting account&#39;s OAuth token. null for standalone ads (Google Ads) and all posting accounts.  |  [optional] |
|**enabled** | **Boolean** | Whether the user explicitly activated this account. false means the account was created as a side effect (e.g., posting account auto-created when user connected ads first). Posting UI and scheduler ignore accounts with enabled: false.  |  [optional] |
|**metadata** | **Object** | Platform-specific metadata. Fields vary by platform. For WhatsApp accounts, includes: - qualityRating: Phone number quality rating from Meta (GREEN, YELLOW, RED, or UNKNOWN) - nameStatus: Display name review status (APPROVED, PENDING_REVIEW, DECLINED, or NONE). Messages cannot be sent until the display name is approved by Meta. - messagingLimitTier: Maximum unique business-initiated conversations per 24h rolling window (TIER_250, TIER_1K, TIER_10K, TIER_100K, or TIER_UNLIMITED). Scales automatically as quality rating improves. - verifiedName: Meta-verified business display name - displayPhoneNumber: Formatted phone number (e.g., \&quot;+1 555-123-4567\&quot;) - wabaId: WhatsApp Business Account ID - phoneNumberId: Meta phone number ID  |  [optional] |
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
| DISCORD | &quot;discord&quot; |
| WHATSAPP | &quot;whatsapp&quot; |
| LINKEDINADS | &quot;linkedinads&quot; |
| METAADS | &quot;metaads&quot; |
| PINTERESTADS | &quot;pinterestads&quot; |
| TIKTOKADS | &quot;tiktokads&quot; |
| XADS | &quot;xads&quot; |
| GOOGLEADS | &quot;googleads&quot; |



