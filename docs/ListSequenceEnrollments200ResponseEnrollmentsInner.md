

# ListSequenceEnrollments200ResponseEnrollmentsInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**contactId** | **String** |  |  [optional] |
|**channelId** | **String** |  |  [optional] |
|**platformIdentifier** | **String** |  |  [optional] |
|**contactName** | **String** |  |  [optional] |
|**currentStepIndex** | **Integer** |  |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) |  |  [optional] |
|**exitReason** | **String** |  |  [optional] |
|**nextStepAt** | **OffsetDateTime** |  |  [optional] |
|**stepsSent** | **Integer** |  |  [optional] |
|**lastStepSentAt** | **OffsetDateTime** |  |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| ACTIVE | &quot;active&quot; |
| COMPLETED | &quot;completed&quot; |
| EXITED | &quot;exited&quot; |
| PAUSED | &quot;paused&quot; |



