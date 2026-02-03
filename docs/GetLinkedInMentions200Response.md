

# GetLinkedInMentions200Response


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**urn** | **String** | The LinkedIn URN (person or organization) |  [optional] |
|**type** | [**TypeEnum**](#TypeEnum) | The type of entity (person or organization) |  [optional] |
|**displayName** | **String** | Display name (provided, from API, or derived from vanity URL) |  [optional] |
|**mentionFormat** | **String** | Ready-to-use mention format for post content |  [optional] |
|**vanityName** | **String** | The vanity name/slug (only for organization mentions) |  [optional] |
|**warning** | **String** | Warning about clickable mentions (only present for person mentions if displayName was not provided) |  [optional] |



## Enum: TypeEnum

| Name | Value |
|---- | -----|
| PERSON | &quot;person&quot; |
| ORGANIZATION | &quot;organization&quot; |



