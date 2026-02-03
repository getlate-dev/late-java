

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
|**tags** | **List&lt;String&gt;** | YouTube tag constraints when targeting YouTube: - No count cap; duplicates removed. - Each tag must be ≤ 100 chars. - Combined characters across all tags ≤ 500.  |  [optional] |
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



