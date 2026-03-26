

# CreateWhatsAppGroupChatRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**accountId** | **String** | WhatsApp social account ID |  |
|**subject** | **String** | Group name (max 128 characters) |  |
|**description** | **String** | Group description (max 2048 characters) |  [optional] |
|**joinApprovalMode** | [**JoinApprovalModeEnum**](#JoinApprovalModeEnum) | Whether users need approval to join via invite link |  [optional] |



## Enum: JoinApprovalModeEnum

| Name | Value |
|---- | -----|
| APPROVAL_REQUIRED | &quot;approval_required&quot; |
| AUTO_APPROVE | &quot;auto_approve&quot; |



