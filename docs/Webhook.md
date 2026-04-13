

# Webhook

Individual webhook configuration for receiving real-time notifications

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** | Unique webhook identifier |  [optional] |
|**name** | **String** | Webhook name (for identification) |  [optional] |
|**url** | **URI** | Webhook endpoint URL |  [optional] |
|**secret** | **String** | Secret key for HMAC-SHA256 signature (not returned in responses for security) |  [optional] |
|**events** | [**List&lt;EventsEnum&gt;**](#List&lt;EventsEnum&gt;) | Events subscribed to |  [optional] |
|**isActive** | **Boolean** | Whether webhook delivery is enabled |  [optional] |
|**lastFiredAt** | **OffsetDateTime** | Timestamp of last successful webhook delivery |  [optional] |
|**failureCount** | **Integer** | Consecutive delivery failures (resets on success, webhook disabled at 10) |  [optional] |
|**customHeaders** | **Map&lt;String, String&gt;** | Custom headers included in webhook requests |  [optional] |



## Enum: List&lt;EventsEnum&gt;

| Name | Value |
|---- | -----|
| POST_SCHEDULED | &quot;post.scheduled&quot; |
| POST_PUBLISHED | &quot;post.published&quot; |
| POST_FAILED | &quot;post.failed&quot; |
| POST_PARTIAL | &quot;post.partial&quot; |
| POST_CANCELLED | &quot;post.cancelled&quot; |
| POST_RECYCLED | &quot;post.recycled&quot; |
| ACCOUNT_CONNECTED | &quot;account.connected&quot; |
| ACCOUNT_DISCONNECTED | &quot;account.disconnected&quot; |
| MESSAGE_RECEIVED | &quot;message.received&quot; |
| MESSAGE_SENT | &quot;message.sent&quot; |
| MESSAGE_EDITED | &quot;message.edited&quot; |
| MESSAGE_DELETED | &quot;message.deleted&quot; |
| MESSAGE_DELIVERED | &quot;message.delivered&quot; |
| MESSAGE_READ | &quot;message.read&quot; |
| MESSAGE_FAILED | &quot;message.failed&quot; |
| COMMENT_RECEIVED | &quot;comment.received&quot; |



