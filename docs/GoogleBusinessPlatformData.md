

# GoogleBusinessPlatformData

Posts support text and a single image (no videos). Images must be publicly accessible URLs. Optional call-to-action button. Posts appear on GBP, Google Search, and Maps. Use locationId for multi-location posting. Language is auto-detected; override with languageCode.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**locationId** | **String** | Target Google Business location ID for multi-location posting. Format: \&quot;locations/123456789\&quot; If omitted, uses the selected/default location on the connection. Use GET /api/v1/accounts/{id}/gmb-locations to list available locations.  |  [optional] |
|**languageCode** | **String** | BCP 47 language code for the post content (e.g., \&quot;en\&quot;, \&quot;de\&quot;, \&quot;es\&quot;, \&quot;fr\&quot;). If omitted, the language is automatically detected from the post text. Setting this explicitly is recommended when auto-detection may not be accurate (e.g., very short posts, mixed-language content, or transliterated text).  |  [optional] |
|**callToAction** | [**GoogleBusinessPlatformDataCallToAction**](GoogleBusinessPlatformDataCallToAction.md) |  |  [optional] |



