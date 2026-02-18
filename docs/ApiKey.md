

# ApiKey


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**name** | **String** |  |  [optional] |
|**keyPreview** | **String** |  |  [optional] |
|**expiresAt** | **OffsetDateTime** |  |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  [optional] |
|**key** | **String** | Returned only once, on creation |  [optional] |
|**scope** | [**ScopeEnum**](#ScopeEnum) | &#39;full&#39; grants access to all profiles, &#39;profiles&#39; restricts to specific profiles |  [optional] |
|**profileIds** | [**List&lt;ApiKeyProfileIdsInner&gt;**](ApiKeyProfileIdsInner.md) | Profiles this key can access (populated with name and color). Only present when scope is &#39;profiles&#39;. |  [optional] |
|**permission** | [**PermissionEnum**](#PermissionEnum) | &#39;read-write&#39; allows all operations, &#39;read&#39; restricts to GET requests only |  [optional] |



## Enum: ScopeEnum

| Name | Value |
|---- | -----|
| FULL | &quot;full&quot; |
| PROFILES | &quot;profiles&quot; |



## Enum: PermissionEnum

| Name | Value |
|---- | -----|
| READ_WRITE | &quot;read-write&quot; |
| READ | &quot;read&quot; |



