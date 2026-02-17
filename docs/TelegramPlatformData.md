

# TelegramPlatformData

Supports text, images (up to 10), videos (up to 10), and mixed media albums. Captions up to 1024 chars for media posts, 4096 for text-only. Channel posts show channel name as author; group posts show bot name. Analytics not available via Telegram Bot API.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**parseMode** | [**ParseModeEnum**](#ParseModeEnum) | Text formatting mode for the message (default is HTML) |  [optional] |
|**disableWebPagePreview** | **Boolean** | Disable link preview generation for URLs in the message |  [optional] |
|**disableNotification** | **Boolean** | Send the message silently (users will receive notification without sound) |  [optional] |
|**protectContent** | **Boolean** | Protect message content from forwarding and saving |  [optional] |



## Enum: ParseModeEnum

| Name | Value |
|---- | -----|
| HTML | &quot;HTML&quot; |
| MARKDOWN | &quot;Markdown&quot; |
| MARKDOWN_V2 | &quot;MarkdownV2&quot; |



