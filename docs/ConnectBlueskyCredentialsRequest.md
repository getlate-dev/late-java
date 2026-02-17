

# ConnectBlueskyCredentialsRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**identifier** | **String** | Your Bluesky handle (e.g. user.bsky.social) or email address |  |
|**appPassword** | **String** | App password generated from Bluesky Settings &gt; App Passwords |  |
|**state** | **String** | Required state formatted as {userId}-{profileId}. Get userId from GET /v1/users and profileId from GET /v1/profiles. |  |
|**redirectUri** | **URI** | Optional URL to redirect to after successful connection |  [optional] |



