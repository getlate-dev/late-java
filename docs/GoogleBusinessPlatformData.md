

# GoogleBusinessPlatformData

Text and single image only (no videos). Supports STANDARD, EVENT, and OFFER post types. Posts appear on GBP, Google Search, and Maps. Use locationId for multi-location posting.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**locationId** | **String** | Target GBP location ID (e.g. \&quot;locations/123456789\&quot;). If omitted, uses the default location. Use GET /v1/accounts/{id}/gmb-locations to list locations. |  [optional] |
|**languageCode** | **String** | BCP 47 language code (e.g. \&quot;en\&quot;, \&quot;de\&quot;, \&quot;es\&quot;). Auto-detected if omitted. Set explicitly for short or mixed-language posts. |  [optional] |
|**topicType** | [**TopicTypeEnum**](#TopicTypeEnum) | Post type. STANDARD is a regular update. EVENT requires the event object. OFFER requires the offer object. Defaults to STANDARD if omitted. |  [optional] |
|**callToAction** | [**GoogleBusinessPlatformDataCallToAction**](GoogleBusinessPlatformDataCallToAction.md) |  |  [optional] |
|**event** | [**GoogleBusinessPlatformDataEvent**](GoogleBusinessPlatformDataEvent.md) |  |  [optional] |
|**offer** | [**GoogleBusinessPlatformDataOffer**](GoogleBusinessPlatformDataOffer.md) |  |  [optional] |



## Enum: TopicTypeEnum

| Name | Value |
|---- | -----|
| STANDARD | &quot;STANDARD&quot; |
| EVENT | &quot;EVENT&quot; |
| OFFER | &quot;OFFER&quot; |



