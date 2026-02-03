

# GetPendingOAuthData200Response


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**platform** | **String** | The platform (e.g., \&quot;linkedin\&quot;) |  [optional] |
|**profileId** | **String** | The Late profile ID |  [optional] |
|**tempToken** | **String** | Temporary access token for the platform |  [optional] |
|**refreshToken** | **String** | Refresh token (if available) |  [optional] |
|**expiresIn** | **BigDecimal** | Token expiry in seconds |  [optional] |
|**userProfile** | **Object** | User profile data (id, username, displayName, profilePicture) |  [optional] |
|**selectionType** | [**SelectionTypeEnum**](#SelectionTypeEnum) | Type of selection data |  [optional] |
|**organizations** | [**List&lt;GetPendingOAuthData200ResponseOrganizationsInner&gt;**](GetPendingOAuthData200ResponseOrganizationsInner.md) | LinkedIn organizations (when selectionType is \&quot;organizations\&quot;) |  [optional] |



## Enum: SelectionTypeEnum

| Name | Value |
|---- | -----|
| ORGANIZATIONS | &quot;organizations&quot; |
| PAGES | &quot;pages&quot; |
| BOARDS | &quot;boards&quot; |
| LOCATIONS | &quot;locations&quot; |
| PROFILES | &quot;profiles&quot; |



