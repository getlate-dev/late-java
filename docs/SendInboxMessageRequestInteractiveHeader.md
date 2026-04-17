

# SendInboxMessageRequestInteractiveHeader

Optional header shown above the body.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**type** | [**TypeEnum**](#TypeEnum) |  |  [optional] |
|**text** | **String** | Required when header type is text. |  [optional] |
|**image** | [**SendInboxMessageRequestInteractiveHeaderImage**](SendInboxMessageRequestInteractiveHeaderImage.md) |  |  [optional] |
|**video** | [**SendInboxMessageRequestInteractiveHeaderImage**](SendInboxMessageRequestInteractiveHeaderImage.md) |  |  [optional] |
|**document** | [**SendInboxMessageRequestInteractiveHeaderImage**](SendInboxMessageRequestInteractiveHeaderImage.md) |  |  [optional] |



## Enum: TypeEnum

| Name | Value |
|---- | -----|
| TEXT | &quot;text&quot; |
| IMAGE | &quot;image&quot; |
| VIDEO | &quot;video&quot; |
| DOCUMENT | &quot;document&quot; |



