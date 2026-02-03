

# CreateInviteTokenRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**scope** | [**ScopeEnum**](#ScopeEnum) | &#39;all&#39; grants access to all profiles, &#39;profiles&#39; restricts to specific profiles |  |
|**profileIds** | **List&lt;String&gt;** | Required if scope is &#39;profiles&#39;. Array of profile IDs to grant access to. |  [optional] |



## Enum: ScopeEnum

| Name | Value |
|---- | -----|
| ALL | &quot;all&quot; |
| PROFILES | &quot;profiles&quot; |



