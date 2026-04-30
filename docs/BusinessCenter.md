

# BusinessCenter

TikTok Business Center entity. Returned by `GET /v1/ads/business-centers`. BCs are TikTok's agency container — one BC owns N advertisers (ad accounts). Most solo advertisers don't have one; the agency token uses BCs to roll up multi-client access. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**bcId** | **String** | Business Center ID |  [optional] |
|**name** | **String** | Display name set by the BC owner |  [optional] |
|**advertiserCount** | **Integer** | Number of advertisers reachable under this BC for the calling token. &#x60;null&#x60; when the BC asset walk returned empty or failed (typical for agency apps without full BC asset read scope) — distinct from &#x60;0&#x60;, which would imply the BC genuinely has no advertisers.  |  [optional] |



