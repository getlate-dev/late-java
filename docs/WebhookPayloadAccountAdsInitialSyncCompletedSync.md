

# WebhookPayloadAccountAdsInitialSyncCompletedSync

Summary of the initial ads sync backfill results.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**status** | [**StatusEnum**](#StatusEnum) | Overall outcome of the initial sync. |  |
|**totalAds** | **Integer** | Total number of ads discovered for backfill. |  |
|**synced** | **Integer** | Number of ads successfully synced. |  |
|**failed** | **Integer** | Number of ads that failed to sync. |  |
|**error** | **String** | Free-form error message from the platform (typically Meta&#39;s Marketing API). Truncated to ~2KB. Present when &#x60;status&#x60; is &#x60;failure&#x60; (and sometimes on &#x60;success&#x60; when discovery saw zero ad accounts). For UX branching prefer &#x60;errorCategory&#x60;; this field is for human display and debugging.  |  [optional] |
|**errorCode** | **String** | Platform-native error code if parsed (e.g. Meta &#x60;190&#x60;, &#x60;10&#x60;, &#x60;200&#x60;). |  [optional] |
|**errorSubcode** | **String** | Platform-native error subcode if parsed. |  [optional] |
|**errorCategory** | [**ErrorCategoryEnum**](#ErrorCategoryEnum) | Stable category for UX branching. New values may be added; existing ones are stable. Mapping:   - &#x60;token_invalid&#x60;: access token is expired or revoked. Reconnect.   - &#x60;permission_denied&#x60;: token lacks required scope, or the user has no role     on the Business Manager that owns the ad account. Reconnect with full     permissions, or have an admin grant access.   - &#x60;no_ad_accounts&#x60;: token is valid but sees zero ad accounts. The user     needs to connect a Business Manager that owns ad accounts.   - &#x60;rate_limited&#x60;: platform throttled us. Sync will retry automatically.   - &#x60;discovery_failed&#x60;: any other platform-side failure. Inspect &#x60;error&#x60;.   - &#x60;unknown&#x60;: classifier could not categorize the failure.  |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| SUCCESS | &quot;success&quot; |
| FAILURE | &quot;failure&quot; |



## Enum: ErrorCategoryEnum

| Name | Value |
|---- | -----|
| TOKEN_INVALID | &quot;token_invalid&quot; |
| PERMISSION_DENIED | &quot;permission_denied&quot; |
| NO_AD_ACCOUNTS | &quot;no_ad_accounts&quot; |
| RATE_LIMITED | &quot;rate_limited&quot; |
| DISCOVERY_FAILED | &quot;discovery_failed&quot; |
| UNKNOWN | &quot;unknown&quot; |



