

# GetGoogleBusinessLocationDetails200ResponseLocation

Compact public-facing summary derived from Google's `metadata`. Useful for surfacing the \"leave a review\" URL (e.g. behind a QR code) without parsing the raw block. Always populated regardless of readMask. For unverified or new locations Google omits placeId/reviewUrl/mapsUri, so those return as null and `isVerified` is false. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**name** | **String** | Business name as set in GBP |  [optional] |
|**placeId** | **String** | Google Maps Place ID for this location |  [optional] |
|**reviewUrl** | **String** | Public \&quot;write a review\&quot; URL Google generates for this place |  [optional] |
|**mapsUri** | **String** | Public Google Maps URL for this location |  [optional] |
|**isVerified** | **Boolean** | True when the location has Voice of Merchant (verified + live on Google) |  [optional] |



