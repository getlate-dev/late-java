

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
|**platformPostUrl** | **URI** | Public URL of the published post. Included in the response for immediate posts; for scheduled posts, fetch via GET /v1/posts/{postId} after publish time. |  [optional] |
|**publishedAt** | **OffsetDateTime** | Timestamp when the post was published to this platform |  [optional] |
|**errorMessage** | **String** | Human-readable error message when status is failed. Contains platform-specific error details explaining why the publish failed. |  [optional] |
|**errorCategory** | [**ErrorCategoryEnum**](#ErrorCategoryEnum) | Error category for programmatic handling: auth_expired (token expired/revoked), user_content (wrong format/too long), user_abuse (rate limits/spam), account_issue (config problems), platform_rejected (policy violation), platform_error (5xx/maintenance), system_error (Late infra), unknown |  [optional] |
|**errorSource** | [**ErrorSourceEnum**](#ErrorSourceEnum) | Who caused the error: user (fix content/reconnect), platform (outage/API change), system (Late issue, rare) |  [optional] |



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



