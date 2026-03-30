

# WhatsAppTemplateButton


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**type** | [**TypeEnum**](#TypeEnum) |  |  |
|**text** | **String** |  |  |
|**url** | **URI** | Required when type is URL |  [optional] |
|**example** | **List&lt;String&gt;** | Example values for URL suffix variables |  [optional] |
|**phoneNumber** | **String** | Required when type is PHONE_NUMBER |  [optional] |
|**otpType** | [**OtpTypeEnum**](#OtpTypeEnum) | Required when type is OTP |  [optional] |
|**autofillText** | **String** |  |  [optional] |
|**packageName** | **String** |  |  [optional] |
|**signatureHash** | **String** |  |  [optional] |
|**flowId** | **String** |  |  [optional] |
|**flowName** | **String** |  |  [optional] |
|**flowJson** | **String** |  |  [optional] |
|**flowAction** | **String** |  |  [optional] |
|**navigateScreen** | **String** |  |  [optional] |



## Enum: TypeEnum

| Name | Value |
|---- | -----|
| QUICK_REPLY | &quot;QUICK_REPLY&quot; |
| URL | &quot;URL&quot; |
| PHONE_NUMBER | &quot;PHONE_NUMBER&quot; |
| OTP | &quot;OTP&quot; |
| FLOW | &quot;FLOW&quot; |
| MPM | &quot;MPM&quot; |
| CATALOG | &quot;CATALOG&quot; |



## Enum: OtpTypeEnum

| Name | Value |
|---- | -----|
| COPY_CODE | &quot;COPY_CODE&quot; |
| ONE_TAP | &quot;ONE_TAP&quot; |
| ZERO_TAP | &quot;ZERO_TAP&quot; |



