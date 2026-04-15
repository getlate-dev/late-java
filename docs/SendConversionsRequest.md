

# SendConversionsRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**accountId** | **String** | SocialAccount ID (metaads or googleads). |  |
|**destinationId** | **String** | Platform destination identifier. For Meta, the pixel/dataset ID. For Google, the conversion action resource name.  |  |
|**events** | [**List&lt;ConversionEvent&gt;**](ConversionEvent.md) |  |  |
|**testCode** | **String** | Meta &#x60;test_event_code&#x60; passthrough. Ignored by Google. |  [optional] |
|**consent** | [**SendConversionsRequestConsent**](SendConversionsRequestConsent.md) |  |  [optional] |



