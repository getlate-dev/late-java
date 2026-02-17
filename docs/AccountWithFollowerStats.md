

# AccountWithFollowerStats


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**platform** | **String** |  |  [optional] |
|**profileId** | [**SocialAccountProfileId**](SocialAccountProfileId.md) |  |  [optional] |
|**username** | **String** |  |  [optional] |
|**displayName** | **String** |  |  [optional] |
|**profileUrl** | **String** | Full profile URL for the connected account on its platform. |  [optional] |
|**isActive** | **Boolean** |  |  [optional] |
|**followersCount** | **BigDecimal** | Follower count (only included if user has analytics add-on) |  [optional] |
|**followersLastUpdated** | **OffsetDateTime** | Last time follower count was updated (only included if user has analytics add-on) |  [optional] |
|**profilePicture** | **String** |  |  [optional] |
|**currentFollowers** | **BigDecimal** | Current follower count |  [optional] |
|**lastUpdated** | **OffsetDateTime** |  |  [optional] |
|**growth** | **BigDecimal** | Follower change over period |  [optional] |
|**growthPercentage** | **BigDecimal** | Percentage growth |  [optional] |
|**dataPoints** | **BigDecimal** | Number of historical snapshots |  [optional] |



