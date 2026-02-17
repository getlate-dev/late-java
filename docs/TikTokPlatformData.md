

# TikTokPlatformData

Photo carousels up to 35 images. Video titles up to 2200 chars; photo titles auto-truncated to 90 chars (use description field for longer text up to 4000 chars). privacyLevel must match creator_info options. allowDuet/allowStitch required for videos. contentPreviewConfirmed and expressConsentGiven must be true. Both camelCase and snake_case accepted.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**draft** | **Boolean** | When true, sends the post to the TikTok Creator Inbox as a draft instead of publishing immediately. |  [optional] |
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
|**videoCoverTimestampMs** | **Integer** | Optional for video posts. Timestamp in milliseconds to select which frame to use as thumbnail (defaults to 1000ms/1 second). |  [optional] |
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



