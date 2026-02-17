

# PostLog

Publishing log entry showing details of a post publishing attempt

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**postId** | [**PostLogPostId**](PostLogPostId.md) |  |  [optional] |
|**userId** | **String** |  |  [optional] |
|**profileId** | **String** |  |  [optional] |
|**platform** | [**PlatformEnum**](#PlatformEnum) |  |  [optional] |
|**accountId** | **String** |  |  [optional] |
|**accountUsername** | **String** |  |  [optional] |
|**action** | [**ActionEnum**](#ActionEnum) | Type of action logged: publish (initial attempt), retry (after failure), media_upload, rate_limit_pause, token_refresh, cancelled |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) |  |  [optional] |
|**statusCode** | **Integer** | HTTP status code from platform API |  [optional] |
|**endpoint** | **String** | Platform API endpoint called |  [optional] |
|**request** | [**PostLogRequest**](PostLogRequest.md) |  |  [optional] |
|**response** | [**PostLogResponse**](PostLogResponse.md) |  |  [optional] |
|**durationMs** | **Integer** | How long the operation took in milliseconds |  [optional] |
|**attemptNumber** | **Integer** | Attempt number (1 for first try, 2+ for retries) |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  [optional] |



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



## Enum: ActionEnum

| Name | Value |
|---- | -----|
| PUBLISH | &quot;publish&quot; |
| RETRY | &quot;retry&quot; |
| MEDIA_UPLOAD | &quot;media_upload&quot; |
| RATE_LIMIT_PAUSE | &quot;rate_limit_pause&quot; |
| TOKEN_REFRESH | &quot;token_refresh&quot; |
| CANCELLED | &quot;cancelled&quot; |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| SUCCESS | &quot;success&quot; |
| FAILED | &quot;failed&quot; |
| PENDING | &quot;pending&quot; |
| SKIPPED | &quot;skipped&quot; |



