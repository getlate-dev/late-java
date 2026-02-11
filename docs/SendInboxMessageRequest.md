

# SendInboxMessageRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**accountId** | **String** | Social account ID |  |
|**message** | **String** | Message text |  [optional] |
|**quickReplies** | [**List&lt;SendInboxMessageRequestQuickRepliesInner&gt;**](SendInboxMessageRequestQuickRepliesInner.md) | Quick reply buttons. Mutually exclusive with buttons. Max 13 items. |  [optional] |
|**buttons** | [**List&lt;SendInboxMessageRequestButtonsInner&gt;**](SendInboxMessageRequestButtonsInner.md) | Action buttons. Mutually exclusive with quickReplies. Max 3 items. |  [optional] |
|**template** | [**SendInboxMessageRequestTemplate**](SendInboxMessageRequestTemplate.md) |  |  [optional] |
|**replyMarkup** | [**SendInboxMessageRequestReplyMarkup**](SendInboxMessageRequestReplyMarkup.md) |  |  [optional] |
|**messagingType** | [**MessagingTypeEnum**](#MessagingTypeEnum) | Facebook messaging type. Required when using messageTag. |  [optional] |
|**messageTag** | [**MessageTagEnum**](#MessageTagEnum) | Facebook message tag for messaging outside 24h window. Requires messagingType MESSAGE_TAG. Instagram only supports HUMAN_AGENT. |  [optional] |
|**replyTo** | **String** | Platform message ID to reply to (Telegram only). |  [optional] |



## Enum: MessagingTypeEnum

| Name | Value |
|---- | -----|
| RESPONSE | &quot;RESPONSE&quot; |
| UPDATE | &quot;UPDATE&quot; |
| MESSAGE_TAG | &quot;MESSAGE_TAG&quot; |



## Enum: MessageTagEnum

| Name | Value |
|---- | -----|
| CONFIRMED_EVENT_UPDATE | &quot;CONFIRMED_EVENT_UPDATE&quot; |
| POST_PURCHASE_UPDATE | &quot;POST_PURCHASE_UPDATE&quot; |
| ACCOUNT_UPDATE | &quot;ACCOUNT_UPDATE&quot; |
| HUMAN_AGENT | &quot;HUMAN_AGENT&quot; |



