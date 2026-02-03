

# QueueSchedule


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** | Unique queue identifier |  [optional] |
|**profileId** | **String** | Profile ID this queue belongs to |  [optional] |
|**name** | **String** | Queue name (e.g., \&quot;Morning Posts\&quot;, \&quot;Evening Content\&quot;) |  [optional] |
|**timezone** | **String** | IANA timezone (e.g., America/New_York) |  [optional] |
|**slots** | [**List&lt;QueueSlot&gt;**](QueueSlot.md) |  |  [optional] |
|**active** | **Boolean** | Whether the queue is active |  [optional] |
|**isDefault** | **Boolean** | Whether this is the default queue for the profile (used when no queueId specified) |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  [optional] |
|**updatedAt** | **OffsetDateTime** |  |  [optional] |



