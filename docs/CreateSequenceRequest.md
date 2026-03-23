

# CreateSequenceRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**profileId** | **String** |  |  |
|**accountId** | **String** |  |  |
|**platform** | [**PlatformEnum**](#PlatformEnum) |  |  |
|**name** | **String** |  |  |
|**description** | **String** |  |  [optional] |
|**steps** | [**List&lt;CreateSequenceRequestStepsInner&gt;**](CreateSequenceRequestStepsInner.md) |  |  [optional] |
|**exitOnReply** | **Boolean** |  |  [optional] |
|**exitOnUnsubscribe** | **Boolean** |  |  [optional] |



## Enum: PlatformEnum

| Name | Value |
|---- | -----|
| INSTAGRAM | &quot;instagram&quot; |
| FACEBOOK | &quot;facebook&quot; |
| TELEGRAM | &quot;telegram&quot; |
| TWITTER | &quot;twitter&quot; |
| BLUESKY | &quot;bluesky&quot; |
| REDDIT | &quot;reddit&quot; |
| WHATSAPP | &quot;whatsapp&quot; |



