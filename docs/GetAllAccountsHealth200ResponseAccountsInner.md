

# GetAllAccountsHealth200ResponseAccountsInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**accountId** | **String** |  |  [optional] |
|**platform** | **String** |  |  [optional] |
|**username** | **String** |  |  [optional] |
|**displayName** | **String** |  |  [optional] |
|**profileId** | **String** |  |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) |  |  [optional] |
|**canPost** | **Boolean** |  |  [optional] |
|**canFetchAnalytics** | **Boolean** |  |  [optional] |
|**tokenValid** | **Boolean** |  |  [optional] |
|**tokenExpiresAt** | **OffsetDateTime** |  |  [optional] |
|**needsReconnect** | **Boolean** |  |  [optional] |
|**issues** | **List&lt;String&gt;** |  |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| HEALTHY | &quot;healthy&quot; |
| WARNING | &quot;warning&quot; |
| ERROR | &quot;error&quot; |



