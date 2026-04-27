

# SendWhatsAppConversionRequest

In addition to the `required` list, **at least one of `conversationId` or `phoneE164` must be supplied** (used to resolve the originating CTWA conversation). The route enforces this at the Zod boundary; OpenAPI's `required` cannot express OR-required cleanly. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**accountId** | **String** | WhatsApp SocialAccount ID. |  |
|**eventName** | [**EventNameEnum**](#EventNameEnum) | Live-verified allowlist of event names accepted by Meta&#39;s CAPI for Business Messaging (Graph API v25.0). Other standard pixel events including &#x60;Lead&#x60;, &#x60;CompleteRegistration&#x60;, &#x60;Subscribe&#x60;, &#x60;Schedule&#x60;, &#x60;Contact&#x60;, &#x60;StartTrial&#x60;, &#x60;AddPaymentInfo&#x60;, &#x60;Search&#x60;, and &#x60;SubmitApplication&#x60; are rejected with subcode 2804066 (\&quot;Messaging Event Invalid Event Type\&quot;) on &#x60;action_source &#x3D; business_messaging&#x60; events. Custom event names are also rejected.  Use &#x60;LeadSubmitted&#x60; (NOT &#x60;Lead&#x60;) for lead-style conversions.  |  |
|**eventTime** | **BigDecimal** | Unix seconds. Defaults to the time of the request when omitted. Meta&#39;s attribution window is 7 days from click; events older than that lose attribution.  |  [optional] |
|**eventId** | **String** | Stable dedup key. Reuse to suppress duplicate events (Meta dedupes against pixel events with the same id).  |  |
|**conversationId** | **String** | Zernio Conversation &#x60;_id&#x60; (preferred lookup). The conversation must have a captured &#x60;ctwa_clid&#x60; in metadata (set automatically by the WhatsApp webhook on the first inbound message after a CTWA ad click).  |  [optional] |
|**phoneE164** | **String** | Contact phone number, digits only with no &#39;+&#39;. When used in lieu of &#x60;conversationId&#x60;, the handler resolves to the most recent CTWA-attributed conversation for this phone on the supplied account.  |  [optional] |
|**value** | **BigDecimal** | Conversion value (e.g. order total). |  [optional] |
|**currency** | **String** | ISO 4217 currency code (e.g. &#x60;USD&#x60;). |  [optional] |
|**contentIds** | **List&lt;String&gt;** | Optional product / content identifiers. |  [optional] |
|**email** | **String** | User email. Normalized + SHA-256 hashed before sending to Meta. |  [optional] |
|**externalId** | **String** | Stable customer identifier. Lowercased + SHA-256 hashed before sending to Meta.  |  [optional] |
|**testCode** | **String** | Meta &#x60;test_event_code&#x60; passthrough. Routes the event to the Test Events tab in Events Manager instead of the production dataset, useful for development.  |  [optional] |



## Enum: EventNameEnum

| Name | Value |
|---- | -----|
| LEAD_SUBMITTED | &quot;LeadSubmitted&quot; |
| PURCHASE | &quot;Purchase&quot; |
| ADD_TO_CART | &quot;AddToCart&quot; |
| INITIATE_CHECKOUT | &quot;InitiateCheckout&quot; |
| VIEW_CONTENT | &quot;ViewContent&quot; |



