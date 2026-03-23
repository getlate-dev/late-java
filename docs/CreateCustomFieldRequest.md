

# CreateCustomFieldRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**profileId** | **String** |  |  |
|**name** | **String** |  |  |
|**slug** | **String** | Auto-generated from name if not provided |  [optional] |
|**type** | [**TypeEnum**](#TypeEnum) |  |  |
|**options** | **List&lt;String&gt;** | Required for select type |  [optional] |



## Enum: TypeEnum

| Name | Value |
|---- | -----|
| TEXT | &quot;text&quot; |
| NUMBER | &quot;number&quot; |
| DATE | &quot;date&quot; |
| BOOLEAN | &quot;boolean&quot; |
| SELECT | &quot;select&quot; |



