

# GetInboxConversationMessages200Response


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**status** | **String** |  |  [optional] |
|**pagination** | [**GetInboxConversationMessages200ResponsePagination**](GetInboxConversationMessages200ResponsePagination.md) |  |  [optional] |
|**sortOrderApplied** | [**SortOrderAppliedEnum**](#SortOrderAppliedEnum) | Sort order actually applied to the returned page. May differ from the requested &#x60;sortOrder&#x60; for Twitter, Facebook and Bluesky (always &#x60;desc&#x60; regardless of request).  |  [optional] |
|**messages** | [**List&lt;GetInboxConversationMessages200ResponseMessagesInner&gt;**](GetInboxConversationMessages200ResponseMessagesInner.md) |  |  [optional] |
|**lastUpdated** | **OffsetDateTime** |  |  [optional] |



## Enum: SortOrderAppliedEnum

| Name | Value |
|---- | -----|
| ASC | &quot;asc&quot; |
| DESC | &quot;desc&quot; |



