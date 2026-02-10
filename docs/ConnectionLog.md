

# ConnectionLog

Connection event log showing account connection/disconnection history

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**userId** | **String** | User who owns the connection (may be null for early OAuth failures) |  [optional] |
|**profileId** | **String** |  |  [optional] |
|**accountId** | **String** | The social account ID (present on successful connections and disconnects) |  [optional] |
|**platform** | [**PlatformEnum**](#PlatformEnum) |  |  [optional] |
|**eventType** | [**EventTypeEnum**](#EventTypeEnum) | Type of connection event: - &#x60;connect_success&#x60; - New account connected successfully - &#x60;connect_failed&#x60; - Connection attempt failed - &#x60;disconnect&#x60; - Account was disconnected - &#x60;reconnect_success&#x60; - Existing account reconnected successfully - &#x60;reconnect_failed&#x60; - Reconnection attempt failed  |  [optional] |
|**connectionMethod** | [**ConnectionMethodEnum**](#ConnectionMethodEnum) | How the connection was initiated |  [optional] |
|**error** | [**ConnectionLogError**](ConnectionLogError.md) |  |  [optional] |
|**success** | [**ConnectionLogSuccess**](ConnectionLogSuccess.md) |  |  [optional] |
|**context** | [**ConnectionLogContext**](ConnectionLogContext.md) |  |  [optional] |
|**durationMs** | **Integer** | How long the operation took in milliseconds |  [optional] |
|**metadata** | **Object** | Additional metadata |  [optional] |
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



## Enum: EventTypeEnum

| Name | Value |
|---- | -----|
| CONNECT_SUCCESS | &quot;connect_success&quot; |
| CONNECT_FAILED | &quot;connect_failed&quot; |
| DISCONNECT | &quot;disconnect&quot; |
| RECONNECT_SUCCESS | &quot;reconnect_success&quot; |
| RECONNECT_FAILED | &quot;reconnect_failed&quot; |



## Enum: ConnectionMethodEnum

| Name | Value |
|---- | -----|
| OAUTH | &quot;oauth&quot; |
| CREDENTIALS | &quot;credentials&quot; |
| INVITATION | &quot;invitation&quot; |



