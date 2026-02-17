

# LinkedInPlatformData

Up to 20 images, no multi-video. Single PDF supported (max 100MB, ~300 pages, cannot mix with other media). Link previews auto-generated when no media attached (disable with disableLinkPreview). Use organizationUrn for multi-org posting.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**organizationUrn** | **String** | Target LinkedIn Organization URN for multi-organization posting. Format: \&quot;urn:li:organization:123456789\&quot; If omitted, uses the selected/default organization on the connection. Use GET /api/v1/accounts/{id}/linkedin-organizations to list available organizations.  |  [optional] |
|**firstComment** | **String** | Optional first comment to add after the post is created |  [optional] |
|**disableLinkPreview** | **Boolean** | Set to true to disable automatic link previews for URLs in the post content (default is false) |  [optional] |



