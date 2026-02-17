

# SelectGoogleBusinessLocationRequestUserProfile

Decoded user profile object from the OAuth callback. Contains the refresh token needed for token refresh. Always include this field. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**name** | **String** |  |  [optional] |
|**refreshToken** | **String** | Google refresh token for long-lived access |  [optional] |
|**tokenExpiresIn** | **Integer** | Token expiration time in seconds |  [optional] |
|**scope** | **String** | Granted OAuth scopes |  [optional] |



