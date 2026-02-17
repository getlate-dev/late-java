

# YouTubePlatformData

Videos up to 3 min are auto-detected as Shorts, longer as regular videos. Custom thumbnails supported for regular videos only (via mediaItem.thumbnail). Scheduled videos are uploaded immediately with the specified visibility. madeForKids defaults to false.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**title** | **String** | Video title. Defaults to first line of content or \&quot;Untitled Video\&quot;. Must be ≤ 100 characters. |  [optional] |
|**visibility** | [**VisibilityEnum**](#VisibilityEnum) | Video visibility: public (default, anyone can watch), unlisted (link only), private (invite only) |  [optional] |
|**madeForKids** | **Boolean** | COPPA compliance flag. Set true for child-directed content (restricts comments, notifications, ad targeting). Defaults to false. YouTube may block views if not explicitly set. |  [optional] |
|**firstComment** | **String** | Optional first comment to post immediately after video upload. Up to 10,000 characters (YouTube&#39;s comment limit). |  [optional] |
|**containsSyntheticMedia** | **Boolean** | AI-generated content disclosure. Set true if the video contains synthetic content that could be mistaken for real. YouTube may add a label. |  [optional] |
|**categoryId** | **String** | YouTube video category ID. Defaults to 22 (People &amp; Blogs). Common: 1 (Film), 2 (Autos), 10 (Music), 15 (Pets), 17 (Sports), 20 (Gaming), 23 (Comedy), 24 (Entertainment), 25 (News), 26 (Howto), 27 (Education), 28 (Science &amp; Tech). |  [optional] |



## Enum: VisibilityEnum

| Name | Value |
|---- | -----|
| PUBLIC | &quot;public&quot; |
| PRIVATE | &quot;private&quot; |
| UNLISTED | &quot;unlisted&quot; |



