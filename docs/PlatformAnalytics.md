

# PlatformAnalytics


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**platform** | **String** |  |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) |  |  [optional] |
|**accountId** | **String** |  |  [optional] |
|**accountUsername** | **String** |  |  [optional] |
|**analytics** | [**PostAnalytics**](PostAnalytics.md) |  |  [optional] |
|**syncStatus** | [**SyncStatusEnum**](#SyncStatusEnum) | Sync state of analytics for this platform |  [optional] |
|**platformPostUrl** | **URI** |  |  [optional] |
|**errorMessage** | **String** | Error details when status is failed |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| PUBLISHED | &quot;published&quot; |
| FAILED | &quot;failed&quot; |



## Enum: SyncStatusEnum

| Name | Value |
|---- | -----|
| SYNCED | &quot;synced&quot; |
| PENDING | &quot;pending&quot; |
| UNAVAILABLE | &quot;unavailable&quot; |



