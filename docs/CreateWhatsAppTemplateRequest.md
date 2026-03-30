

# CreateWhatsAppTemplateRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**accountId** | **String** | WhatsApp social account ID |  |
|**name** | **String** | Template name (lowercase, letters/numbers/underscores, must start with a letter) |  |
|**category** | [**CategoryEnum**](#CategoryEnum) | Template category |  |
|**language** | **String** | Template language code (e.g., en_US) |  |
|**components** | [**List&lt;WhatsAppTemplateComponent&gt;**](WhatsAppTemplateComponent.md) | Template components (HEADER, BODY, FOOTER, BUTTONS). Required for custom templates, omit when using library_template_name. |  [optional] |
|**libraryTemplateName** | **String** | Name of a pre-built template from Meta&#39;s template library (e.g., \&quot;appointment_reminder\&quot;, \&quot;auto_pay_reminder_1\&quot;, \&quot;address_update\&quot;). When provided, the template is pre-approved by Meta with no review wait. Omit &#x60;components&#x60; when using this field.  |  [optional] |
|**libraryTemplateBodyInputs** | **Object** | Optional body customizations for library templates. Available options depend on the template (e.g., add_contact_number, add_learn_more_link, add_security_recommendation, add_track_package_link, code_expiration_minutes).  |  [optional] |
|**libraryTemplateButtonInputs** | [**List&lt;CreateWhatsAppTemplateRequestLibraryTemplateButtonInputsInner&gt;**](CreateWhatsAppTemplateRequestLibraryTemplateButtonInputsInner.md) | Optional button customizations for library templates. Each item specifies button type and configuration (e.g., URL, phone number, quick reply).  |  [optional] |



## Enum: CategoryEnum

| Name | Value |
|---- | -----|
| AUTHENTICATION | &quot;AUTHENTICATION&quot; |
| MARKETING | &quot;MARKETING&quot; |
| UTILITY | &quot;UTILITY&quot; |



