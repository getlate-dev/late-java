

# CreateWhatsAppTemplateRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**accountId** | **String** | WhatsApp social account ID |  |
|**name** | **String** | Template name (lowercase, letters/numbers/underscores, must start with a letter) |  |
|**category** | [**CategoryEnum**](#CategoryEnum) | Template category |  |
|**language** | **String** | Template language code (e.g., en_US) |  |
|**components** | **List&lt;Object&gt;** | Template components (header, body, footer, buttons) |  |



## Enum: CategoryEnum

| Name | Value |
|---- | -----|
| AUTHENTICATION | &quot;AUTHENTICATION&quot; |
| MARKETING | &quot;MARKETING&quot; |
| UTILITY | &quot;UTILITY&quot; |



