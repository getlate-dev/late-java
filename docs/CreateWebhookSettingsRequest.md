

# CreateWebhookSettingsRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**name** | **String** | Webhook name (max 50 characters) |  [optional] |
|**url** | **URI** | Webhook endpoint URL (must be HTTPS in production) |  [optional] |
|**secret** | **String** | Secret key for HMAC-SHA256 signature verification |  [optional] |
|**events** | [**List&lt;EventsEnum&gt;**](#List&lt;EventsEnum&gt;) | Events to subscribe to |  [optional] |
|**isActive** | **Boolean** | Enable or disable webhook delivery |  [optional] |
|**customHeaders** | **Map&lt;String, String&gt;** | Custom headers to include in webhook requests |  [optional] |



## Enum: List&lt;EventsEnum&gt;

| Name | Value |
|---- | -----|
| POST_SCHEDULED | &quot;post.scheduled&quot; |
| POST_PUBLISHED | &quot;post.published&quot; |
| POST_FAILED | &quot;post.failed&quot; |
| POST_PARTIAL | &quot;post.partial&quot; |
| ACCOUNT_CONNECTED | &quot;account.connected&quot; |
| ACCOUNT_DISCONNECTED | &quot;account.disconnected&quot; |
| MESSAGE_RECEIVED | &quot;message.received&quot; |
| COMMENT_RECEIVED | &quot;comment.received&quot; |



