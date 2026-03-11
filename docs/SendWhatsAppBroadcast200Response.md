

# SendWhatsAppBroadcast200Response


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**success** | **Boolean** |  |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) | Final broadcast status |  [optional] |
|**sent** | **Integer** | Number of messages sent successfully |  [optional] |
|**failed** | **Integer** | Number of messages that failed |  [optional] |
|**total** | **Integer** | Total recipient count |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| COMPLETED | &quot;completed&quot; |
| FAILED | &quot;failed&quot; |



