

# CreateStandaloneAdRequestPromotedObject

Meta only. Forwarded to the ad set's `promoted_object` (snake-cased).  Required for goals whose ad-set optimization_goal points at a specific event/page/app — without it Meta rejects the ad-set create with `error_subcode: 1815430` \"Please select a promoted object for your ad set\":   - `goal: conversions` (OFFSITE_CONVERSIONS) — requires `pixelId` + `customEventType`   - `goal: app_promotion` (APP_INSTALLS) — requires `applicationId` + `objectStoreUrl`   - `goal: lead_generation` (LEAD_GENERATION) — `pageId` is auto-filled from the connected Page when omitted  Other goals (engagement, traffic, awareness, video_views) ignore this field. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**pixelId** | **String** | Facebook Pixel ID. Required for &#x60;goal: conversions&#x60;. |  [optional] |
|**customEventType** | **String** | Standard event the campaign optimises against, e.g. &#x60;PURCHASE&#x60;, &#x60;LEAD&#x60;, &#x60;COMPLETE_REGISTRATION&#x60;, &#x60;ADD_TO_CART&#x60;. Uppercased internally so callers can pass any case. Required for &#x60;goal: conversions&#x60;.  |  [optional] |
|**pageId** | **String** | Facebook Page ID. Used by &#x60;goal: lead_generation&#x60;. Auto-filled from the connected Page when omitted.  |  [optional] |
|**applicationId** | **String** | App ID. Required for &#x60;goal: app_promotion&#x60;. |  [optional] |
|**objectStoreUrl** | **URI** | App Store / Play Store listing URL. Required for &#x60;goal: app_promotion&#x60;. |  [optional] |
|**customConversionId** | **String** | Custom Conversion ID, when optimising against one instead of a standard event. |  [optional] |
|**productCatalogId** | **String** | Catalog ID for catalog/Advantage+ Shopping campaigns. |  [optional] |
|**productSetId** | **String** | Product Set ID inside the catalog. |  [optional] |



