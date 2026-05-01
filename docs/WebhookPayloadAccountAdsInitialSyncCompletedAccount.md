

# WebhookPayloadAccountAdsInitialSyncCompletedAccount


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**accountId** | **String** | The account&#39;s unique identifier (same as used in /v1/accounts/{accountId}) |  |
|**profileId** | **String** | The profile&#39;s unique identifier this account belongs to |  |
|**platform** | **String** |  |  |
|**username** | **String** |  |  |
|**displayName** | **String** |  |  [optional] |
|**platformUserId** | **String** | The platform-side account/ad-account ID (e.g. Meta ad account ID). |  [optional] |
|**profilePicture** | **URI** | URL of the account&#39;s profile picture, when available. |  [optional] |
|**platformAdAccountId** | **String** | When the consumer scoped the connect call to a single ad account, this echoes that ID back so the webhook can be correlated to the originating connect request without consulting the consumer&#39;s DB. Meta uses the &#x60;act_*&#x60; shape.  |  [optional] |
|**platformAdAccountIds** | **List&lt;String&gt;** | Every ad-account ID that the connected token could see at discovery time. Useful for \&quot;we synced ads from these accounts\&quot; UX without a follow-up API call. Empty array when the token had no ad-account visibility.  |  [optional] |



