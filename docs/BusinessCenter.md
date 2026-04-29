

# BusinessCenter

TikTok Business Center entity. Returned by `GET /v1/ads/business-centers`. BCs are TikTok's agency container — one BC owns N advertisers (ad accounts). Most solo advertisers don't have one; the agency token uses BCs to roll up multi-client access. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**bcId** | **String** | Business Center ID |  [optional] |
|**name** | **String** | Display name set by the BC owner |  [optional] |
|**advertiserCount** | **Integer** | Number of advertisers (ad accounts) reachable under this BC for the calling token |  [optional] |



