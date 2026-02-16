

# GoogleBusinessPlatformData

Google Business Profile post settings: - Posts support text content and a single image (no videos) - Images must be publicly accessible URLs - Call-to-action buttons drive user engagement - Posts appear on your Google Business Profile and in Google Search/Maps - Use locationId to post to multiple locations from the same account connection - Language is auto-detected from content; override with languageCode if needed 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**locationId** | **String** | Target Google Business location ID for multi-location posting. Format: \&quot;locations/123456789\&quot; If omitted, uses the selected/default location on the connection. Use GET /api/v1/accounts/{id}/gmb-locations to list available locations.  |  [optional] |
|**languageCode** | **String** | BCP 47 language code for the post content (e.g., \&quot;en\&quot;, \&quot;de\&quot;, \&quot;es\&quot;, \&quot;fr\&quot;). If omitted, the language is automatically detected from the post text. Setting this explicitly is recommended when auto-detection may not be accurate (e.g., very short posts, mixed-language content, or transliterated text).  |  [optional] |
|**callToAction** | [**GoogleBusinessPlatformDataCallToAction**](GoogleBusinessPlatformDataCallToAction.md) |  |  [optional] |



