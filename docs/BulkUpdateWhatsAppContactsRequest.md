

# BulkUpdateWhatsAppContactsRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**action** | [**ActionEnum**](#ActionEnum) | Bulk action to perform |  |
|**contactIds** | **List&lt;String&gt;** | Contact IDs to update (max 500) |  |
|**tags** | **List&lt;String&gt;** | Tags to add or remove (required for addTags/removeTags) |  [optional] |
|**groups** | **List&lt;String&gt;** | Groups to add or remove (required for addGroups/removeGroups) |  [optional] |



## Enum: ActionEnum

| Name | Value |
|---- | -----|
| ADD_TAGS | &quot;addTags&quot; |
| REMOVE_TAGS | &quot;removeTags&quot; |
| ADD_GROUPS | &quot;addGroups&quot; |
| REMOVE_GROUPS | &quot;removeGroups&quot; |
| OPT_IN | &quot;optIn&quot; |
| OPT_OUT | &quot;optOut&quot; |
| BLOCK | &quot;block&quot; |
| UNBLOCK | &quot;unblock&quot; |



