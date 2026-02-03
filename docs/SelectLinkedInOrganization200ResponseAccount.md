

# SelectLinkedInOrganization200ResponseAccount


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**accountId** | **String** | ID of the created SocialAccount |  [optional] |
|**platform** | [**PlatformEnum**](#PlatformEnum) |  |  [optional] |
|**username** | **String** |  |  [optional] |
|**displayName** | **String** |  |  [optional] |
|**profilePicture** | **String** |  |  [optional] |
|**isActive** | **Boolean** |  |  [optional] |
|**accountType** | [**AccountTypeEnum**](#AccountTypeEnum) |  |  [optional] |



## Enum: PlatformEnum

| Name | Value |
|---- | -----|
| LINKEDIN | &quot;linkedin&quot; |



## Enum: AccountTypeEnum

| Name | Value |
|---- | -----|
| PERSONAL | &quot;personal&quot; |
| ORGANIZATION | &quot;organization&quot; |



