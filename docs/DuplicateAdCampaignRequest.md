

# DuplicateAdCampaignRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**platform** | [**PlatformEnum**](#PlatformEnum) |  |  |
|**deepCopy** | **Boolean** | Copy child ad sets + ads + creatives + targeting |  [optional] |
|**statusOption** | [**StatusOptionEnum**](#StatusOptionEnum) |  |  [optional] |
|**startTime** | **OffsetDateTime** | Reschedule the copied hierarchy&#39;s start time |  [optional] |
|**endTime** | **OffsetDateTime** |  |  [optional] |
|**renameStrategy** | [**RenameStrategyEnum**](#RenameStrategyEnum) |  |  [optional] |
|**renamePrefix** | **String** |  |  [optional] |
|**renameSuffix** | **String** |  |  [optional] |
|**syncAfter** | **Boolean** | Trigger ads discovery on the owning account after the copy succeeds |  [optional] |



## Enum: PlatformEnum

| Name | Value |
|---- | -----|
| FACEBOOK | &quot;facebook&quot; |
| INSTAGRAM | &quot;instagram&quot; |
| TIKTOK | &quot;tiktok&quot; |



## Enum: StatusOptionEnum

| Name | Value |
|---- | -----|
| ACTIVE | &quot;ACTIVE&quot; |
| PAUSED | &quot;PAUSED&quot; |
| INHERITED_FROM_SOURCE | &quot;INHERITED_FROM_SOURCE&quot; |



## Enum: RenameStrategyEnum

| Name | Value |
|---- | -----|
| DEEP_RENAME | &quot;DEEP_RENAME&quot; |
| ONLY_TOP_LEVEL_RENAME | &quot;ONLY_TOP_LEVEL_RENAME&quot; |
| NO_RENAME | &quot;NO_RENAME&quot; |



