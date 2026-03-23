

# GetSequence200ResponseSequence


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**name** | **String** |  |  [optional] |
|**description** | **String** |  |  [optional] |
|**platform** | **String** |  |  [optional] |
|**accountId** | **String** |  |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) |  |  [optional] |
|**steps** | [**List&lt;GetSequence200ResponseSequenceStepsInner&gt;**](GetSequence200ResponseSequenceStepsInner.md) |  |  [optional] |
|**exitOnReply** | **Boolean** |  |  [optional] |
|**exitOnUnsubscribe** | **Boolean** |  |  [optional] |
|**totalEnrolled** | **Integer** |  |  [optional] |
|**totalCompleted** | **Integer** |  |  [optional] |
|**totalExited** | **Integer** |  |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  [optional] |
|**updatedAt** | **OffsetDateTime** |  |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| DRAFT | &quot;draft&quot; |
| ACTIVE | &quot;active&quot; |
| PAUSED | &quot;paused&quot; |



