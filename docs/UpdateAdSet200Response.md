

# UpdateAdSet200Response


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**budget** | [**AdBudget**](AdBudget.md) |  |  [optional] |
|**budgetLevel** | [**BudgetLevelEnum**](#BudgetLevelEnum) |  |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) |  |  [optional] |
|**statusUpdated** | **Integer** |  |  [optional] |
|**statusSkipped** | **Integer** |  |  [optional] |
|**bidStrategy** | **BidStrategy** |  |  [optional] |
|**bidAmount** | **BigDecimal** |  |  [optional] |
|**roasAverageFloor** | **BigDecimal** |  |  [optional] |



## Enum: BudgetLevelEnum

| Name | Value |
|---- | -----|
| ADSET | &quot;adset&quot; |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| ACTIVE | &quot;active&quot; |
| PAUSED | &quot;paused&quot; |



