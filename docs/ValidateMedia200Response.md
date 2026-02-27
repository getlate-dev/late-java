

# ValidateMedia200Response


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**valid** | **Boolean** |  |  [optional] |
|**url** | **URI** |  |  [optional] |
|**error** | **String** | Error message if valid is false |  [optional] |
|**contentType** | **String** |  |  [optional] |
|**size** | **Integer** | File size in bytes |  [optional] |
|**sizeFormatted** | **String** |  |  [optional] |
|**type** | [**TypeEnum**](#TypeEnum) |  |  [optional] |
|**platformLimits** | [**Map&lt;String, ValidateMedia200ResponsePlatformLimitsValue&gt;**](ValidateMedia200ResponsePlatformLimitsValue.md) | Per-platform size limit comparison (only present when size and type are known) |  [optional] |



## Enum: TypeEnum

| Name | Value |
|---- | -----|
| IMAGE | &quot;image&quot; |
| VIDEO | &quot;video&quot; |
| UNKNOWN | &quot;unknown&quot; |



