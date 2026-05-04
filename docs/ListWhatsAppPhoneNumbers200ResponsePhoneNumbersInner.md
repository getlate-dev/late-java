

# ListWhatsAppPhoneNumbers200ResponsePhoneNumbersInner

Phone number entry. Field names use Meta WhatsApp Cloud API snake_case (passed through unchanged); wabaId and wabaName are Zernio enrichment.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** | Phone Number ID (Meta) |  [optional] |
|**displayPhoneNumber** | **String** | E.164-formatted display number |  [optional] |
|**verifiedName** | **String** | Meta-verified business name |  [optional] |
|**qualityRating** | **String** | GREEN, YELLOW, RED, or UNKNOWN |  [optional] |
|**nameStatus** | **String** | APPROVED, PENDING_REVIEW, DECLINED, or NONE |  [optional] |
|**messagingLimitTier** | **String** | TIER_250, TIER_1K, TIER_10K, TIER_100K, or TIER_UNLIMITED |  [optional] |
|**wabaId** | **String** | WhatsApp Business Account ID (Zernio enrichment) |  [optional] |
|**wabaName** | **String** | WABA display name (Zernio enrichment) |  [optional] |



