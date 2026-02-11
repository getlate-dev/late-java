

# SendInboxMessageRequestReplyMarkup

Telegram-native keyboard markup. Ignored on other platforms.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**type** | [**TypeEnum**](#TypeEnum) | Keyboard type |  [optional] |
|**keyboard** | **List&lt;List&lt;SendInboxMessageRequestReplyMarkupKeyboardInnerInner&gt;&gt;** | Array of rows, each row is an array of buttons |  [optional] |
|**oneTime** | **Boolean** | Hide keyboard after use (reply_keyboard only) |  [optional] |



## Enum: TypeEnum

| Name | Value |
|---- | -----|
| INLINE_KEYBOARD | &quot;inline_keyboard&quot; |
| REPLY_KEYBOARD | &quot;reply_keyboard&quot; |



