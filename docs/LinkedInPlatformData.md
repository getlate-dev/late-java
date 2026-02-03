

# LinkedInPlatformData

Constraints: - Multi-image posts support up to 20 images. - Multi-video posts are not supported. - Single PDF document posts are supported (max 100MB, ~300 pages). Documents cannot be mixed with other media. - Post ID is returned in the x-restli-id response header. - Link previews are automatically generated for URLs when no media is attached (can be disabled with disableLinkPreview). - Use organizationUrn to post to multiple organizations from the same account connection. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**organizationUrn** | **String** | Target LinkedIn Organization URN for multi-organization posting. Format: \&quot;urn:li:organization:123456789\&quot; If omitted, uses the selected/default organization on the connection. Use GET /api/v1/accounts/{id}/linkedin-organizations to list available organizations.  |  [optional] |
|**firstComment** | **String** | Optional first comment to add after the post is created |  [optional] |
|**disableLinkPreview** | **Boolean** | Set to true to disable automatic link previews for URLs in the post content (default is false) |  [optional] |



