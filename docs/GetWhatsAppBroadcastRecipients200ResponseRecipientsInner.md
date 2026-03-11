

# GetWhatsAppBroadcastRecipients200ResponseRecipientsInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**phone** | **String** |  |  [optional] |
|**name** | **String** |  |  [optional] |
|**variables** | **Object** |  |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) |  |  [optional] |
|**messageId** | **String** |  |  [optional] |
|**error** | **String** |  |  [optional] |
|**sentAt** | **OffsetDateTime** |  |  [optional] |
|**deliveredAt** | **OffsetDateTime** |  |  [optional] |
|**readAt** | **OffsetDateTime** |  |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| PENDING | &quot;pending&quot; |
| SENT | &quot;sent&quot; |
| DELIVERED | &quot;delivered&quot; |
| READ | &quot;read&quot; |
| FAILED | &quot;failed&quot; |



