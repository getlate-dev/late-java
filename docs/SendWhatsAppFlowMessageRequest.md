

# SendWhatsAppFlowMessageRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**accountId** | **String** | WhatsApp social account ID |  |
|**to** | **String** | Recipient phone number (E.164 format, e.g. +1234567890) |  |
|**flowId** | **String** | Published flow ID |  |
|**flowCta** | **String** | CTA button text (e.g. &#39;Book Now&#39;, &#39;Sign Up&#39;) |  |
|**flowAction** | [**FlowActionEnum**](#FlowActionEnum) | Action type: navigate opens a screen directly, data_exchange hits your endpoint first |  [optional] |
|**flowToken** | **String** | Unique token to correlate responses. Auto-generated UUID if omitted. |  [optional] |
|**flowActionPayload** | [**SendWhatsAppFlowMessageRequestFlowActionPayload**](SendWhatsAppFlowMessageRequestFlowActionPayload.md) |  |  [optional] |
|**body** | **String** | Message body text |  |
|**header** | [**SendWhatsAppFlowMessageRequestHeader**](SendWhatsAppFlowMessageRequestHeader.md) |  |  [optional] |
|**footer** | **String** | Optional footer text |  [optional] |
|**draft** | **Boolean** | Set true to test an unpublished (DRAFT) flow |  [optional] |



## Enum: FlowActionEnum

| Name | Value |
|---- | -----|
| NAVIGATE | &quot;navigate&quot; |
| DATA_EXCHANGE | &quot;data_exchange&quot; |



