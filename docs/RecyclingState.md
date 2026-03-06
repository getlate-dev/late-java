

# RecyclingState

Current recycling configuration and state on a post

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**enabled** | **Boolean** | Whether recycling is currently active |  [optional] |
|**gap** | **Integer** | Number of interval units between reposts |  [optional] |
|**gapFreq** | [**GapFreqEnum**](#GapFreqEnum) | Interval unit (week or month) |  [optional] |
|**startDate** | **OffsetDateTime** |  |  [optional] |
|**expireCount** | **Integer** |  |  [optional] |
|**expireDate** | **OffsetDateTime** |  |  [optional] |
|**contentVariations** | **List&lt;String&gt;** | Content variations for recycled copies (if configured) |  [optional] |
|**contentVariationIndex** | **Integer** | Current position in the content variations rotation (read-only) |  [optional] |
|**recycleCount** | **Integer** | How many recycled copies have been created so far (read-only) |  [optional] |
|**nextRecycleAt** | **OffsetDateTime** | When the next recycled copy will be created (read-only) |  [optional] |
|**lastRecycledAt** | **OffsetDateTime** | When the last recycled copy was created (read-only) |  [optional] |



## Enum: GapFreqEnum

| Name | Value |
|---- | -----|
| WEEK | &quot;week&quot; |
| MONTH | &quot;month&quot; |



