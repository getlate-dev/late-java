

# ConversionEvent

A single conversion event to relay to the ad platform. All PII fields (email, phone, names) are hashed with SHA-256 server-side using each platform's normalization rules before they leave Zernio. Callers send plaintext. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**eventName** | **String** | Standard event name (Purchase, Lead, CompleteRegistration, AddToCart, InitiateCheckout, AddPaymentInfo, Subscribe, StartTrial, ViewContent, Search, Contact, SubmitApplication, Schedule) or a custom string (only supported on platforms that accept custom events).  |  |
|**eventTime** | **Integer** | When the conversion happened, in unix seconds. |  |
|**eventId** | **String** | Unique dedup key. The same eventId must be used on pixel + CAPI to prevent double-counting. Mapped to event_id on Meta and transactionId on Google.  |  |
|**value** | **BigDecimal** | Conversion value in the specified currency. |  [optional] |
|**currency** | **String** | ISO 4217 currency code. |  [optional] |
|**user** | [**ConversionEventUser**](ConversionEventUser.md) |  |  |
|**items** | [**List&lt;ConversionEventItemsInner&gt;**](ConversionEventItemsInner.md) | Item-level detail for ecommerce events. |  [optional] |
|**sourceUrl** | **URI** | URL where the conversion originated (used by Meta). |  [optional] |
|**actionSource** | [**ActionSourceEnum**](#ActionSourceEnum) | Where the conversion happened. Used by Meta; Google ignores. |  [optional] |
|**platformData** | **Map&lt;String, Object&gt;** | Escape hatch for platform-specific fields we haven&#39;t normalized. Forwarded as-is. |  [optional] |



## Enum: ActionSourceEnum

| Name | Value |
|---- | -----|
| WEB | &quot;web&quot; |
| APP | &quot;app&quot; |
| OFFLINE | &quot;offline&quot; |
| CRM | &quot;crm&quot; |
| PHONE_CALL | &quot;phone_call&quot; |
| SYSTEM_GENERATED | &quot;system_generated&quot; |



