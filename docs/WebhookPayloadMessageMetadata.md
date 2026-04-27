

# WebhookPayloadMessageMetadata

Interactive message metadata (present when message is a quick reply tap, postback button tap, or inline keyboard callback)

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**quickReplyPayload** | **String** | Payload from a quick reply tap (Facebook/Instagram Messenger). |  [optional] |
|**postbackPayload** | **String** | Payload from a postback button tap (Facebook/Instagram Messenger). |  [optional] |
|**postbackTitle** | **String** | Title of the tapped postback button (Facebook/Instagram Messenger). |  [optional] |
|**callbackData** | **String** | Callback data from an inline keyboard button tap (Telegram). |  [optional] |
|**interactiveType** | [**InteractiveTypeEnum**](#InteractiveTypeEnum) | WhatsApp only. Which kind of interactive reply the user sent: &#x60;button_reply&#x60; (tap on an interactive button), &#x60;list_reply&#x60; (tap on a list row), or &#x60;nfm_reply&#x60; (a WhatsApp Flow submission).  |  [optional] |
|**interactiveId** | **String** | WhatsApp only. The &#x60;id&#x60; of the tapped button or list row, matching the &#x60;id&#x60; you supplied when the message was sent. Not set for Flow responses.  |  [optional] |
|**buttonPayload** | **String** | WhatsApp only. Payload attached to a tapped template button. Template buttons emit a plain &#x60;button&#x60; webhook (not an interactive reply), so &#x60;interactiveType&#x60; is empty while this field is populated.  |  [optional] |
|**flowResponseJson** | **String** | WhatsApp only. Raw &#x60;nfm_reply.response_json&#x60; string returned by a Flow submission. Useful if you need the exact wire payload; for typed access use &#x60;flowResponseData&#x60; instead.  |  [optional] |
|**flowResponseData** | **Map&lt;String, Object&gt;** | WhatsApp only. Parsed Flow response JSON. Populated when &#x60;flowResponseJson&#x60; is valid JSON; otherwise omitted. Keys and value types depend on the specific Flow that was submitted.  |  [optional] |
|**referral** | [**WebhookPayloadMessageMetadataReferral**](WebhookPayloadMessageMetadataReferral.md) |  |  [optional] |



## Enum: InteractiveTypeEnum

| Name | Value |
|---- | -----|
| BUTTON_REPLY | &quot;button_reply&quot; |
| LIST_REPLY | &quot;list_reply&quot; |
| NFM_REPLY | &quot;nfm_reply&quot; |



