# AdCampaignsApi

All URIs are relative to *https://zernio.com/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**bulkUpdateAdCampaignStatus**](AdCampaignsApi.md#bulkUpdateAdCampaignStatus) | **POST** /v1/ads/campaigns/bulk-status | Pause or resume many campaigns |
| [**bulkUpdateAdCampaignStatusWithHttpInfo**](AdCampaignsApi.md#bulkUpdateAdCampaignStatusWithHttpInfo) | **POST** /v1/ads/campaigns/bulk-status | Pause or resume many campaigns |
| [**deleteAdCampaign**](AdCampaignsApi.md#deleteAdCampaign) | **DELETE** /v1/ads/campaigns/{campaignId} | Delete a campaign |
| [**deleteAdCampaignWithHttpInfo**](AdCampaignsApi.md#deleteAdCampaignWithHttpInfo) | **DELETE** /v1/ads/campaigns/{campaignId} | Delete a campaign |
| [**duplicateAdCampaign**](AdCampaignsApi.md#duplicateAdCampaign) | **POST** /v1/ads/campaigns/{campaignId}/duplicate | Duplicate a campaign |
| [**duplicateAdCampaignWithHttpInfo**](AdCampaignsApi.md#duplicateAdCampaignWithHttpInfo) | **POST** /v1/ads/campaigns/{campaignId}/duplicate | Duplicate a campaign |
| [**getAdTree**](AdCampaignsApi.md#getAdTree) | **GET** /v1/ads/tree | Get campaign tree |
| [**getAdTreeWithHttpInfo**](AdCampaignsApi.md#getAdTreeWithHttpInfo) | **GET** /v1/ads/tree | Get campaign tree |
| [**listAdCampaigns**](AdCampaignsApi.md#listAdCampaigns) | **GET** /v1/ads/campaigns | List campaigns |
| [**listAdCampaignsWithHttpInfo**](AdCampaignsApi.md#listAdCampaignsWithHttpInfo) | **GET** /v1/ads/campaigns | List campaigns |
| [**updateAdCampaign**](AdCampaignsApi.md#updateAdCampaign) | **PUT** /v1/ads/campaigns/{campaignId} | Update a campaign (budget and/or bid strategy) |
| [**updateAdCampaignWithHttpInfo**](AdCampaignsApi.md#updateAdCampaignWithHttpInfo) | **PUT** /v1/ads/campaigns/{campaignId} | Update a campaign (budget and/or bid strategy) |
| [**updateAdCampaignStatus**](AdCampaignsApi.md#updateAdCampaignStatus) | **PUT** /v1/ads/campaigns/{campaignId}/status | Pause or resume a campaign |
| [**updateAdCampaignStatusWithHttpInfo**](AdCampaignsApi.md#updateAdCampaignStatusWithHttpInfo) | **PUT** /v1/ads/campaigns/{campaignId}/status | Pause or resume a campaign |
| [**updateAdSet**](AdCampaignsApi.md#updateAdSet) | **PUT** /v1/ads/ad-sets/{adSetId} | Update an ad set (budget, status, and/or bid strategy) |
| [**updateAdSetWithHttpInfo**](AdCampaignsApi.md#updateAdSetWithHttpInfo) | **PUT** /v1/ads/ad-sets/{adSetId} | Update an ad set (budget, status, and/or bid strategy) |
| [**updateAdSetStatus**](AdCampaignsApi.md#updateAdSetStatus) | **PUT** /v1/ads/ad-sets/{adSetId}/status | Pause or resume a single ad set |
| [**updateAdSetStatusWithHttpInfo**](AdCampaignsApi.md#updateAdSetStatusWithHttpInfo) | **PUT** /v1/ads/ad-sets/{adSetId}/status | Pause or resume a single ad set |



## bulkUpdateAdCampaignStatus

> BulkUpdateAdCampaignStatus200Response bulkUpdateAdCampaignStatus(bulkUpdateAdCampaignStatusRequest)

Pause or resume many campaigns

Process up to 50 campaigns in one call. Each campaign is updated concurrently and the response contains a per-campaign result so a single bad row does not fail the whole batch. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdCampaignsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdCampaignsApi apiInstance = new AdCampaignsApi(defaultClient);
        BulkUpdateAdCampaignStatusRequest bulkUpdateAdCampaignStatusRequest = new BulkUpdateAdCampaignStatusRequest(); // BulkUpdateAdCampaignStatusRequest | 
        try {
            BulkUpdateAdCampaignStatus200Response result = apiInstance.bulkUpdateAdCampaignStatus(bulkUpdateAdCampaignStatusRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdCampaignsApi#bulkUpdateAdCampaignStatus");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **bulkUpdateAdCampaignStatusRequest** | [**BulkUpdateAdCampaignStatusRequest**](BulkUpdateAdCampaignStatusRequest.md)|  | |

### Return type

[**BulkUpdateAdCampaignStatus200Response**](BulkUpdateAdCampaignStatus200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Per-campaign results |  -  |
| **400** | Invalid input |  -  |
| **401** | Unauthorized |  -  |

## bulkUpdateAdCampaignStatusWithHttpInfo

> ApiResponse<BulkUpdateAdCampaignStatus200Response> bulkUpdateAdCampaignStatus bulkUpdateAdCampaignStatusWithHttpInfo(bulkUpdateAdCampaignStatusRequest)

Pause or resume many campaigns

Process up to 50 campaigns in one call. Each campaign is updated concurrently and the response contains a per-campaign result so a single bad row does not fail the whole batch. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdCampaignsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdCampaignsApi apiInstance = new AdCampaignsApi(defaultClient);
        BulkUpdateAdCampaignStatusRequest bulkUpdateAdCampaignStatusRequest = new BulkUpdateAdCampaignStatusRequest(); // BulkUpdateAdCampaignStatusRequest | 
        try {
            ApiResponse<BulkUpdateAdCampaignStatus200Response> response = apiInstance.bulkUpdateAdCampaignStatusWithHttpInfo(bulkUpdateAdCampaignStatusRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdCampaignsApi#bulkUpdateAdCampaignStatus");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Response headers: " + e.getResponseHeaders());
            System.err.println("Reason: " + e.getResponseBody());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **bulkUpdateAdCampaignStatusRequest** | [**BulkUpdateAdCampaignStatusRequest**](BulkUpdateAdCampaignStatusRequest.md)|  | |

### Return type

ApiResponse<[**BulkUpdateAdCampaignStatus200Response**](BulkUpdateAdCampaignStatus200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Per-campaign results |  -  |
| **400** | Invalid input |  -  |
| **401** | Unauthorized |  -  |


## deleteAdCampaign

> DeleteAdCampaign200Response deleteAdCampaign(campaignId, deleteAdCampaignRequest)

Delete a campaign

Deletes the whole campaign on the platform, cascading to its ad sets and ads. Locally, all Ad documents for this campaign are marked &#x60;status: cancelled&#x60;.  Meta-only for now. Other platforms return 501 Not Implemented — fall back to DELETE /v1/ads/{adId} per ad in the meantime. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdCampaignsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdCampaignsApi apiInstance = new AdCampaignsApi(defaultClient);
        String campaignId = "campaignId_example"; // String | Platform campaign ID
        DeleteAdCampaignRequest deleteAdCampaignRequest = new DeleteAdCampaignRequest(); // DeleteAdCampaignRequest | 
        try {
            DeleteAdCampaign200Response result = apiInstance.deleteAdCampaign(campaignId, deleteAdCampaignRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdCampaignsApi#deleteAdCampaign");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **campaignId** | **String**| Platform campaign ID | |
| **deleteAdCampaignRequest** | [**DeleteAdCampaignRequest**](DeleteAdCampaignRequest.md)|  | |

### Return type

[**DeleteAdCampaign200Response**](DeleteAdCampaign200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Campaign deleted |  -  |
| **401** | Unauthorized |  -  |
| **404** | Campaign not found |  -  |
| **501** | Operation not supported on this platform |  -  |

## deleteAdCampaignWithHttpInfo

> ApiResponse<DeleteAdCampaign200Response> deleteAdCampaign deleteAdCampaignWithHttpInfo(campaignId, deleteAdCampaignRequest)

Delete a campaign

Deletes the whole campaign on the platform, cascading to its ad sets and ads. Locally, all Ad documents for this campaign are marked &#x60;status: cancelled&#x60;.  Meta-only for now. Other platforms return 501 Not Implemented — fall back to DELETE /v1/ads/{adId} per ad in the meantime. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdCampaignsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdCampaignsApi apiInstance = new AdCampaignsApi(defaultClient);
        String campaignId = "campaignId_example"; // String | Platform campaign ID
        DeleteAdCampaignRequest deleteAdCampaignRequest = new DeleteAdCampaignRequest(); // DeleteAdCampaignRequest | 
        try {
            ApiResponse<DeleteAdCampaign200Response> response = apiInstance.deleteAdCampaignWithHttpInfo(campaignId, deleteAdCampaignRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdCampaignsApi#deleteAdCampaign");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Response headers: " + e.getResponseHeaders());
            System.err.println("Reason: " + e.getResponseBody());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **campaignId** | **String**| Platform campaign ID | |
| **deleteAdCampaignRequest** | [**DeleteAdCampaignRequest**](DeleteAdCampaignRequest.md)|  | |

### Return type

ApiResponse<[**DeleteAdCampaign200Response**](DeleteAdCampaign200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Campaign deleted |  -  |
| **401** | Unauthorized |  -  |
| **404** | Campaign not found |  -  |
| **501** | Operation not supported on this platform |  -  |


## duplicateAdCampaign

> DuplicateAdCampaign200Response duplicateAdCampaign(campaignId, duplicateAdCampaignRequest)

Duplicate a campaign

Duplicates a campaign, including its ad sets, ads, creatives, and targeting by default (&#x60;deepCopy: true&#x60;). The copy is created paused so callers can review before launching.  Per-platform implementation: - **Meta** uses the native &#x60;POST /{campaign-id}/copies&#x60; endpoint. - **TikTok** has no native copy primitive; Zernio walks the source   graph (&#x60;/v2/campaign/get/&#x60;, &#x60;/v2/adgroup/get/&#x60;, &#x60;/v2/ad/get/&#x60;) and   recreates each entity via the corresponding &#x60;/create/&#x60; endpoints,   carrying over budget / targeting / bid_type / bid_price /   deep_bid_type / creative fields. Spark Ad linkage (&#x60;tiktok_item_id&#x60;)   is preserved.  The new hierarchy is asynchronous to materialize in our DB — we trigger sync discovery automatically. Set &#x60;syncAfter: false&#x60; to skip and poll &#x60;/v1/ads/tree&#x60; on your own cadence.  Other platforms return 501 Not Implemented. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdCampaignsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdCampaignsApi apiInstance = new AdCampaignsApi(defaultClient);
        String campaignId = "campaignId_example"; // String | Source platform campaign ID
        DuplicateAdCampaignRequest duplicateAdCampaignRequest = new DuplicateAdCampaignRequest(); // DuplicateAdCampaignRequest | 
        try {
            DuplicateAdCampaign200Response result = apiInstance.duplicateAdCampaign(campaignId, duplicateAdCampaignRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdCampaignsApi#duplicateAdCampaign");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **campaignId** | **String**| Source platform campaign ID | |
| **duplicateAdCampaignRequest** | [**DuplicateAdCampaignRequest**](DuplicateAdCampaignRequest.md)|  | |

### Return type

[**DuplicateAdCampaign200Response**](DuplicateAdCampaign200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Campaign duplicated |  -  |
| **400** | Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Source campaign not found |  -  |
| **501** | Operation not supported on this platform |  -  |

## duplicateAdCampaignWithHttpInfo

> ApiResponse<DuplicateAdCampaign200Response> duplicateAdCampaign duplicateAdCampaignWithHttpInfo(campaignId, duplicateAdCampaignRequest)

Duplicate a campaign

Duplicates a campaign, including its ad sets, ads, creatives, and targeting by default (&#x60;deepCopy: true&#x60;). The copy is created paused so callers can review before launching.  Per-platform implementation: - **Meta** uses the native &#x60;POST /{campaign-id}/copies&#x60; endpoint. - **TikTok** has no native copy primitive; Zernio walks the source   graph (&#x60;/v2/campaign/get/&#x60;, &#x60;/v2/adgroup/get/&#x60;, &#x60;/v2/ad/get/&#x60;) and   recreates each entity via the corresponding &#x60;/create/&#x60; endpoints,   carrying over budget / targeting / bid_type / bid_price /   deep_bid_type / creative fields. Spark Ad linkage (&#x60;tiktok_item_id&#x60;)   is preserved.  The new hierarchy is asynchronous to materialize in our DB — we trigger sync discovery automatically. Set &#x60;syncAfter: false&#x60; to skip and poll &#x60;/v1/ads/tree&#x60; on your own cadence.  Other platforms return 501 Not Implemented. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdCampaignsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdCampaignsApi apiInstance = new AdCampaignsApi(defaultClient);
        String campaignId = "campaignId_example"; // String | Source platform campaign ID
        DuplicateAdCampaignRequest duplicateAdCampaignRequest = new DuplicateAdCampaignRequest(); // DuplicateAdCampaignRequest | 
        try {
            ApiResponse<DuplicateAdCampaign200Response> response = apiInstance.duplicateAdCampaignWithHttpInfo(campaignId, duplicateAdCampaignRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdCampaignsApi#duplicateAdCampaign");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Response headers: " + e.getResponseHeaders());
            System.err.println("Reason: " + e.getResponseBody());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **campaignId** | **String**| Source platform campaign ID | |
| **duplicateAdCampaignRequest** | [**DuplicateAdCampaignRequest**](DuplicateAdCampaignRequest.md)|  | |

### Return type

ApiResponse<[**DuplicateAdCampaign200Response**](DuplicateAdCampaign200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Campaign duplicated |  -  |
| **400** | Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Source campaign not found |  -  |
| **501** | Operation not supported on this platform |  -  |


## getAdTree

> GetAdTree200Response getAdTree(page, limit, source, platform, status, adAccountId, accountId, profileId, fromDate, toDate)

Get campaign tree

Returns a nested Campaign &gt; Ad Set &gt; Ad hierarchy with rolled-up metrics at each level. Uses a two-stage aggregation: ads are grouped into ad sets, then ad sets into campaigns. Metrics are computed over an optional date range, then rolled up from ad level to ad set and campaign levels. Pagination is at the campaign level. Ads without a campaign or ad set ID are grouped into synthetic \&quot;Ungrouped\&quot; buckets. If no date range is provided, defaults to the last 90 days. Date range is capped at 90 days max. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdCampaignsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdCampaignsApi apiInstance = new AdCampaignsApi(defaultClient);
        Integer page = 1; // Integer | Page number (1-based)
        Integer limit = 20; // Integer | Campaigns per page
        String source = "zernio"; // String | `all` (default) returns both Zernio-created ads and those discovered from the platform's ad manager — matches the web UI's default view. Pass `zernio` to restrict to isExternal=false only. Status is NOT filtered by default — use the `status` param for that.
        String platform = "facebook"; // String | 
        AdStatus status = AdStatus.fromValue("active"); // AdStatus | Filter by derived campaign status (post-aggregation)
        String adAccountId = "adAccountId_example"; // String | Platform ad account ID
        String accountId = "accountId_example"; // String | Social account ID
        String profileId = "profileId_example"; // String | Profile ID
        LocalDate fromDate = LocalDate.now(); // LocalDate | Start of metrics date range (YYYY-MM-DD). Defaults to 90 days ago.
        LocalDate toDate = LocalDate.now(); // LocalDate | End of metrics date range (YYYY-MM-DD). Defaults to today. Max 90-day range.
        try {
            GetAdTree200Response result = apiInstance.getAdTree(page, limit, source, platform, status, adAccountId, accountId, profileId, fromDate, toDate);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdCampaignsApi#getAdTree");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **page** | **Integer**| Page number (1-based) | [optional] [default to 1] |
| **limit** | **Integer**| Campaigns per page | [optional] [default to 20] |
| **source** | **String**| &#x60;all&#x60; (default) returns both Zernio-created ads and those discovered from the platform&#39;s ad manager — matches the web UI&#39;s default view. Pass &#x60;zernio&#x60; to restrict to isExternal&#x3D;false only. Status is NOT filtered by default — use the &#x60;status&#x60; param for that. | [optional] [default to all] [enum: zernio, all] |
| **platform** | **String**|  | [optional] [enum: facebook, instagram, tiktok, linkedin, pinterest, google, twitter] |
| **status** | [**AdStatus**](.md)| Filter by derived campaign status (post-aggregation) | [optional] [enum: active, paused, pending_review, rejected, completed, cancelled, error] |
| **adAccountId** | **String**| Platform ad account ID | [optional] |
| **accountId** | **String**| Social account ID | [optional] |
| **profileId** | **String**| Profile ID | [optional] |
| **fromDate** | **LocalDate**| Start of metrics date range (YYYY-MM-DD). Defaults to 90 days ago. | [optional] |
| **toDate** | **LocalDate**| End of metrics date range (YYYY-MM-DD). Defaults to today. Max 90-day range. | [optional] |

### Return type

[**GetAdTree200Response**](GetAdTree200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Nested campaign tree with pagination |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |

## getAdTreeWithHttpInfo

> ApiResponse<GetAdTree200Response> getAdTree getAdTreeWithHttpInfo(page, limit, source, platform, status, adAccountId, accountId, profileId, fromDate, toDate)

Get campaign tree

Returns a nested Campaign &gt; Ad Set &gt; Ad hierarchy with rolled-up metrics at each level. Uses a two-stage aggregation: ads are grouped into ad sets, then ad sets into campaigns. Metrics are computed over an optional date range, then rolled up from ad level to ad set and campaign levels. Pagination is at the campaign level. Ads without a campaign or ad set ID are grouped into synthetic \&quot;Ungrouped\&quot; buckets. If no date range is provided, defaults to the last 90 days. Date range is capped at 90 days max. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdCampaignsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdCampaignsApi apiInstance = new AdCampaignsApi(defaultClient);
        Integer page = 1; // Integer | Page number (1-based)
        Integer limit = 20; // Integer | Campaigns per page
        String source = "zernio"; // String | `all` (default) returns both Zernio-created ads and those discovered from the platform's ad manager — matches the web UI's default view. Pass `zernio` to restrict to isExternal=false only. Status is NOT filtered by default — use the `status` param for that.
        String platform = "facebook"; // String | 
        AdStatus status = AdStatus.fromValue("active"); // AdStatus | Filter by derived campaign status (post-aggregation)
        String adAccountId = "adAccountId_example"; // String | Platform ad account ID
        String accountId = "accountId_example"; // String | Social account ID
        String profileId = "profileId_example"; // String | Profile ID
        LocalDate fromDate = LocalDate.now(); // LocalDate | Start of metrics date range (YYYY-MM-DD). Defaults to 90 days ago.
        LocalDate toDate = LocalDate.now(); // LocalDate | End of metrics date range (YYYY-MM-DD). Defaults to today. Max 90-day range.
        try {
            ApiResponse<GetAdTree200Response> response = apiInstance.getAdTreeWithHttpInfo(page, limit, source, platform, status, adAccountId, accountId, profileId, fromDate, toDate);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdCampaignsApi#getAdTree");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Response headers: " + e.getResponseHeaders());
            System.err.println("Reason: " + e.getResponseBody());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **page** | **Integer**| Page number (1-based) | [optional] [default to 1] |
| **limit** | **Integer**| Campaigns per page | [optional] [default to 20] |
| **source** | **String**| &#x60;all&#x60; (default) returns both Zernio-created ads and those discovered from the platform&#39;s ad manager — matches the web UI&#39;s default view. Pass &#x60;zernio&#x60; to restrict to isExternal&#x3D;false only. Status is NOT filtered by default — use the &#x60;status&#x60; param for that. | [optional] [default to all] [enum: zernio, all] |
| **platform** | **String**|  | [optional] [enum: facebook, instagram, tiktok, linkedin, pinterest, google, twitter] |
| **status** | [**AdStatus**](.md)| Filter by derived campaign status (post-aggregation) | [optional] [enum: active, paused, pending_review, rejected, completed, cancelled, error] |
| **adAccountId** | **String**| Platform ad account ID | [optional] |
| **accountId** | **String**| Social account ID | [optional] |
| **profileId** | **String**| Profile ID | [optional] |
| **fromDate** | **LocalDate**| Start of metrics date range (YYYY-MM-DD). Defaults to 90 days ago. | [optional] |
| **toDate** | **LocalDate**| End of metrics date range (YYYY-MM-DD). Defaults to today. Max 90-day range. | [optional] |

### Return type

ApiResponse<[**GetAdTree200Response**](GetAdTree200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Nested campaign tree with pagination |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |


## listAdCampaigns

> ListAdCampaigns200Response listAdCampaigns(page, limit, source, platform, status, adAccountId, accountId, profileId)

List campaigns

Returns campaigns as virtual aggregations over ad documents grouped by platform campaign ID. Metrics (spend, impressions, clicks, etc.) are summed across all ads in each campaign. Campaign status is derived from child ad statuses (active &gt; pending_review &gt; paused &gt; error &gt; completed &gt; cancelled &gt; rejected). 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdCampaignsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdCampaignsApi apiInstance = new AdCampaignsApi(defaultClient);
        Integer page = 1; // Integer | Page number (1-based)
        Integer limit = 20; // Integer | 
        String source = "zernio"; // String | `all` (default) returns both Zernio-created ads and those discovered from the platform's ad manager — matches the web UI's default view. Pass `zernio` to restrict to isExternal=false only. Status is NOT filtered by default — use the `status` param for that.
        String platform = "facebook"; // String | 
        AdStatus status = AdStatus.fromValue("active"); // AdStatus | Filter by derived campaign status (post-aggregation)
        String adAccountId = "adAccountId_example"; // String | Platform ad account ID (e.g. act_123 for Meta)
        String accountId = "accountId_example"; // String | Social account ID
        String profileId = "profileId_example"; // String | Profile ID
        try {
            ListAdCampaigns200Response result = apiInstance.listAdCampaigns(page, limit, source, platform, status, adAccountId, accountId, profileId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdCampaignsApi#listAdCampaigns");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **page** | **Integer**| Page number (1-based) | [optional] [default to 1] |
| **limit** | **Integer**|  | [optional] [default to 20] |
| **source** | **String**| &#x60;all&#x60; (default) returns both Zernio-created ads and those discovered from the platform&#39;s ad manager — matches the web UI&#39;s default view. Pass &#x60;zernio&#x60; to restrict to isExternal&#x3D;false only. Status is NOT filtered by default — use the &#x60;status&#x60; param for that. | [optional] [default to all] [enum: zernio, all] |
| **platform** | **String**|  | [optional] [enum: facebook, instagram, tiktok, linkedin, pinterest, google, twitter] |
| **status** | [**AdStatus**](.md)| Filter by derived campaign status (post-aggregation) | [optional] [enum: active, paused, pending_review, rejected, completed, cancelled, error] |
| **adAccountId** | **String**| Platform ad account ID (e.g. act_123 for Meta) | [optional] |
| **accountId** | **String**| Social account ID | [optional] |
| **profileId** | **String**| Profile ID | [optional] |

### Return type

[**ListAdCampaigns200Response**](ListAdCampaigns200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated campaigns |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |

## listAdCampaignsWithHttpInfo

> ApiResponse<ListAdCampaigns200Response> listAdCampaigns listAdCampaignsWithHttpInfo(page, limit, source, platform, status, adAccountId, accountId, profileId)

List campaigns

Returns campaigns as virtual aggregations over ad documents grouped by platform campaign ID. Metrics (spend, impressions, clicks, etc.) are summed across all ads in each campaign. Campaign status is derived from child ad statuses (active &gt; pending_review &gt; paused &gt; error &gt; completed &gt; cancelled &gt; rejected). 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdCampaignsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdCampaignsApi apiInstance = new AdCampaignsApi(defaultClient);
        Integer page = 1; // Integer | Page number (1-based)
        Integer limit = 20; // Integer | 
        String source = "zernio"; // String | `all` (default) returns both Zernio-created ads and those discovered from the platform's ad manager — matches the web UI's default view. Pass `zernio` to restrict to isExternal=false only. Status is NOT filtered by default — use the `status` param for that.
        String platform = "facebook"; // String | 
        AdStatus status = AdStatus.fromValue("active"); // AdStatus | Filter by derived campaign status (post-aggregation)
        String adAccountId = "adAccountId_example"; // String | Platform ad account ID (e.g. act_123 for Meta)
        String accountId = "accountId_example"; // String | Social account ID
        String profileId = "profileId_example"; // String | Profile ID
        try {
            ApiResponse<ListAdCampaigns200Response> response = apiInstance.listAdCampaignsWithHttpInfo(page, limit, source, platform, status, adAccountId, accountId, profileId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdCampaignsApi#listAdCampaigns");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Response headers: " + e.getResponseHeaders());
            System.err.println("Reason: " + e.getResponseBody());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **page** | **Integer**| Page number (1-based) | [optional] [default to 1] |
| **limit** | **Integer**|  | [optional] [default to 20] |
| **source** | **String**| &#x60;all&#x60; (default) returns both Zernio-created ads and those discovered from the platform&#39;s ad manager — matches the web UI&#39;s default view. Pass &#x60;zernio&#x60; to restrict to isExternal&#x3D;false only. Status is NOT filtered by default — use the &#x60;status&#x60; param for that. | [optional] [default to all] [enum: zernio, all] |
| **platform** | **String**|  | [optional] [enum: facebook, instagram, tiktok, linkedin, pinterest, google, twitter] |
| **status** | [**AdStatus**](.md)| Filter by derived campaign status (post-aggregation) | [optional] [enum: active, paused, pending_review, rejected, completed, cancelled, error] |
| **adAccountId** | **String**| Platform ad account ID (e.g. act_123 for Meta) | [optional] |
| **accountId** | **String**| Social account ID | [optional] |
| **profileId** | **String**| Profile ID | [optional] |

### Return type

ApiResponse<[**ListAdCampaigns200Response**](ListAdCampaigns200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated campaigns |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |


## updateAdCampaign

> UpdateAdCampaign200Response updateAdCampaign(campaignId, updateAdCampaignRequest)

Update a campaign (budget and/or bid strategy)

Campaign-level edits. At least one of &#x60;budget&#x60; or &#x60;bidStrategy&#x60; is required.  - &#x60;budget&#x60; updates the CBO (Campaign Budget Optimization) budget. For ABO campaigns   (where the budget lives on the ad set), use PUT /v1/ads/ad-sets/{adSetId} instead — this endpoint   will return 409 with code BUDGET_LEVEL_MISMATCH. - &#x60;bidStrategy&#x60; sets the campaign-level default bid strategy. Per Meta&#39;s spec, &#x60;bid_amount&#x60; and   &#x60;bid_constraints&#x60; do NOT exist at the campaign level — pass them via PUT /v1/ads/ad-sets/{adSetId}.  Meta-only for now. Other platforms return 501 Not Implemented. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdCampaignsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdCampaignsApi apiInstance = new AdCampaignsApi(defaultClient);
        String campaignId = "campaignId_example"; // String | Platform campaign ID
        UpdateAdCampaignRequest updateAdCampaignRequest = new UpdateAdCampaignRequest(); // UpdateAdCampaignRequest | 
        try {
            UpdateAdCampaign200Response result = apiInstance.updateAdCampaign(campaignId, updateAdCampaignRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdCampaignsApi#updateAdCampaign");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **campaignId** | **String**| Platform campaign ID | |
| **updateAdCampaignRequest** | [**UpdateAdCampaignRequest**](UpdateAdCampaignRequest.md)|  | |

### Return type

[**UpdateAdCampaign200Response**](UpdateAdCampaign200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Campaign updated |  -  |
| **400** | Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Campaign not found |  -  |
| **409** | Campaign is ABO — route to /v1/ads/ad-sets/{adSetId} instead |  -  |
| **501** | Operation not supported on this platform |  -  |

## updateAdCampaignWithHttpInfo

> ApiResponse<UpdateAdCampaign200Response> updateAdCampaign updateAdCampaignWithHttpInfo(campaignId, updateAdCampaignRequest)

Update a campaign (budget and/or bid strategy)

Campaign-level edits. At least one of &#x60;budget&#x60; or &#x60;bidStrategy&#x60; is required.  - &#x60;budget&#x60; updates the CBO (Campaign Budget Optimization) budget. For ABO campaigns   (where the budget lives on the ad set), use PUT /v1/ads/ad-sets/{adSetId} instead — this endpoint   will return 409 with code BUDGET_LEVEL_MISMATCH. - &#x60;bidStrategy&#x60; sets the campaign-level default bid strategy. Per Meta&#39;s spec, &#x60;bid_amount&#x60; and   &#x60;bid_constraints&#x60; do NOT exist at the campaign level — pass them via PUT /v1/ads/ad-sets/{adSetId}.  Meta-only for now. Other platforms return 501 Not Implemented. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdCampaignsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdCampaignsApi apiInstance = new AdCampaignsApi(defaultClient);
        String campaignId = "campaignId_example"; // String | Platform campaign ID
        UpdateAdCampaignRequest updateAdCampaignRequest = new UpdateAdCampaignRequest(); // UpdateAdCampaignRequest | 
        try {
            ApiResponse<UpdateAdCampaign200Response> response = apiInstance.updateAdCampaignWithHttpInfo(campaignId, updateAdCampaignRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdCampaignsApi#updateAdCampaign");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Response headers: " + e.getResponseHeaders());
            System.err.println("Reason: " + e.getResponseBody());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **campaignId** | **String**| Platform campaign ID | |
| **updateAdCampaignRequest** | [**UpdateAdCampaignRequest**](UpdateAdCampaignRequest.md)|  | |

### Return type

ApiResponse<[**UpdateAdCampaign200Response**](UpdateAdCampaign200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Campaign updated |  -  |
| **400** | Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Campaign not found |  -  |
| **409** | Campaign is ABO — route to /v1/ads/ad-sets/{adSetId} instead |  -  |
| **501** | Operation not supported on this platform |  -  |


## updateAdCampaignStatus

> UpdateAdCampaignStatus200Response updateAdCampaignStatus(campaignId, updateAdCampaignStatusRequest)

Pause or resume a campaign

Updates the status of all ads in a campaign. Makes one platform API call (not per-ad) since status cascades through the campaign hierarchy. Ads in terminal statuses (rejected, completed, cancelled) are automatically skipped. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdCampaignsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdCampaignsApi apiInstance = new AdCampaignsApi(defaultClient);
        String campaignId = "campaignId_example"; // String | Platform campaign ID
        UpdateAdCampaignStatusRequest updateAdCampaignStatusRequest = new UpdateAdCampaignStatusRequest(); // UpdateAdCampaignStatusRequest | 
        try {
            UpdateAdCampaignStatus200Response result = apiInstance.updateAdCampaignStatus(campaignId, updateAdCampaignStatusRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdCampaignsApi#updateAdCampaignStatus");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **campaignId** | **String**| Platform campaign ID | |
| **updateAdCampaignStatusRequest** | [**UpdateAdCampaignStatusRequest**](UpdateAdCampaignStatusRequest.md)|  | |

### Return type

[**UpdateAdCampaignStatus200Response**](UpdateAdCampaignStatus200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Campaign status updated |  -  |
| **400** | Invalid input or campaign spans multiple social accounts |  -  |
| **401** | Unauthorized |  -  |
| **404** | No ads found for this campaign |  -  |

## updateAdCampaignStatusWithHttpInfo

> ApiResponse<UpdateAdCampaignStatus200Response> updateAdCampaignStatus updateAdCampaignStatusWithHttpInfo(campaignId, updateAdCampaignStatusRequest)

Pause or resume a campaign

Updates the status of all ads in a campaign. Makes one platform API call (not per-ad) since status cascades through the campaign hierarchy. Ads in terminal statuses (rejected, completed, cancelled) are automatically skipped. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdCampaignsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdCampaignsApi apiInstance = new AdCampaignsApi(defaultClient);
        String campaignId = "campaignId_example"; // String | Platform campaign ID
        UpdateAdCampaignStatusRequest updateAdCampaignStatusRequest = new UpdateAdCampaignStatusRequest(); // UpdateAdCampaignStatusRequest | 
        try {
            ApiResponse<UpdateAdCampaignStatus200Response> response = apiInstance.updateAdCampaignStatusWithHttpInfo(campaignId, updateAdCampaignStatusRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdCampaignsApi#updateAdCampaignStatus");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Response headers: " + e.getResponseHeaders());
            System.err.println("Reason: " + e.getResponseBody());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **campaignId** | **String**| Platform campaign ID | |
| **updateAdCampaignStatusRequest** | [**UpdateAdCampaignStatusRequest**](UpdateAdCampaignStatusRequest.md)|  | |

### Return type

ApiResponse<[**UpdateAdCampaignStatus200Response**](UpdateAdCampaignStatus200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Campaign status updated |  -  |
| **400** | Invalid input or campaign spans multiple social accounts |  -  |
| **401** | Unauthorized |  -  |
| **404** | No ads found for this campaign |  -  |


## updateAdSet

> UpdateAdSet200Response updateAdSet(adSetId, updateAdSetRequest)

Update an ad set (budget, status, and/or bid strategy)

Ad-set-level writes. Use this for ABO budget updates, ad-set-scoped pause/resume, and bid-strategy edits. At least one of &#x60;budget&#x60;, &#x60;status&#x60;, or &#x60;bidStrategy&#x60; is required.  Bid strategy compatibility (per Meta&#39;s spec): - &#x60;LOWEST_COST_WITHOUT_CAP&#x60;: no &#x60;bidAmount&#x60;, no &#x60;roasAverageFloor&#x60;. - &#x60;LOWEST_COST_WITH_BID_CAP&#x60; / &#x60;COST_CAP&#x60;: &#x60;bidAmount&#x60; REQUIRED (whole currency units). - &#x60;LOWEST_COST_WITH_MIN_ROAS&#x60;: &#x60;roasAverageFloor&#x60; REQUIRED (decimal multiplier, e.g. 2.0 &#x3D; 2.0x ROAS).  When updating &#x60;budget&#x60; on an ABO campaign: if the parent campaign is CBO, the response is 409 with code BUDGET_LEVEL_MISMATCH — route to PUT /v1/ads/campaigns/{campaignId} instead. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdCampaignsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdCampaignsApi apiInstance = new AdCampaignsApi(defaultClient);
        String adSetId = "adSetId_example"; // String | Platform ad set ID
        UpdateAdSetRequest updateAdSetRequest = new UpdateAdSetRequest(); // UpdateAdSetRequest | 
        try {
            UpdateAdSet200Response result = apiInstance.updateAdSet(adSetId, updateAdSetRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdCampaignsApi#updateAdSet");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **adSetId** | **String**| Platform ad set ID | |
| **updateAdSetRequest** | [**UpdateAdSetRequest**](UpdateAdSetRequest.md)|  | |

### Return type

[**UpdateAdSet200Response**](UpdateAdSet200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Ad set updated |  -  |
| **400** | Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Ad set not found |  -  |
| **409** | Campaign is CBO — route to /v1/ads/campaigns/{campaignId} instead |  -  |
| **501** | bidStrategy not supported on the platform (Meta + TikTok only) |  -  |

## updateAdSetWithHttpInfo

> ApiResponse<UpdateAdSet200Response> updateAdSet updateAdSetWithHttpInfo(adSetId, updateAdSetRequest)

Update an ad set (budget, status, and/or bid strategy)

Ad-set-level writes. Use this for ABO budget updates, ad-set-scoped pause/resume, and bid-strategy edits. At least one of &#x60;budget&#x60;, &#x60;status&#x60;, or &#x60;bidStrategy&#x60; is required.  Bid strategy compatibility (per Meta&#39;s spec): - &#x60;LOWEST_COST_WITHOUT_CAP&#x60;: no &#x60;bidAmount&#x60;, no &#x60;roasAverageFloor&#x60;. - &#x60;LOWEST_COST_WITH_BID_CAP&#x60; / &#x60;COST_CAP&#x60;: &#x60;bidAmount&#x60; REQUIRED (whole currency units). - &#x60;LOWEST_COST_WITH_MIN_ROAS&#x60;: &#x60;roasAverageFloor&#x60; REQUIRED (decimal multiplier, e.g. 2.0 &#x3D; 2.0x ROAS).  When updating &#x60;budget&#x60; on an ABO campaign: if the parent campaign is CBO, the response is 409 with code BUDGET_LEVEL_MISMATCH — route to PUT /v1/ads/campaigns/{campaignId} instead. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdCampaignsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdCampaignsApi apiInstance = new AdCampaignsApi(defaultClient);
        String adSetId = "adSetId_example"; // String | Platform ad set ID
        UpdateAdSetRequest updateAdSetRequest = new UpdateAdSetRequest(); // UpdateAdSetRequest | 
        try {
            ApiResponse<UpdateAdSet200Response> response = apiInstance.updateAdSetWithHttpInfo(adSetId, updateAdSetRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdCampaignsApi#updateAdSet");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Response headers: " + e.getResponseHeaders());
            System.err.println("Reason: " + e.getResponseBody());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **adSetId** | **String**| Platform ad set ID | |
| **updateAdSetRequest** | [**UpdateAdSetRequest**](UpdateAdSetRequest.md)|  | |

### Return type

ApiResponse<[**UpdateAdSet200Response**](UpdateAdSet200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Ad set updated |  -  |
| **400** | Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Ad set not found |  -  |
| **409** | Campaign is CBO — route to /v1/ads/campaigns/{campaignId} instead |  -  |
| **501** | bidStrategy not supported on the platform (Meta + TikTok only) |  -  |


## updateAdSetStatus

> UpdateAdSetStatus200Response updateAdSetStatus(adSetId, updateAdCampaignStatusRequest)

Pause or resume a single ad set

Ad-set-scoped pause/resume (doesn&#39;t touch sibling ad sets). Thin wrapper over PUT /v1/ads/ad-sets/{adSetId} for callers that only want the status toggle and prefer a symmetric URL to /v1/ads/campaigns/{campaignId}/status. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdCampaignsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdCampaignsApi apiInstance = new AdCampaignsApi(defaultClient);
        String adSetId = "adSetId_example"; // String | Platform ad set ID
        UpdateAdCampaignStatusRequest updateAdCampaignStatusRequest = new UpdateAdCampaignStatusRequest(); // UpdateAdCampaignStatusRequest | 
        try {
            UpdateAdSetStatus200Response result = apiInstance.updateAdSetStatus(adSetId, updateAdCampaignStatusRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdCampaignsApi#updateAdSetStatus");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **adSetId** | **String**| Platform ad set ID | |
| **updateAdCampaignStatusRequest** | [**UpdateAdCampaignStatusRequest**](UpdateAdCampaignStatusRequest.md)|  | |

### Return type

[**UpdateAdSetStatus200Response**](UpdateAdSetStatus200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Ad set status updated |  -  |
| **400** | Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Ad set not found |  -  |

## updateAdSetStatusWithHttpInfo

> ApiResponse<UpdateAdSetStatus200Response> updateAdSetStatus updateAdSetStatusWithHttpInfo(adSetId, updateAdCampaignStatusRequest)

Pause or resume a single ad set

Ad-set-scoped pause/resume (doesn&#39;t touch sibling ad sets). Thin wrapper over PUT /v1/ads/ad-sets/{adSetId} for callers that only want the status toggle and prefer a symmetric URL to /v1/ads/campaigns/{campaignId}/status. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdCampaignsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdCampaignsApi apiInstance = new AdCampaignsApi(defaultClient);
        String adSetId = "adSetId_example"; // String | Platform ad set ID
        UpdateAdCampaignStatusRequest updateAdCampaignStatusRequest = new UpdateAdCampaignStatusRequest(); // UpdateAdCampaignStatusRequest | 
        try {
            ApiResponse<UpdateAdSetStatus200Response> response = apiInstance.updateAdSetStatusWithHttpInfo(adSetId, updateAdCampaignStatusRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdCampaignsApi#updateAdSetStatus");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Response headers: " + e.getResponseHeaders());
            System.err.println("Reason: " + e.getResponseBody());
            e.printStackTrace();
        }
    }
}
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **adSetId** | **String**| Platform ad set ID | |
| **updateAdCampaignStatusRequest** | [**UpdateAdCampaignStatusRequest**](UpdateAdCampaignStatusRequest.md)|  | |

### Return type

ApiResponse<[**UpdateAdSetStatus200Response**](UpdateAdSetStatus200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Ad set status updated |  -  |
| **400** | Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Ad set not found |  -  |

