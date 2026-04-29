

# TriggerAdsInitialSync202Response


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**status** | [**StatusEnum**](#StatusEnum) |  |  [optional] |
|**traceId** | **String** | Trace ID for the enqueued job. Reused on &#x60;already_queued&#x60;. |  [optional] |
|**message** | **String** |  |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| QUEUED | &quot;queued&quot; |
| ALREADY_QUEUED | &quot;already_queued&quot; |



