

# SendInboxMessageRequestInteractiveActionOneOf2Parameters


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**flowMessageVersion** | [**FlowMessageVersionEnum**](#FlowMessageVersionEnum) | Defaults to \&quot;3\&quot; when omitted. |  [optional] |
|**flowToken** | **String** | Opaque token you choose to correlate Flow responses with your own state (max 200 chars). |  |
|**flowId** | **String** | Published Flow ID from Meta Business Manager. |  |
|**flowCta** | **String** | Button label that opens the Flow (max 20 chars). |  |
|**flowAction** | [**FlowActionEnum**](#FlowActionEnum) | &#x60;navigate&#x60; sends the user to &#x60;flow_action_payload.screen&#x60;; &#x60;data_exchange&#x60; posts data to your Flow endpoint. |  |
|**flowActionPayload** | [**SendInboxMessageRequestInteractiveActionOneOf2ParametersFlowActionPayload**](SendInboxMessageRequestInteractiveActionOneOf2ParametersFlowActionPayload.md) |  |  [optional] |
|**mode** | [**ModeEnum**](#ModeEnum) | Set to &#x60;draft&#x60; to test an unpublished Flow. |  [optional] |



## Enum: FlowMessageVersionEnum

| Name | Value |
|---- | -----|
| _3 | &quot;3&quot; |



## Enum: FlowActionEnum

| Name | Value |
|---- | -----|
| NAVIGATE | &quot;navigate&quot; |
| DATA_EXCHANGE | &quot;data_exchange&quot; |



## Enum: ModeEnum

| Name | Value |
|---- | -----|
| DRAFT | &quot;draft&quot; |



