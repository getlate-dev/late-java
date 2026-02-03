

# InstagramPlatformDataTrialParams

Trial Reels configuration. Trial reels are only shared to non-followers initially. They can later be \"graduated\" (converted to regular reels visible to followers) either manually in the Instagram app or automatically based on performance. Only applies to Reels (video posts). 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**graduationStrategy** | [**GraduationStrategyEnum**](#GraduationStrategyEnum) | The graduation strategy specifies when a trial reel becomes a regular reel: - MANUAL: The trial reel can only be manually graduated from the native Instagram app. - SS_PERFORMANCE: The trial reel will be automatically graduated if it performs well with non-followers.  |  [optional] |



## Enum: GraduationStrategyEnum

| Name | Value |
|---- | -----|
| MANUAL | &quot;MANUAL&quot; |
| SS_PERFORMANCE | &quot;SS_PERFORMANCE&quot; |



