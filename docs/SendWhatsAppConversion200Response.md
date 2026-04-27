

# SendWhatsAppConversion200Response


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**platform** | [**PlatformEnum**](#PlatformEnum) |  |  [optional] |
|**eventsReceived** | **Integer** | Events accepted by Meta. |  [optional] |
|**eventsFailed** | **Integer** | Events rejected by Meta (see failures). |  [optional] |
|**failures** | [**List&lt;SendConversions200ResponseFailuresInner&gt;**](SendConversions200ResponseFailuresInner.md) | Per-event failure detail. Empty when all events were accepted.  |  [optional] |
|**traceId** | **String** | Meta &#x60;fbtrace_id&#x60; for debugging. Surface in support tickets.  |  [optional] |



## Enum: PlatformEnum

| Name | Value |
|---- | -----|
| METAADS | &quot;metaads&quot; |



