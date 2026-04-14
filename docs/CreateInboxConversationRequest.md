

# CreateInboxConversationRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**accountId** | **String** | The social account ID to send from |  |
|**participantId** | **String** | Twitter numeric user ID of the recipient. Provide either this or participantUsername. |  [optional] |
|**participantUsername** | **String** | Twitter username (with or without @) of the recipient. Resolved to a user ID via lookup. Provide either this or participantId. |  [optional] |
|**message** | **String** | Text content of the message. At least one of message or attachment is required. |  [optional] |
|**skipDmCheck** | **Boolean** | Skip the receives_your_dm eligibility check before sending. Use if you have already verified the recipient accepts DMs. |  [optional] |



