

# Lead

A single lead submission returned by the leads endpoint and the lead.received webhook.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** | Meta &#x60;leadgen_id&#x60;. |  [optional] |
|**createdTime** | **OffsetDateTime** |  |  [optional] |
|**adId** | **String** | Meta ad ID that surfaced the form. Organic leads omit this. |  [optional] |
|**formId** | **String** |  |  [optional] |
|**fields** | **Map&lt;String, String&gt;** | Flattened key→value map of answers (multi-value fields joined with \&quot;, \&quot;). |  [optional] |
|**fieldData** | [**List&lt;LeadFieldDataInner&gt;**](LeadFieldDataInner.md) | Raw &#x60;field_data&#x60; from Meta (one entry per question). |  [optional] |



