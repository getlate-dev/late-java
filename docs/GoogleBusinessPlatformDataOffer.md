

# GoogleBusinessPlatformDataOffer

Offer details. Required when topicType is OFFER. All fields are optional per Google's API, but at least one is recommended.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**offerType** | [**OfferTypeEnum**](#OfferTypeEnum) | Type of offer |  [optional] |
|**redeemOnlineUrl** | **URI** | URL where the offer can be redeemed online |  [optional] |
|**termsConditions** | **String** | Terms and conditions for the offer |  [optional] |
|**couponCode** | **String** | Coupon code for the offer |  [optional] |



## Enum: OfferTypeEnum

| Name | Value |
|---- | -----|
| OFFER | &quot;OFFER&quot; |
| BUY_ONE_GET_ONE | &quot;BUY_ONE_GET_ONE&quot; |



