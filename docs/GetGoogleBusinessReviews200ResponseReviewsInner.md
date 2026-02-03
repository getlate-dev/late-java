

# GetGoogleBusinessReviews200ResponseReviewsInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** | Review ID |  [optional] |
|**name** | **String** | Full resource name |  [optional] |
|**reviewer** | [**GetGoogleBusinessReviews200ResponseReviewsInnerReviewer**](GetGoogleBusinessReviews200ResponseReviewsInnerReviewer.md) |  |  [optional] |
|**rating** | **Integer** | Numeric star rating |  [optional] |
|**starRating** | [**StarRatingEnum**](#StarRatingEnum) | Google&#39;s string rating |  [optional] |
|**comment** | **String** | Review text |  [optional] |
|**createTime** | **OffsetDateTime** |  |  [optional] |
|**updateTime** | **OffsetDateTime** |  |  [optional] |
|**reviewReply** | [**GetGoogleBusinessReviews200ResponseReviewsInnerReviewReply**](GetGoogleBusinessReviews200ResponseReviewsInnerReviewReply.md) |  |  [optional] |



## Enum: StarRatingEnum

| Name | Value |
|---- | -----|
| ONE | &quot;ONE&quot; |
| TWO | &quot;TWO&quot; |
| THREE | &quot;THREE&quot; |
| FOUR | &quot;FOUR&quot; |
| FIVE | &quot;FIVE&quot; |



