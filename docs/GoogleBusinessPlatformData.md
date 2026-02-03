

# GoogleBusinessPlatformData

Google Business Profile post settings: - Posts support text content and a single image (no videos) - Images must be publicly accessible URLs - Call-to-action buttons drive user engagement - Posts appear on your Google Business Profile and in Google Search/Maps - Use locationId to post to multiple locations from the same account connection 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**locationId** | **String** | Target Google Business location ID for multi-location posting. Format: \&quot;locations/123456789\&quot; If omitted, uses the selected/default location on the connection. Use GET /api/v1/accounts/{id}/gmb-locations to list available locations.  |  [optional] |
|**callToAction** | [**GoogleBusinessPlatformDataCallToAction**](GoogleBusinessPlatformDataCallToAction.md) |  |  [optional] |



