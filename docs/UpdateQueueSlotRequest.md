

# UpdateQueueSlotRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**profileId** | **String** |  |  |
|**queueId** | **String** | Queue ID to update (optional) |  [optional] |
|**name** | **String** | Queue name |  [optional] |
|**timezone** | **String** |  |  |
|**slots** | [**List&lt;QueueSlot&gt;**](QueueSlot.md) |  |  |
|**active** | **Boolean** |  |  [optional] |
|**setAsDefault** | **Boolean** | Make this queue the default |  [optional] |
|**reshuffleExisting** | **Boolean** | Whether to reschedule existing queued posts to match new slots |  [optional] |



