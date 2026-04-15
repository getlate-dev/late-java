

# SendConversions200Response


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**platform** | [**PlatformEnum**](#PlatformEnum) |  |  [optional] |
|**eventsReceived** | **Integer** | Events accepted by the platform. |  [optional] |
|**eventsFailed** | **Integer** | Events rejected (see failures). |  [optional] |
|**failures** | [**List&lt;SendConversions200ResponseFailuresInner&gt;**](SendConversions200ResponseFailuresInner.md) |  |  [optional] |
|**traceId** | **String** | Platform trace ID (fbtrace_id for Meta, requestId for Google) for debugging. |  [optional] |



## Enum: PlatformEnum

| Name | Value |
|---- | -----|
| METAADS | &quot;metaads&quot; |
| GOOGLEADS | &quot;googleads&quot; |



