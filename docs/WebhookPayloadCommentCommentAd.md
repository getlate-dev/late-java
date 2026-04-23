

# WebhookPayloadCommentCommentAd

Ad context. Present only when the comment was made on paid content. Instagram: populated from the webhook payload's `value.media.ad_id`/`ad_title`. Facebook: populated via a Graph API lookup of the parent post's `promotion_status`. Absent for comments on organic posts that are not currently promoted. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** | Meta ad ID (Instagram only). |  [optional] |
|**title** | **String** | Ad creative title (Instagram only). |  [optional] |
|**promotionStatus** | **String** | Facebook promotion status returned by Graph API. Common values: \&quot;active\&quot; (organic post currently boosted), \&quot;ineligible\&quot; (dark post / ad creative — not promotable because it already is an ad).  |  [optional] |



