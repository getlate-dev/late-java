# AdsApi

All URIs are relative to *https://zernio.com/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**boostPost**](AdsApi.md#boostPost) | **POST** /v1/ads/boost | Boost post as ad |
| [**boostPostWithHttpInfo**](AdsApi.md#boostPostWithHttpInfo) | **POST** /v1/ads/boost | Boost post as ad |
| [**createStandaloneAd**](AdsApi.md#createStandaloneAd) | **POST** /v1/ads/create | Create standalone ad |
| [**createStandaloneAdWithHttpInfo**](AdsApi.md#createStandaloneAdWithHttpInfo) | **POST** /v1/ads/create | Create standalone ad |
| [**deleteAd**](AdsApi.md#deleteAd) | **DELETE** /v1/ads/{adId} | Cancel an ad |
| [**deleteAdWithHttpInfo**](AdsApi.md#deleteAdWithHttpInfo) | **DELETE** /v1/ads/{adId} | Cancel an ad |
| [**getAd**](AdsApi.md#getAd) | **GET** /v1/ads/{adId} | Get ad details |
| [**getAdWithHttpInfo**](AdsApi.md#getAdWithHttpInfo) | **GET** /v1/ads/{adId} | Get ad details |
| [**getAdAnalytics**](AdsApi.md#getAdAnalytics) | **GET** /v1/ads/{adId}/analytics | Get ad analytics |
| [**getAdAnalyticsWithHttpInfo**](AdsApi.md#getAdAnalyticsWithHttpInfo) | **GET** /v1/ads/{adId}/analytics | Get ad analytics |
| [**listAdAccounts**](AdsApi.md#listAdAccounts) | **GET** /v1/ads/accounts | List ad accounts |
| [**listAdAccountsWithHttpInfo**](AdsApi.md#listAdAccountsWithHttpInfo) | **GET** /v1/ads/accounts | List ad accounts |
| [**listAds**](AdsApi.md#listAds) | **GET** /v1/ads | List ads |
| [**listAdsWithHttpInfo**](AdsApi.md#listAdsWithHttpInfo) | **GET** /v1/ads | List ads |
| [**listConversionDestinations**](AdsApi.md#listConversionDestinations) | **GET** /v1/accounts/{accountId}/conversion-destinations | List destinations for the Conversions API |
| [**listConversionDestinationsWithHttpInfo**](AdsApi.md#listConversionDestinationsWithHttpInfo) | **GET** /v1/accounts/{accountId}/conversion-destinations | List destinations for the Conversions API |
| [**searchAdInterests**](AdsApi.md#searchAdInterests) | **GET** /v1/ads/interests | Search targeting interests |
| [**searchAdInterestsWithHttpInfo**](AdsApi.md#searchAdInterestsWithHttpInfo) | **GET** /v1/ads/interests | Search targeting interests |
| [**sendConversions**](AdsApi.md#sendConversions) | **POST** /v1/ads/conversions | Send conversion events to an ad platform |
| [**sendConversionsWithHttpInfo**](AdsApi.md#sendConversionsWithHttpInfo) | **POST** /v1/ads/conversions | Send conversion events to an ad platform |
| [**updateAd**](AdsApi.md#updateAd) | **PUT** /v1/ads/{adId} | Update ad |
| [**updateAdWithHttpInfo**](AdsApi.md#updateAdWithHttpInfo) | **PUT** /v1/ads/{adId} | Update ad |



## boostPost

> UpdateAd200Response boostPost(boostPostRequest)

Boost post as ad

Creates a paid ad campaign from an existing published post. Creates the full platform campaign hierarchy (campaign, ad set, ad).

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        BoostPostRequest boostPostRequest = new BoostPostRequest(); // BoostPostRequest | 
        try {
            UpdateAd200Response result = apiInstance.boostPost(boostPostRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#boostPost");
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
| **boostPostRequest** | [**BoostPostRequest**](BoostPostRequest.md)|  | |

### Return type

[**UpdateAd200Response**](UpdateAd200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Ad created |  -  |
| **400** | Missing required fields or invalid values |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **422** | Platform ads connection required (TikTok Ads, X Ads) or missing linked account |  -  |

## boostPostWithHttpInfo

> ApiResponse<UpdateAd200Response> boostPost boostPostWithHttpInfo(boostPostRequest)

Boost post as ad

Creates a paid ad campaign from an existing published post. Creates the full platform campaign hierarchy (campaign, ad set, ad).

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        BoostPostRequest boostPostRequest = new BoostPostRequest(); // BoostPostRequest | 
        try {
            ApiResponse<UpdateAd200Response> response = apiInstance.boostPostWithHttpInfo(boostPostRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#boostPost");
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
| **boostPostRequest** | [**BoostPostRequest**](BoostPostRequest.md)|  | |

### Return type

ApiResponse<[**UpdateAd200Response**](UpdateAd200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Ad created |  -  |
| **400** | Missing required fields or invalid values |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **422** | Platform ads connection required (TikTok Ads, X Ads) or missing linked account |  -  |


## createStandaloneAd

> CreateStandaloneAd201Response createStandaloneAd(createStandaloneAdRequest)

Create standalone ad

Creates a paid ad with custom creative. The request body supports three mutually-exclusive shapes:  1. **Legacy single-creative** (all platforms). Top-level &#x60;headline&#x60; + &#x60;body&#x60; + &#x60;imageUrl&#x60; + &#x60;linkUrl&#x60; + &#x60;callToAction&#x60; create 1 campaign + 1 ad set + 1 ad. 2. **Multi-creative** (Meta only — use &#x60;creatives[]&#x60; array). Creates 1 campaign + 1 ad set + N ads sharing the same budget / targeting / schedule. This is the standard performance-marketing creative-testing flow — Meta&#39;s delivery algorithm A/B tests the creatives inside a single ad set so budget isn&#39;t fragmented across N parallel campaigns. 3. **Attach to existing ad set** (Meta only — pass &#x60;adSetId&#x60; + a single creative). Adds one new ad to an existing ad set without creating a new campaign. Budget, targeting, goal are inherited from the ad set on Meta.  &#x60;creatives[]&#x60; and &#x60;adSetId&#x60; are mutually exclusive; specifying both returns 400. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        CreateStandaloneAdRequest createStandaloneAdRequest = new CreateStandaloneAdRequest(); // CreateStandaloneAdRequest | 
        try {
            CreateStandaloneAd201Response result = apiInstance.createStandaloneAd(createStandaloneAdRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#createStandaloneAd");
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
| **createStandaloneAdRequest** | [**CreateStandaloneAdRequest**](CreateStandaloneAdRequest.md)|  | |

### Return type

[**CreateStandaloneAd201Response**](CreateStandaloneAd201Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Ad(s) created |  -  |
| **400** | Missing required fields, invalid values, or non-Meta platform used with creatives[] / adSetId |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **422** | Platform ads connection required (TikTok Ads, X Ads) or missing linked account |  -  |

## createStandaloneAdWithHttpInfo

> ApiResponse<CreateStandaloneAd201Response> createStandaloneAd createStandaloneAdWithHttpInfo(createStandaloneAdRequest)

Create standalone ad

Creates a paid ad with custom creative. The request body supports three mutually-exclusive shapes:  1. **Legacy single-creative** (all platforms). Top-level &#x60;headline&#x60; + &#x60;body&#x60; + &#x60;imageUrl&#x60; + &#x60;linkUrl&#x60; + &#x60;callToAction&#x60; create 1 campaign + 1 ad set + 1 ad. 2. **Multi-creative** (Meta only — use &#x60;creatives[]&#x60; array). Creates 1 campaign + 1 ad set + N ads sharing the same budget / targeting / schedule. This is the standard performance-marketing creative-testing flow — Meta&#39;s delivery algorithm A/B tests the creatives inside a single ad set so budget isn&#39;t fragmented across N parallel campaigns. 3. **Attach to existing ad set** (Meta only — pass &#x60;adSetId&#x60; + a single creative). Adds one new ad to an existing ad set without creating a new campaign. Budget, targeting, goal are inherited from the ad set on Meta.  &#x60;creatives[]&#x60; and &#x60;adSetId&#x60; are mutually exclusive; specifying both returns 400. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        CreateStandaloneAdRequest createStandaloneAdRequest = new CreateStandaloneAdRequest(); // CreateStandaloneAdRequest | 
        try {
            ApiResponse<CreateStandaloneAd201Response> response = apiInstance.createStandaloneAdWithHttpInfo(createStandaloneAdRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#createStandaloneAd");
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
| **createStandaloneAdRequest** | [**CreateStandaloneAdRequest**](CreateStandaloneAdRequest.md)|  | |

### Return type

ApiResponse<[**CreateStandaloneAd201Response**](CreateStandaloneAd201Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Ad(s) created |  -  |
| **400** | Missing required fields, invalid values, or non-Meta platform used with creatives[] / adSetId |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **422** | Platform ads connection required (TikTok Ads, X Ads) or missing linked account |  -  |


## deleteAd

> DeleteAccountGroup200Response deleteAd(adId)

Cancel an ad

Cancels the ad on the platform and marks it as cancelled in the database. The ad is preserved for history.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        String adId = "adId_example"; // String | 
        try {
            DeleteAccountGroup200Response result = apiInstance.deleteAd(adId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#deleteAd");
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
| **adId** | **String**|  | |

### Return type

[**DeleteAccountGroup200Response**](DeleteAccountGroup200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Ad cancelled |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## deleteAdWithHttpInfo

> ApiResponse<DeleteAccountGroup200Response> deleteAd deleteAdWithHttpInfo(adId)

Cancel an ad

Cancels the ad on the platform and marks it as cancelled in the database. The ad is preserved for history.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        String adId = "adId_example"; // String | 
        try {
            ApiResponse<DeleteAccountGroup200Response> response = apiInstance.deleteAdWithHttpInfo(adId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#deleteAd");
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
| **adId** | **String**|  | |

### Return type

ApiResponse<[**DeleteAccountGroup200Response**](DeleteAccountGroup200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Ad cancelled |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## getAd

> GetAd200Response getAd(adId)

Get ad details

Returns an ad with its creative, targeting, status, and performance metrics.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        String adId = "adId_example"; // String | 
        try {
            GetAd200Response result = apiInstance.getAd(adId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#getAd");
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
| **adId** | **String**|  | |

### Return type

[**GetAd200Response**](GetAd200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Ad details |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## getAdWithHttpInfo

> ApiResponse<GetAd200Response> getAd getAdWithHttpInfo(adId)

Get ad details

Returns an ad with its creative, targeting, status, and performance metrics.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        String adId = "adId_example"; // String | 
        try {
            ApiResponse<GetAd200Response> response = apiInstance.getAdWithHttpInfo(adId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#getAd");
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
| **adId** | **String**|  | |

### Return type

ApiResponse<[**GetAd200Response**](GetAd200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Ad details |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## getAdAnalytics

> GetAdAnalytics200Response getAdAnalytics(adId, fromDate, toDate, breakdowns)

Get ad analytics

Returns detailed performance analytics for an ad. Includes summary metrics, a daily timeline over the requested date range, and optional demographic breakdowns (Meta and TikTok only). If no date range is provided, defaults to the last 90 days. Date range is capped at 90 days max. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        String adId = "adId_example"; // String | 
        LocalDate fromDate = LocalDate.now(); // LocalDate | Start of date range (YYYY-MM-DD). Defaults to 90 days ago.
        LocalDate toDate = LocalDate.now(); // LocalDate | End of date range (YYYY-MM-DD). Defaults to today. Max 90-day range.
        String breakdowns = "breakdowns_example"; // String | Comma-separated breakdown dimensions. Meta: age, gender, country, publisher_platform, device_platform, region. TikTok: gender, age, country_code, platform, ac, language.
        try {
            GetAdAnalytics200Response result = apiInstance.getAdAnalytics(adId, fromDate, toDate, breakdowns);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#getAdAnalytics");
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
| **adId** | **String**|  | |
| **fromDate** | **LocalDate**| Start of date range (YYYY-MM-DD). Defaults to 90 days ago. | [optional] |
| **toDate** | **LocalDate**| End of date range (YYYY-MM-DD). Defaults to today. Max 90-day range. | [optional] |
| **breakdowns** | **String**| Comma-separated breakdown dimensions. Meta: age, gender, country, publisher_platform, device_platform, region. TikTok: gender, age, country_code, platform, ac, language. | [optional] |

### Return type

[**GetAdAnalytics200Response**](GetAdAnalytics200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Ad analytics |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Resource not found |  -  |

## getAdAnalyticsWithHttpInfo

> ApiResponse<GetAdAnalytics200Response> getAdAnalytics getAdAnalyticsWithHttpInfo(adId, fromDate, toDate, breakdowns)

Get ad analytics

Returns detailed performance analytics for an ad. Includes summary metrics, a daily timeline over the requested date range, and optional demographic breakdowns (Meta and TikTok only). If no date range is provided, defaults to the last 90 days. Date range is capped at 90 days max. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        String adId = "adId_example"; // String | 
        LocalDate fromDate = LocalDate.now(); // LocalDate | Start of date range (YYYY-MM-DD). Defaults to 90 days ago.
        LocalDate toDate = LocalDate.now(); // LocalDate | End of date range (YYYY-MM-DD). Defaults to today. Max 90-day range.
        String breakdowns = "breakdowns_example"; // String | Comma-separated breakdown dimensions. Meta: age, gender, country, publisher_platform, device_platform, region. TikTok: gender, age, country_code, platform, ac, language.
        try {
            ApiResponse<GetAdAnalytics200Response> response = apiInstance.getAdAnalyticsWithHttpInfo(adId, fromDate, toDate, breakdowns);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#getAdAnalytics");
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
| **adId** | **String**|  | |
| **fromDate** | **LocalDate**| Start of date range (YYYY-MM-DD). Defaults to 90 days ago. | [optional] |
| **toDate** | **LocalDate**| End of date range (YYYY-MM-DD). Defaults to today. Max 90-day range. | [optional] |
| **breakdowns** | **String**| Comma-separated breakdown dimensions. Meta: age, gender, country, publisher_platform, device_platform, region. TikTok: gender, age, country_code, platform, ac, language. | [optional] |

### Return type

ApiResponse<[**GetAdAnalytics200Response**](GetAdAnalytics200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Ad analytics |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Resource not found |  -  |


## listAdAccounts

> ListAdAccounts200Response listAdAccounts(accountId)

List ad accounts

Returns the platform ad accounts available for the given social account (e.g. Meta ad accounts, TikTok advertiser IDs, Google Ads customer IDs).

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        String accountId = "accountId_example"; // String | Social account ID
        try {
            ListAdAccounts200Response result = apiInstance.listAdAccounts(accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#listAdAccounts");
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
| **accountId** | **String**| Social account ID | |

### Return type

[**ListAdAccounts200Response**](ListAdAccounts200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Ad accounts |  -  |
| **401** | Unauthorized |  -  |
| **422** | Platform ads connection required (TikTok Ads, X Ads) or Instagram missing linked Facebook account |  -  |

## listAdAccountsWithHttpInfo

> ApiResponse<ListAdAccounts200Response> listAdAccounts listAdAccountsWithHttpInfo(accountId)

List ad accounts

Returns the platform ad accounts available for the given social account (e.g. Meta ad accounts, TikTok advertiser IDs, Google Ads customer IDs).

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        String accountId = "accountId_example"; // String | Social account ID
        try {
            ApiResponse<ListAdAccounts200Response> response = apiInstance.listAdAccountsWithHttpInfo(accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#listAdAccounts");
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
| **accountId** | **String**| Social account ID | |

### Return type

ApiResponse<[**ListAdAccounts200Response**](ListAdAccounts200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Ad accounts |  -  |
| **401** | Unauthorized |  -  |
| **422** | Platform ads connection required (TikTok Ads, X Ads) or Instagram missing linked Facebook account |  -  |


## listAds

> ListAds200Response listAds(page, limit, source, status, platform, accountId, adAccountId, profileId, campaignId, fromDate, toDate)

List ads

Returns a paginated list of ads with metrics computed over an optional date range. Use source&#x3D;all to include externally-synced ads from platform ad managers. If no date range is provided, defaults to the last 90 days. Date range is capped at 90 days max. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        Integer page = 1; // Integer | Page number (1-based)
        Integer limit = 50; // Integer | 
        String source = "zernio"; // String | all (default) = Zernio-created + platform-discovered ads. zernio = restrict to Zernio-created only.
        AdStatus status = AdStatus.fromValue("active"); // AdStatus | 
        String platform = "facebook"; // String | 
        String accountId = "accountId_example"; // String | Social account ID
        String adAccountId = "adAccountId_example"; // String | Platform ad account ID (e.g. act_123 for Meta). Mirrors the same filter on /v1/ads/campaigns and /v1/ads/tree.
        String profileId = "profileId_example"; // String | Profile ID
        String campaignId = "campaignId_example"; // String | Platform campaign ID (filter ads within a campaign)
        LocalDate fromDate = LocalDate.now(); // LocalDate | Start of metrics date range (YYYY-MM-DD). Defaults to 90 days ago.
        LocalDate toDate = LocalDate.now(); // LocalDate | End of metrics date range (YYYY-MM-DD). Defaults to today. Max 90-day range.
        try {
            ListAds200Response result = apiInstance.listAds(page, limit, source, status, platform, accountId, adAccountId, profileId, campaignId, fromDate, toDate);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#listAds");
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
| **limit** | **Integer**|  | [optional] [default to 50] |
| **source** | **String**| all (default) &#x3D; Zernio-created + platform-discovered ads. zernio &#x3D; restrict to Zernio-created only. | [optional] [default to all] [enum: zernio, all] |
| **status** | [**AdStatus**](.md)|  | [optional] [enum: active, paused, pending_review, rejected, completed, cancelled, error] |
| **platform** | **String**|  | [optional] [enum: facebook, instagram, tiktok, linkedin, pinterest, google, twitter] |
| **accountId** | **String**| Social account ID | [optional] |
| **adAccountId** | **String**| Platform ad account ID (e.g. act_123 for Meta). Mirrors the same filter on /v1/ads/campaigns and /v1/ads/tree. | [optional] |
| **profileId** | **String**| Profile ID | [optional] |
| **campaignId** | **String**| Platform campaign ID (filter ads within a campaign) | [optional] |
| **fromDate** | **LocalDate**| Start of metrics date range (YYYY-MM-DD). Defaults to 90 days ago. | [optional] |
| **toDate** | **LocalDate**| End of metrics date range (YYYY-MM-DD). Defaults to today. Max 90-day range. | [optional] |

### Return type

[**ListAds200Response**](ListAds200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated ads |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |

## listAdsWithHttpInfo

> ApiResponse<ListAds200Response> listAds listAdsWithHttpInfo(page, limit, source, status, platform, accountId, adAccountId, profileId, campaignId, fromDate, toDate)

List ads

Returns a paginated list of ads with metrics computed over an optional date range. Use source&#x3D;all to include externally-synced ads from platform ad managers. If no date range is provided, defaults to the last 90 days. Date range is capped at 90 days max. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        Integer page = 1; // Integer | Page number (1-based)
        Integer limit = 50; // Integer | 
        String source = "zernio"; // String | all (default) = Zernio-created + platform-discovered ads. zernio = restrict to Zernio-created only.
        AdStatus status = AdStatus.fromValue("active"); // AdStatus | 
        String platform = "facebook"; // String | 
        String accountId = "accountId_example"; // String | Social account ID
        String adAccountId = "adAccountId_example"; // String | Platform ad account ID (e.g. act_123 for Meta). Mirrors the same filter on /v1/ads/campaigns and /v1/ads/tree.
        String profileId = "profileId_example"; // String | Profile ID
        String campaignId = "campaignId_example"; // String | Platform campaign ID (filter ads within a campaign)
        LocalDate fromDate = LocalDate.now(); // LocalDate | Start of metrics date range (YYYY-MM-DD). Defaults to 90 days ago.
        LocalDate toDate = LocalDate.now(); // LocalDate | End of metrics date range (YYYY-MM-DD). Defaults to today. Max 90-day range.
        try {
            ApiResponse<ListAds200Response> response = apiInstance.listAdsWithHttpInfo(page, limit, source, status, platform, accountId, adAccountId, profileId, campaignId, fromDate, toDate);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#listAds");
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
| **limit** | **Integer**|  | [optional] [default to 50] |
| **source** | **String**| all (default) &#x3D; Zernio-created + platform-discovered ads. zernio &#x3D; restrict to Zernio-created only. | [optional] [default to all] [enum: zernio, all] |
| **status** | [**AdStatus**](.md)|  | [optional] [enum: active, paused, pending_review, rejected, completed, cancelled, error] |
| **platform** | **String**|  | [optional] [enum: facebook, instagram, tiktok, linkedin, pinterest, google, twitter] |
| **accountId** | **String**| Social account ID | [optional] |
| **adAccountId** | **String**| Platform ad account ID (e.g. act_123 for Meta). Mirrors the same filter on /v1/ads/campaigns and /v1/ads/tree. | [optional] |
| **profileId** | **String**| Profile ID | [optional] |
| **campaignId** | **String**| Platform campaign ID (filter ads within a campaign) | [optional] |
| **fromDate** | **LocalDate**| Start of metrics date range (YYYY-MM-DD). Defaults to 90 days ago. | [optional] |
| **toDate** | **LocalDate**| End of metrics date range (YYYY-MM-DD). Defaults to today. Max 90-day range. | [optional] |

### Return type

ApiResponse<[**ListAds200Response**](ListAds200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated ads |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |


## listConversionDestinations

> ListConversionDestinations200Response listConversionDestinations(accountId)

List destinations for the Conversions API

Returns the list of pixels (Meta) or conversion actions (Google) accessible to the connected ads account. Use the returned &#x60;id&#x60; as &#x60;destinationId&#x60; when posting to &#x60;POST /v1/ads/conversions&#x60;.  For Google, each destination&#39;s &#x60;type&#x60; reflects the conversion action&#39;s category (PURCHASE, LEAD, SIGN_UP, etc.) — the event type is locked to the destination. For Meta, &#x60;type&#x60; is absent: pixels accept any event name per request. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        String accountId = "accountId_example"; // String | SocialAccount ID (metaads or googleads).
        try {
            ListConversionDestinations200Response result = apiInstance.listConversionDestinations(accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#listConversionDestinations");
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
| **accountId** | **String**| SocialAccount ID (metaads or googleads). | |

### Return type

[**ListConversionDestinations200Response**](ListConversionDestinations200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Destinations listed |  -  |
| **400** | Account&#39;s platform is not supported by the Conversions API. |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required. |  -  |
| **404** | Account not found or not accessible. |  -  |

## listConversionDestinationsWithHttpInfo

> ApiResponse<ListConversionDestinations200Response> listConversionDestinations listConversionDestinationsWithHttpInfo(accountId)

List destinations for the Conversions API

Returns the list of pixels (Meta) or conversion actions (Google) accessible to the connected ads account. Use the returned &#x60;id&#x60; as &#x60;destinationId&#x60; when posting to &#x60;POST /v1/ads/conversions&#x60;.  For Google, each destination&#39;s &#x60;type&#x60; reflects the conversion action&#39;s category (PURCHASE, LEAD, SIGN_UP, etc.) — the event type is locked to the destination. For Meta, &#x60;type&#x60; is absent: pixels accept any event name per request. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        String accountId = "accountId_example"; // String | SocialAccount ID (metaads or googleads).
        try {
            ApiResponse<ListConversionDestinations200Response> response = apiInstance.listConversionDestinationsWithHttpInfo(accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#listConversionDestinations");
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
| **accountId** | **String**| SocialAccount ID (metaads or googleads). | |

### Return type

ApiResponse<[**ListConversionDestinations200Response**](ListConversionDestinations200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Destinations listed |  -  |
| **400** | Account&#39;s platform is not supported by the Conversions API. |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required. |  -  |
| **404** | Account not found or not accessible. |  -  |


## searchAdInterests

> SearchAdInterests200Response searchAdInterests(q, accountId)

Search targeting interests

Search for interest-based targeting options available on the platform.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        String q = "q_example"; // String | Search query
        String accountId = "accountId_example"; // String | Social account ID
        try {
            SearchAdInterests200Response result = apiInstance.searchAdInterests(q, accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#searchAdInterests");
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
| **q** | **String**| Search query | |
| **accountId** | **String**| Social account ID | |

### Return type

[**SearchAdInterests200Response**](SearchAdInterests200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Matching interests |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |

## searchAdInterestsWithHttpInfo

> ApiResponse<SearchAdInterests200Response> searchAdInterests searchAdInterestsWithHttpInfo(q, accountId)

Search targeting interests

Search for interest-based targeting options available on the platform.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        String q = "q_example"; // String | Search query
        String accountId = "accountId_example"; // String | Social account ID
        try {
            ApiResponse<SearchAdInterests200Response> response = apiInstance.searchAdInterestsWithHttpInfo(q, accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#searchAdInterests");
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
| **q** | **String**| Search query | |
| **accountId** | **String**| Social account ID | |

### Return type

ApiResponse<[**SearchAdInterests200Response**](SearchAdInterests200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Matching interests |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |


## sendConversions

> SendConversions200Response sendConversions(sendConversionsRequest)

Send conversion events to an ad platform

Relay one or more conversion events to the target ad platform&#39;s native Conversions API. Supported platforms: Meta (metaads) via Graph API, Google Ads (googleads) via Data Manager API &#x60;ingestEvents&#x60;.  Platform is inferred from the provided &#x60;accountId&#x60;. &#x60;destinationId&#x60; semantics differ per platform: - Meta: pixel (dataset) ID, e.g. \&quot;123456789012345\&quot; - Google: conversion action resource name, e.g.   \&quot;customers/1234567890/conversionActions/987654321\&quot;  Callers can list valid destinations via &#x60;GET /v1/accounts/{accountId}/conversion-destinations&#x60;.  All PII (email, phone, names, external IDs) is hashed with SHA-256 server-side per each platform&#39;s normalization spec (including Google&#39;s Gmail-specific dot/plus-suffix stripping). Send plaintext.  Requires the Ads add-on.  Batching: Meta caps at 1000 events per request and rejects the entire batch if any event is malformed. Google caps at 2000. Both are handled automatically by chunking.  Dedup: pass a stable &#x60;eventId&#x60; on every event. Meta uses it to dedupe against pixel events; Google maps it to transactionId. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        SendConversionsRequest sendConversionsRequest = new SendConversionsRequest(); // SendConversionsRequest | 
        try {
            SendConversions200Response result = apiInstance.sendConversions(sendConversionsRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#sendConversions");
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
| **sendConversionsRequest** | [**SendConversionsRequest**](SendConversionsRequest.md)|  | |

### Return type

[**SendConversions200Response**](SendConversions200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Events processed. Inspect &#x60;eventsFailed&#x60; and &#x60;failures[]&#x60; to detect partial failure. For Meta, a batch is all-or-nothing (either every event in a chunk succeeds, or every event in the chunk is listed in failures). For Google, the API returns success/failure at the request level only.  |  -  |
| **400** | Invalid body (missing accountId/destinationId/events, malformed event shape). |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required. |  -  |
| **404** | Account not found or not accessible. |  -  |

## sendConversionsWithHttpInfo

> ApiResponse<SendConversions200Response> sendConversions sendConversionsWithHttpInfo(sendConversionsRequest)

Send conversion events to an ad platform

Relay one or more conversion events to the target ad platform&#39;s native Conversions API. Supported platforms: Meta (metaads) via Graph API, Google Ads (googleads) via Data Manager API &#x60;ingestEvents&#x60;.  Platform is inferred from the provided &#x60;accountId&#x60;. &#x60;destinationId&#x60; semantics differ per platform: - Meta: pixel (dataset) ID, e.g. \&quot;123456789012345\&quot; - Google: conversion action resource name, e.g.   \&quot;customers/1234567890/conversionActions/987654321\&quot;  Callers can list valid destinations via &#x60;GET /v1/accounts/{accountId}/conversion-destinations&#x60;.  All PII (email, phone, names, external IDs) is hashed with SHA-256 server-side per each platform&#39;s normalization spec (including Google&#39;s Gmail-specific dot/plus-suffix stripping). Send plaintext.  Requires the Ads add-on.  Batching: Meta caps at 1000 events per request and rejects the entire batch if any event is malformed. Google caps at 2000. Both are handled automatically by chunking.  Dedup: pass a stable &#x60;eventId&#x60; on every event. Meta uses it to dedupe against pixel events; Google maps it to transactionId. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        SendConversionsRequest sendConversionsRequest = new SendConversionsRequest(); // SendConversionsRequest | 
        try {
            ApiResponse<SendConversions200Response> response = apiInstance.sendConversionsWithHttpInfo(sendConversionsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#sendConversions");
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
| **sendConversionsRequest** | [**SendConversionsRequest**](SendConversionsRequest.md)|  | |

### Return type

ApiResponse<[**SendConversions200Response**](SendConversions200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Events processed. Inspect &#x60;eventsFailed&#x60; and &#x60;failures[]&#x60; to detect partial failure. For Meta, a batch is all-or-nothing (either every event in a chunk succeeds, or every event in the chunk is listed in failures). For Google, the API returns success/failure at the request level only.  |  -  |
| **400** | Invalid body (missing accountId/destinationId/events, malformed event shape). |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required. |  -  |
| **404** | Account not found or not accessible. |  -  |


## updateAd

> UpdateAd200Response updateAd(adId, updateAdRequest)

Update ad

Update one or more fields on an ad. Status changes and budget updates are propagated to the platform. Targeting updates are Meta-only.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        String adId = "adId_example"; // String | 
        UpdateAdRequest updateAdRequest = new UpdateAdRequest(); // UpdateAdRequest | 
        try {
            UpdateAd200Response result = apiInstance.updateAd(adId, updateAdRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#updateAd");
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
| **adId** | **String**|  | |
| **updateAdRequest** | [**UpdateAdRequest**](UpdateAdRequest.md)|  | |

### Return type

[**UpdateAd200Response**](UpdateAd200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Ad updated |  -  |
| **400** | Invalid status transition or budget below minimum |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## updateAdWithHttpInfo

> ApiResponse<UpdateAd200Response> updateAd updateAdWithHttpInfo(adId, updateAdRequest)

Update ad

Update one or more fields on an ad. Status changes and budget updates are propagated to the platform. Targeting updates are Meta-only.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdsApi apiInstance = new AdsApi(defaultClient);
        String adId = "adId_example"; // String | 
        UpdateAdRequest updateAdRequest = new UpdateAdRequest(); // UpdateAdRequest | 
        try {
            ApiResponse<UpdateAd200Response> response = apiInstance.updateAdWithHttpInfo(adId, updateAdRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdsApi#updateAd");
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
| **adId** | **String**|  | |
| **updateAdRequest** | [**UpdateAdRequest**](UpdateAdRequest.md)|  | |

### Return type

ApiResponse<[**UpdateAd200Response**](UpdateAd200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Ad updated |  -  |
| **400** | Invalid status transition or budget below minimum |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

