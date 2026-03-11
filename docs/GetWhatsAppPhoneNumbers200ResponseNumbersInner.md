

# GetWhatsAppPhoneNumbers200ResponseNumbersInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**phoneNumber** | **String** |  |  [optional] |
|**country** | **String** |  |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) |  |  [optional] |
|**profileId** | **Object** |  |  [optional] |
|**provisionedAt** | **OffsetDateTime** |  |  [optional] |
|**metaPreverifiedId** | **String** |  |  [optional] |
|**metaVerificationStatus** | **String** |  |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| PENDING_PAYMENT | &quot;pending_payment&quot; |
| PROVISIONING | &quot;provisioning&quot; |
| ACTIVE | &quot;active&quot; |
| SUSPENDED | &quot;suspended&quot; |
| RELEASING | &quot;releasing&quot; |
| RELEASED | &quot;released&quot; |



