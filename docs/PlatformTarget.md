

# PlatformTarget


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**platform** | **String** | Supported values: twitter, threads, instagram, youtube, facebook, linkedin, pinterest, reddit, tiktok, bluesky, googlebusiness, telegram |  [optional] |
|**accountId** | [**PlatformTargetAccountId**](PlatformTargetAccountId.md) |  |  [optional] |
|**customContent** | **String** | Platform-specific text override. When set, this content is used instead of the top-level post content for this platform. Useful for tailoring captions per platform (e.g. keeping tweets under 280 characters). |  [optional] |
|**customMedia** | [**List&lt;MediaItem&gt;**](MediaItem.md) |  |  [optional] |
|**scheduledFor** | **OffsetDateTime** | Optional per-platform scheduled time override (uses post.scheduledFor when omitted) |  [optional] |
|**platformSpecificData** | [**PlatformTargetPlatformSpecificData**](PlatformTargetPlatformSpecificData.md) |  |  [optional] |
|**status** | **String** | Platform-specific status: pending, publishing, published, failed |  [optional] |
|**platformPostId** | **String** | The native post ID on the platform (populated after successful publish) |  [optional] |
|**platformPostUrl** | **URI** | Public URL of the published post on the platform. Populated after successful publish. For immediate posts (publishNow&#x3D;true),  this is included in the response. For scheduled posts, fetch the post  via GET /v1/posts/{postId} after the scheduled time.  |  [optional] |
|**publishedAt** | **OffsetDateTime** | Timestamp when the post was published to this platform |  [optional] |
|**errorMessage** | **String** | Human-readable error message when status is &#39;failed&#39;. Contains platform-specific error details explaining why the publish failed. Examples: - \&quot;Instagram access token has expired. Please reconnect your account.\&quot; - \&quot;Post text exceeds the 500 character limit for Threads.\&quot; - \&quot;You do not have enough karma to post in this subreddit.\&quot; - \&quot;Video is too long for Reels. Facebook Reels must be 90 seconds or less.\&quot;  |  [optional] |
|**errorCategory** | [**ErrorCategoryEnum**](#ErrorCategoryEnum) | Error category for programmatic handling: - auth_expired: Token expired or revoked, account needs reconnection - user_content: Content doesn&#39;t meet platform requirements (too long, wrong format, etc.) - user_abuse: Rate limits, spam detection, excessive posting - account_issue: Account configuration problems (missing board, inactive account) - platform_rejected: Platform rules violated (banned, suspended, policy violation) - platform_error: Platform-side issues (5xx errors, maintenance) - system_error: Late infrastructure issues (timeouts, network errors) - unknown: Unclassified error  |  [optional] |
|**errorSource** | [**ErrorSourceEnum**](#ErrorSourceEnum) | Who/what caused the error: - user: User action required (fix content, reconnect account) - platform: Platform-side issue (outage, API change) - system: Late system issue (rare)  |  [optional] |



## Enum: ErrorCategoryEnum

| Name | Value |
|---- | -----|
| AUTH_EXPIRED | &quot;auth_expired&quot; |
| USER_CONTENT | &quot;user_content&quot; |
| USER_ABUSE | &quot;user_abuse&quot; |
| ACCOUNT_ISSUE | &quot;account_issue&quot; |
| PLATFORM_REJECTED | &quot;platform_rejected&quot; |
| PLATFORM_ERROR | &quot;platform_error&quot; |
| SYSTEM_ERROR | &quot;system_error&quot; |
| UNKNOWN | &quot;unknown&quot; |



## Enum: ErrorSourceEnum

| Name | Value |
|---- | -----|
| USER | &quot;user&quot; |
| PLATFORM | &quot;platform&quot; |
| SYSTEM | &quot;system&quot; |



