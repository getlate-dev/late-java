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
| [**searchAdInterests**](AdsApi.md#searchAdInterests) | **GET** /v1/ads/interests | Search targeting interests |
| [**searchAdInterestsWithHttpInfo**](AdsApi.md#searchAdInterestsWithHttpInfo) | **GET** /v1/ads/interests | Search targeting interests |
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

> UpdateAd200Response createStandaloneAd(createStandaloneAdRequest)

Create standalone ad

Creates a paid ad with custom creative (headline, body, image/video, link). Creates the full platform campaign hierarchy.

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
            UpdateAd200Response result = apiInstance.createStandaloneAd(createStandaloneAdRequest);
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

## createStandaloneAdWithHttpInfo

> ApiResponse<UpdateAd200Response> createStandaloneAd createStandaloneAdWithHttpInfo(createStandaloneAdRequest)

Create standalone ad

Creates a paid ad with custom creative (headline, body, image/video, link). Creates the full platform campaign hierarchy.

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
            ApiResponse<UpdateAd200Response> response = apiInstance.createStandaloneAdWithHttpInfo(createStandaloneAdRequest);
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
        String source = "zernio"; // String | zernio = Zernio-created only, all = include external ads
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
| **source** | **String**| zernio &#x3D; Zernio-created only, all &#x3D; include external ads | [optional] [default to zernio] [enum: zernio, all] |
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
        String source = "zernio"; // String | zernio = Zernio-created only, all = include external ads
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
| **source** | **String**| zernio &#x3D; Zernio-created only, all &#x3D; include external ads | [optional] [default to zernio] [enum: zernio, all] |
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

