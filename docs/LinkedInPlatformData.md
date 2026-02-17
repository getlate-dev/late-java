

# LinkedInPlatformData

Up to 20 images, no multi-video. Single PDF supported (max 100MB). Link previews auto-generated when no media attached. Use organizationUrn for multi-org posting.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**organizationUrn** | **String** | Target LinkedIn Organization URN (e.g. \&quot;urn:li:organization:123456789\&quot;). If omitted, uses the default org. Use GET /v1/accounts/{id}/linkedin-organizations to list orgs. |  [optional] |
|**firstComment** | **String** | Optional first comment to add after the post is created |  [optional] |
|**disableLinkPreview** | **Boolean** | Set to true to disable automatic link previews for URLs in the post content (default is false) |  [optional] |



