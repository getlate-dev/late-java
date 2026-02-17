

# Post


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**userId** | [**PostUserId**](PostUserId.md) |  |  [optional] |
|**title** | **String** | YouTube: title must be ≤ 100 characters.  |  [optional] |
|**content** | **String** |  |  [optional] |
|**mediaItems** | [**List&lt;MediaItem&gt;**](MediaItem.md) |  |  [optional] |
|**platforms** | [**List&lt;PlatformTarget&gt;**](PlatformTarget.md) |  |  [optional] |
|**scheduledFor** | **OffsetDateTime** |  |  [optional] |
|**timezone** | **String** |  |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) |  |  [optional] |
|**tags** | **List&lt;String&gt;** | YouTube constraints: each tag max 100 chars, combined max 500 chars, duplicates removed. |  [optional] |
|**hashtags** | **List&lt;String&gt;** |  |  [optional] |
|**mentions** | **List&lt;String&gt;** |  |  [optional] |
|**visibility** | [**VisibilityEnum**](#VisibilityEnum) |  |  [optional] |
|**metadata** | **Map&lt;String, Object&gt;** |  |  [optional] |
|**queuedFromProfile** | **String** | Profile ID if the post was scheduled via the queue |  [optional] |
|**queueId** | **String** | Queue ID if the post was scheduled via a specific queue |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  [optional] |
|**updatedAt** | **OffsetDateTime** |  |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| DRAFT | &quot;draft&quot; |
| SCHEDULED | &quot;scheduled&quot; |
| PUBLISHING | &quot;publishing&quot; |
| PUBLISHED | &quot;published&quot; |
| FAILED | &quot;failed&quot; |
| PARTIAL | &quot;partial&quot; |



## Enum: VisibilityEnum

| Name | Value |
|---- | -----|
| PUBLIC | &quot;public&quot; |
| PRIVATE | &quot;private&quot; |
| UNLISTED | &quot;unlisted&quot; |



