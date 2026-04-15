

# ConversionEventUser

User identity fields. More signals mean higher match rates.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**email** | **String** | Plaintext email. Hashed server-side. |  [optional] |
|**phone** | **String** | Phone number, ideally E.164. Hashed server-side. |  [optional] |
|**firstName** | **String** | Plaintext first name. Hashed server-side. |  [optional] |
|**lastName** | **String** | Plaintext last name. Hashed server-side. |  [optional] |
|**externalId** | **String** | Stable customer identifier (e.g. CRM user ID). Hashed server-side. |  [optional] |
|**ipAddress** | **String** | Client IP address. Sent plaintext. |  [optional] |
|**userAgent** | **String** | Client user-agent string. Sent plaintext. |  [optional] |
|**country** | **String** | ISO 3166-1 alpha-2 country code, e.g. &#39;us&#39;. |  [optional] |
|**clickIds** | [**ConversionEventUserClickIds**](ConversionEventUserClickIds.md) |  |  [optional] |



