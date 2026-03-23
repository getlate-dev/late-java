

# GetBroadcast200ResponseBroadcast


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**name** | **String** |  |  [optional] |
|**description** | **String** |  |  [optional] |
|**platform** | **String** |  |  [optional] |
|**accountId** | **String** |  |  [optional] |
|**message** | [**GetBroadcast200ResponseBroadcastMessage**](GetBroadcast200ResponseBroadcastMessage.md) |  |  [optional] |
|**template** | [**GetWhatsAppBroadcasts200ResponseBroadcastsInnerTemplate**](GetWhatsAppBroadcasts200ResponseBroadcastsInnerTemplate.md) |  |  [optional] |
|**segmentFilters** | [**GetBroadcast200ResponseBroadcastSegmentFilters**](GetBroadcast200ResponseBroadcastSegmentFilters.md) |  |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) |  |  [optional] |
|**scheduledAt** | **OffsetDateTime** |  |  [optional] |
|**startedAt** | **OffsetDateTime** |  |  [optional] |
|**completedAt** | **OffsetDateTime** |  |  [optional] |
|**recipientCount** | **Integer** |  |  [optional] |
|**sentCount** | **Integer** |  |  [optional] |
|**deliveredCount** | **Integer** |  |  [optional] |
|**readCount** | **Integer** |  |  [optional] |
|**failedCount** | **Integer** |  |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  [optional] |
|**updatedAt** | **OffsetDateTime** |  |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| DRAFT | &quot;draft&quot; |
| SCHEDULED | &quot;scheduled&quot; |
| SENDING | &quot;sending&quot; |
| COMPLETED | &quot;completed&quot; |
| FAILED | &quot;failed&quot; |
| CANCELLED | &quot;cancelled&quot; |



