

# WebhookLog

Webhook delivery log entry

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** |  |  [optional] |
|**webhookId** | **String** | ID of the webhook that was triggered |  [optional] |
|**webhookName** | **String** | Name of the webhook that was triggered |  [optional] |
|**event** | [**EventEnum**](#EventEnum) |  |  [optional] |
|**url** | **URI** |  |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) |  |  [optional] |
|**statusCode** | **Integer** | HTTP status code from webhook endpoint |  [optional] |
|**requestPayload** | **Object** | Payload sent to webhook endpoint |  [optional] |
|**responseBody** | **String** | Response body from webhook endpoint (truncated to 10KB) |  [optional] |
|**errorMessage** | **String** | Error message if delivery failed |  [optional] |
|**attemptNumber** | **Integer** | Delivery attempt number (max 3 retries) |  [optional] |
|**responseTime** | **Integer** | Response time in milliseconds |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  [optional] |



## Enum: EventEnum

| Name | Value |
|---- | -----|
| POST_SCHEDULED | &quot;post.scheduled&quot; |
| POST_PUBLISHED | &quot;post.published&quot; |
| POST_FAILED | &quot;post.failed&quot; |
| POST_PARTIAL | &quot;post.partial&quot; |
| ACCOUNT_CONNECTED | &quot;account.connected&quot; |
| ACCOUNT_DISCONNECTED | &quot;account.disconnected&quot; |
| MESSAGE_RECEIVED | &quot;message.received&quot; |
| WEBHOOK_TEST | &quot;webhook.test&quot; |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| SUCCESS | &quot;success&quot; |
| FAILED | &quot;failed&quot; |



