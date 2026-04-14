# AdCampaignsApi

All URIs are relative to *https://zernio.com/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getAdTree**](AdCampaignsApi.md#getAdTree) | **GET** /v1/ads/tree | Get campaign tree |
| [**getAdTreeWithHttpInfo**](AdCampaignsApi.md#getAdTreeWithHttpInfo) | **GET** /v1/ads/tree | Get campaign tree |
| [**listAdCampaigns**](AdCampaignsApi.md#listAdCampaigns) | **GET** /v1/ads/campaigns | List campaigns |
| [**listAdCampaignsWithHttpInfo**](AdCampaignsApi.md#listAdCampaignsWithHttpInfo) | **GET** /v1/ads/campaigns | List campaigns |
| [**updateAdCampaignStatus**](AdCampaignsApi.md#updateAdCampaignStatus) | **PUT** /v1/ads/campaigns/{campaignId}/status | Pause or resume a campaign |
| [**updateAdCampaignStatusWithHttpInfo**](AdCampaignsApi.md#updateAdCampaignStatusWithHttpInfo) | **PUT** /v1/ads/campaigns/{campaignId}/status | Pause or resume a campaign |



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
        String source = "zernio"; // String | 
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
| **source** | **String**|  | [optional] [default to zernio] [enum: zernio, all] |
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
        String source = "zernio"; // String | 
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
| **source** | **String**|  | [optional] [default to zernio] [enum: zernio, all] |
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
        String source = "zernio"; // String | 
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
| **source** | **String**|  | [optional] [default to zernio] [enum: zernio, all] |
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
        String source = "zernio"; // String | 
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
| **source** | **String**|  | [optional] [default to zernio] [enum: zernio, all] |
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

