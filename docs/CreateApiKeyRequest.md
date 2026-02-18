

# CreateApiKeyRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**name** | **String** |  |  |
|**expiresIn** | **Integer** | Days until expiry |  [optional] |
|**scope** | [**ScopeEnum**](#ScopeEnum) | &#39;full&#39; grants access to all profiles (default), &#39;profiles&#39; restricts to specific profiles |  [optional] |
|**profileIds** | **List&lt;String&gt;** | Profile IDs this key can access. Required when scope is &#39;profiles&#39;. |  [optional] |
|**permission** | [**PermissionEnum**](#PermissionEnum) | &#39;read-write&#39; allows all operations (default), &#39;read&#39; restricts to GET requests only |  [optional] |



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



