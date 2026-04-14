

# TikTokPlatformData

Photo carousels up to 35 images. Video titles up to 2200 chars, photo titles truncated to 90 chars. privacyLevel must match creator_info options. Both camelCase and snake_case accepted.  Creator Inbox (draft mode): Set draft: true to send content to the TikTok Creator Inbox instead of publishing immediately. The creator receives an inbox notification and completes the post using TikTok's editing flow. This maps to TikTok's post_mode: \"MEDIA_UPLOAD\" internally.  Important: The field publish_type is NOT supported. Use draft: true for Creator Inbox flow.  Photo drafts use the /v2/post/publish/content/init/ endpoint with post_mode: \"MEDIA_UPLOAD\". Video drafts use the dedicated /v2/post/publish/inbox/video/init/ endpoint.  When draft: true, the video.upload scope is required. When draft is false or omitted (direct post), the video.publish scope is required. For Creator Inbox, TikTok app version must be 31.8 or higher. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**draft** | **Boolean** | When true, sends the post to the TikTok Creator Inbox as a draft instead of publishing immediately. The creator receives an inbox notification to complete posting via TikTok&#39;s editing flow. Maps to TikTok API post_mode: \&quot;MEDIA_UPLOAD\&quot; (photos) or the dedicated inbox endpoint (videos). When false or omitted, publishes directly via post_mode: \&quot;DIRECT_POST\&quot;. Note: publish_type is not a supported field. Use this field instead.  |  [optional] |
|**privacyLevel** | **String** | One of the values returned by the TikTok creator info API for the account |  [optional] |
|**allowComment** | **Boolean** | Allow comments on the post |  [optional] |
|**allowDuet** | **Boolean** | Allow duets (required for video posts) |  [optional] |
|**allowStitch** | **Boolean** | Allow stitches (required for video posts) |  [optional] |
|**commercialContentType** | [**CommercialContentTypeEnum**](#CommercialContentTypeEnum) | Type of commercial content disclosure |  [optional] |
|**brandPartnerPromote** | **Boolean** | Whether the post promotes a brand partner |  [optional] |
|**isBrandOrganicPost** | **Boolean** | Whether the post is a brand organic post |  [optional] |
|**contentPreviewConfirmed** | **Boolean** | User has confirmed they previewed the content |  [optional] |
|**expressConsentGiven** | **Boolean** | User has given express consent for posting |  [optional] |
|**mediaType** | [**MediaTypeEnum**](#MediaTypeEnum) | Optional override. Defaults based on provided media items. |  [optional] |
|**videoCoverTimestampMs** | **Integer** | Optional for video posts. Timestamp in milliseconds to select which frame to use as thumbnail (defaults to 1000ms/1 second). Ignored when videoCoverImageUrl is provided. |  [optional] |
|**videoCoverImageUrl** | **URI** | Optional for video posts. URL of a custom thumbnail image (JPG, PNG, or WebP, max 20MB). The image is stitched as a single frame at the start of the video and used as the cover. Overrides videoCoverTimestampMs when provided. |  [optional] |
|**photoCoverIndex** | **Integer** | Optional for photo carousels. Index of image to use as cover, 0-based (defaults to 0/first image). |  [optional] |
|**autoAddMusic** | **Boolean** | When true, TikTok may add recommended music (photos only) |  [optional] |
|**videoMadeWithAi** | **Boolean** | Set true to disclose AI-generated content |  [optional] |
|**description** | **String** | Optional long-form description for photo posts (max 4000 chars). Recommended when content exceeds 90 chars, as photo titles are auto-truncated. |  [optional] |



## Enum: CommercialContentTypeEnum

| Name | Value |
|---- | -----|
| NONE | &quot;none&quot; |
| BRAND_ORGANIC | &quot;brand_organic&quot; |
| BRAND_CONTENT | &quot;brand_content&quot; |



## Enum: MediaTypeEnum

| Name | Value |
|---- | -----|
| VIDEO | &quot;video&quot; |
| PHOTO | &quot;photo&quot; |



