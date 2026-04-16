

# GeoRestriction

Country-level geo-restriction (allowlist). When set, the post is only visible to users in the specified countries. Supported on Facebook (feed posts, videos, reels), X/Twitter (media-level restriction), and LinkedIn (organization pages only, min 300 targeted followers). Ignored on unsupported platforms. Stories (Facebook, Instagram) do not support geo-restriction. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**countries** | **List&lt;String&gt;** | ISO 3166-1 alpha-2 country codes (uppercase). Only users in these countries can see the post. Maximum 25 countries per post. Example: [\&quot;US\&quot;, \&quot;CA\&quot;, \&quot;GB\&quot;, \&quot;ES\&quot;].  |  |



