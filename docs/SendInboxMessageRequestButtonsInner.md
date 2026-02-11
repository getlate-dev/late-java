

# SendInboxMessageRequestButtonsInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**type** | [**TypeEnum**](#TypeEnum) | Button type. phone is Facebook only. |  |
|**title** | **String** | Button label (max 20 chars) |  |
|**url** | **String** | URL for url-type buttons |  [optional] |
|**payload** | **String** | Payload for postback-type buttons |  [optional] |
|**phone** | **String** | Phone number for phone-type buttons (Facebook only) |  [optional] |



## Enum: TypeEnum

| Name | Value |
|---- | -----|
| URL | &quot;url&quot; |
| POSTBACK | &quot;postback&quot; |
| PHONE | &quot;phone&quot; |



