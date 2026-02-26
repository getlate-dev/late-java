# AnalyticsApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getAnalytics**](AnalyticsApi.md#getAnalytics) | **GET** /v1/analytics | Get post analytics |
| [**getAnalyticsWithHttpInfo**](AnalyticsApi.md#getAnalyticsWithHttpInfo) | **GET** /v1/analytics | Get post analytics |
| [**getBestTimeToPost**](AnalyticsApi.md#getBestTimeToPost) | **GET** /v1/analytics/best-time | Get best times to post |
| [**getBestTimeToPostWithHttpInfo**](AnalyticsApi.md#getBestTimeToPostWithHttpInfo) | **GET** /v1/analytics/best-time | Get best times to post |
| [**getContentDecay**](AnalyticsApi.md#getContentDecay) | **GET** /v1/analytics/content-decay | Get content performance decay |
| [**getContentDecayWithHttpInfo**](AnalyticsApi.md#getContentDecayWithHttpInfo) | **GET** /v1/analytics/content-decay | Get content performance decay |
| [**getDailyMetrics**](AnalyticsApi.md#getDailyMetrics) | **GET** /v1/analytics/daily-metrics | Get daily aggregated metrics |
| [**getDailyMetricsWithHttpInfo**](AnalyticsApi.md#getDailyMetricsWithHttpInfo) | **GET** /v1/analytics/daily-metrics | Get daily aggregated metrics |
| [**getFollowerStats**](AnalyticsApi.md#getFollowerStats) | **GET** /v1/accounts/follower-stats | Get follower stats |
| [**getFollowerStatsWithHttpInfo**](AnalyticsApi.md#getFollowerStatsWithHttpInfo) | **GET** /v1/accounts/follower-stats | Get follower stats |
| [**getLinkedInAggregateAnalytics**](AnalyticsApi.md#getLinkedInAggregateAnalytics) | **GET** /v1/accounts/{accountId}/linkedin-aggregate-analytics | Get LinkedIn aggregate stats |
| [**getLinkedInAggregateAnalyticsWithHttpInfo**](AnalyticsApi.md#getLinkedInAggregateAnalyticsWithHttpInfo) | **GET** /v1/accounts/{accountId}/linkedin-aggregate-analytics | Get LinkedIn aggregate stats |
| [**getLinkedInPostAnalytics**](AnalyticsApi.md#getLinkedInPostAnalytics) | **GET** /v1/accounts/{accountId}/linkedin-post-analytics | Get LinkedIn post stats |
| [**getLinkedInPostAnalyticsWithHttpInfo**](AnalyticsApi.md#getLinkedInPostAnalyticsWithHttpInfo) | **GET** /v1/accounts/{accountId}/linkedin-post-analytics | Get LinkedIn post stats |
| [**getPostingFrequency**](AnalyticsApi.md#getPostingFrequency) | **GET** /v1/analytics/posting-frequency | Get posting frequency vs engagement |
| [**getPostingFrequencyWithHttpInfo**](AnalyticsApi.md#getPostingFrequencyWithHttpInfo) | **GET** /v1/analytics/posting-frequency | Get posting frequency vs engagement |
| [**getYouTubeDailyViews**](AnalyticsApi.md#getYouTubeDailyViews) | **GET** /v1/analytics/youtube/daily-views | Get YouTube daily views |
| [**getYouTubeDailyViewsWithHttpInfo**](AnalyticsApi.md#getYouTubeDailyViewsWithHttpInfo) | **GET** /v1/analytics/youtube/daily-views | Get YouTube daily views |



## getAnalytics

> GetAnalytics200Response getAnalytics(postId, platform, profileId, source, fromDate, toDate, limit, page, sortBy, order)

Get post analytics

Returns analytics for posts. With postId, returns a single post. Without it, returns a paginated list with overview stats. Accepts both Late Post IDs and External Post IDs (auto-resolved). Data is cached and refreshed at most once per hour. For follower stats, use /v1/accounts/follower-stats. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String postId = "postId_example"; // String | Returns analytics for a single post. Accepts both Late Post IDs and External Post IDs. Late IDs are auto-resolved to External Post analytics.
        String platform = "platform_example"; // String | Filter by platform (default \"all\")
        String profileId = "profileId_example"; // String | Filter by profile ID (default \"all\")
        String source = "all"; // String | Filter by post source: late (posted via Late API), external (synced from platform), all (default)
        LocalDate fromDate = LocalDate.now(); // LocalDate | Inclusive lower bound
        LocalDate toDate = LocalDate.now(); // LocalDate | Inclusive upper bound
        Integer limit = 50; // Integer | Page size (default 50)
        Integer page = 1; // Integer | Page number (default 1)
        String sortBy = "date"; // String | Sort by date or engagement
        String order = "asc"; // String | Sort order
        try {
            GetAnalytics200Response result = apiInstance.getAnalytics(postId, platform, profileId, source, fromDate, toDate, limit, page, sortBy, order);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getAnalytics");
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
| **postId** | **String**| Returns analytics for a single post. Accepts both Late Post IDs and External Post IDs. Late IDs are auto-resolved to External Post analytics. | [optional] |
| **platform** | **String**| Filter by platform (default \&quot;all\&quot;) | [optional] |
| **profileId** | **String**| Filter by profile ID (default \&quot;all\&quot;) | [optional] |
| **source** | **String**| Filter by post source: late (posted via Late API), external (synced from platform), all (default) | [optional] [default to all] [enum: all, late, external] |
| **fromDate** | **LocalDate**| Inclusive lower bound | [optional] |
| **toDate** | **LocalDate**| Inclusive upper bound | [optional] |
| **limit** | **Integer**| Page size (default 50) | [optional] [default to 50] |
| **page** | **Integer**| Page number (default 1) | [optional] [default to 1] |
| **sortBy** | **String**| Sort by date or engagement | [optional] [default to date] [enum: date, engagement] |
| **order** | **String**| Sort order | [optional] [default to desc] [enum: asc, desc] |

### Return type

[**GetAnalytics200Response**](GetAnalytics200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Analytics result |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

## getAnalyticsWithHttpInfo

> ApiResponse<GetAnalytics200Response> getAnalytics getAnalyticsWithHttpInfo(postId, platform, profileId, source, fromDate, toDate, limit, page, sortBy, order)

Get post analytics

Returns analytics for posts. With postId, returns a single post. Without it, returns a paginated list with overview stats. Accepts both Late Post IDs and External Post IDs (auto-resolved). Data is cached and refreshed at most once per hour. For follower stats, use /v1/accounts/follower-stats. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String postId = "postId_example"; // String | Returns analytics for a single post. Accepts both Late Post IDs and External Post IDs. Late IDs are auto-resolved to External Post analytics.
        String platform = "platform_example"; // String | Filter by platform (default \"all\")
        String profileId = "profileId_example"; // String | Filter by profile ID (default \"all\")
        String source = "all"; // String | Filter by post source: late (posted via Late API), external (synced from platform), all (default)
        LocalDate fromDate = LocalDate.now(); // LocalDate | Inclusive lower bound
        LocalDate toDate = LocalDate.now(); // LocalDate | Inclusive upper bound
        Integer limit = 50; // Integer | Page size (default 50)
        Integer page = 1; // Integer | Page number (default 1)
        String sortBy = "date"; // String | Sort by date or engagement
        String order = "asc"; // String | Sort order
        try {
            ApiResponse<GetAnalytics200Response> response = apiInstance.getAnalyticsWithHttpInfo(postId, platform, profileId, source, fromDate, toDate, limit, page, sortBy, order);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getAnalytics");
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
| **postId** | **String**| Returns analytics for a single post. Accepts both Late Post IDs and External Post IDs. Late IDs are auto-resolved to External Post analytics. | [optional] |
| **platform** | **String**| Filter by platform (default \&quot;all\&quot;) | [optional] |
| **profileId** | **String**| Filter by profile ID (default \&quot;all\&quot;) | [optional] |
| **source** | **String**| Filter by post source: late (posted via Late API), external (synced from platform), all (default) | [optional] [default to all] [enum: all, late, external] |
| **fromDate** | **LocalDate**| Inclusive lower bound | [optional] |
| **toDate** | **LocalDate**| Inclusive upper bound | [optional] |
| **limit** | **Integer**| Page size (default 50) | [optional] [default to 50] |
| **page** | **Integer**| Page number (default 1) | [optional] [default to 1] |
| **sortBy** | **String**| Sort by date or engagement | [optional] [default to date] [enum: date, engagement] |
| **order** | **String**| Sort order | [optional] [default to desc] [enum: asc, desc] |

### Return type

ApiResponse<[**GetAnalytics200Response**](GetAnalytics200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Analytics result |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |


## getBestTimeToPost

> GetBestTimeToPost200Response getBestTimeToPost(platform, profileId)

Get best times to post

Returns the best times to post based on historical engagement data. Groups all published posts by day of week and hour (UTC), calculating average engagement per slot. Use this to auto-schedule posts at optimal times. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String platform = "platform_example"; // String | Filter by platform (e.g. \"instagram\", \"tiktok\"). Omit for all platforms.
        String profileId = "profileId_example"; // String | Filter by profile ID. Omit for all profiles.
        try {
            GetBestTimeToPost200Response result = apiInstance.getBestTimeToPost(platform, profileId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getBestTimeToPost");
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
| **platform** | **String**| Filter by platform (e.g. \&quot;instagram\&quot;, \&quot;tiktok\&quot;). Omit for all platforms. | [optional] |
| **profileId** | **String**| Filter by profile ID. Omit for all profiles. | [optional] |

### Return type

[**GetBestTimeToPost200Response**](GetBestTimeToPost200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Best time slots |  -  |
| **401** | Unauthorized |  -  |
| **403** | Analytics add-on required |  -  |

## getBestTimeToPostWithHttpInfo

> ApiResponse<GetBestTimeToPost200Response> getBestTimeToPost getBestTimeToPostWithHttpInfo(platform, profileId)

Get best times to post

Returns the best times to post based on historical engagement data. Groups all published posts by day of week and hour (UTC), calculating average engagement per slot. Use this to auto-schedule posts at optimal times. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String platform = "platform_example"; // String | Filter by platform (e.g. \"instagram\", \"tiktok\"). Omit for all platforms.
        String profileId = "profileId_example"; // String | Filter by profile ID. Omit for all profiles.
        try {
            ApiResponse<GetBestTimeToPost200Response> response = apiInstance.getBestTimeToPostWithHttpInfo(platform, profileId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getBestTimeToPost");
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
| **platform** | **String**| Filter by platform (e.g. \&quot;instagram\&quot;, \&quot;tiktok\&quot;). Omit for all platforms. | [optional] |
| **profileId** | **String**| Filter by profile ID. Omit for all profiles. | [optional] |

### Return type

ApiResponse<[**GetBestTimeToPost200Response**](GetBestTimeToPost200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Best time slots |  -  |
| **401** | Unauthorized |  -  |
| **403** | Analytics add-on required |  -  |


## getContentDecay

> GetContentDecay200Response getContentDecay(platform, profileId)

Get content performance decay

Returns how engagement accumulates over time after a post is published. Each bucket shows what percentage of the post&#39;s total engagement had been reached by that time window. Useful for understanding content lifespan (e.g. \&quot;posts reach 78% of total engagement within 24 hours\&quot;). Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String platform = "platform_example"; // String | Filter by platform (e.g. \"instagram\", \"tiktok\"). Omit for all platforms.
        String profileId = "profileId_example"; // String | Filter by profile ID. Omit for all profiles.
        try {
            GetContentDecay200Response result = apiInstance.getContentDecay(platform, profileId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getContentDecay");
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
| **platform** | **String**| Filter by platform (e.g. \&quot;instagram\&quot;, \&quot;tiktok\&quot;). Omit for all platforms. | [optional] |
| **profileId** | **String**| Filter by profile ID. Omit for all profiles. | [optional] |

### Return type

[**GetContentDecay200Response**](GetContentDecay200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Content decay buckets |  -  |
| **401** | Unauthorized |  -  |
| **403** | Analytics add-on required |  -  |

## getContentDecayWithHttpInfo

> ApiResponse<GetContentDecay200Response> getContentDecay getContentDecayWithHttpInfo(platform, profileId)

Get content performance decay

Returns how engagement accumulates over time after a post is published. Each bucket shows what percentage of the post&#39;s total engagement had been reached by that time window. Useful for understanding content lifespan (e.g. \&quot;posts reach 78% of total engagement within 24 hours\&quot;). Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String platform = "platform_example"; // String | Filter by platform (e.g. \"instagram\", \"tiktok\"). Omit for all platforms.
        String profileId = "profileId_example"; // String | Filter by profile ID. Omit for all profiles.
        try {
            ApiResponse<GetContentDecay200Response> response = apiInstance.getContentDecayWithHttpInfo(platform, profileId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getContentDecay");
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
| **platform** | **String**| Filter by platform (e.g. \&quot;instagram\&quot;, \&quot;tiktok\&quot;). Omit for all platforms. | [optional] |
| **profileId** | **String**| Filter by profile ID. Omit for all profiles. | [optional] |

### Return type

ApiResponse<[**GetContentDecay200Response**](GetContentDecay200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Content decay buckets |  -  |
| **401** | Unauthorized |  -  |
| **403** | Analytics add-on required |  -  |


## getDailyMetrics

> GetDailyMetrics200Response getDailyMetrics(platform, profileId, fromDate, toDate)

Get daily aggregated metrics

Returns daily aggregated analytics metrics and a per-platform breakdown. Each day includes post count, platform distribution, and summed metrics (impressions, reach, likes, comments, shares, saves, clicks, views). Defaults to the last 180 days. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String platform = "platform_example"; // String | Filter by platform (e.g. \"instagram\", \"tiktok\"). Omit for all platforms.
        String profileId = "profileId_example"; // String | Filter by profile ID. Omit for all profiles.
        OffsetDateTime fromDate = OffsetDateTime.now(); // OffsetDateTime | Inclusive start date (ISO 8601). Defaults to 180 days ago.
        OffsetDateTime toDate = OffsetDateTime.now(); // OffsetDateTime | Inclusive end date (ISO 8601). Defaults to now.
        try {
            GetDailyMetrics200Response result = apiInstance.getDailyMetrics(platform, profileId, fromDate, toDate);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getDailyMetrics");
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
| **platform** | **String**| Filter by platform (e.g. \&quot;instagram\&quot;, \&quot;tiktok\&quot;). Omit for all platforms. | [optional] |
| **profileId** | **String**| Filter by profile ID. Omit for all profiles. | [optional] |
| **fromDate** | **OffsetDateTime**| Inclusive start date (ISO 8601). Defaults to 180 days ago. | [optional] |
| **toDate** | **OffsetDateTime**| Inclusive end date (ISO 8601). Defaults to now. | [optional] |

### Return type

[**GetDailyMetrics200Response**](GetDailyMetrics200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Daily metrics and platform breakdown |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |

## getDailyMetricsWithHttpInfo

> ApiResponse<GetDailyMetrics200Response> getDailyMetrics getDailyMetricsWithHttpInfo(platform, profileId, fromDate, toDate)

Get daily aggregated metrics

Returns daily aggregated analytics metrics and a per-platform breakdown. Each day includes post count, platform distribution, and summed metrics (impressions, reach, likes, comments, shares, saves, clicks, views). Defaults to the last 180 days. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String platform = "platform_example"; // String | Filter by platform (e.g. \"instagram\", \"tiktok\"). Omit for all platforms.
        String profileId = "profileId_example"; // String | Filter by profile ID. Omit for all profiles.
        OffsetDateTime fromDate = OffsetDateTime.now(); // OffsetDateTime | Inclusive start date (ISO 8601). Defaults to 180 days ago.
        OffsetDateTime toDate = OffsetDateTime.now(); // OffsetDateTime | Inclusive end date (ISO 8601). Defaults to now.
        try {
            ApiResponse<GetDailyMetrics200Response> response = apiInstance.getDailyMetricsWithHttpInfo(platform, profileId, fromDate, toDate);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getDailyMetrics");
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
| **platform** | **String**| Filter by platform (e.g. \&quot;instagram\&quot;, \&quot;tiktok\&quot;). Omit for all platforms. | [optional] |
| **profileId** | **String**| Filter by profile ID. Omit for all profiles. | [optional] |
| **fromDate** | **OffsetDateTime**| Inclusive start date (ISO 8601). Defaults to 180 days ago. | [optional] |
| **toDate** | **OffsetDateTime**| Inclusive end date (ISO 8601). Defaults to now. | [optional] |

### Return type

ApiResponse<[**GetDailyMetrics200Response**](GetDailyMetrics200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Daily metrics and platform breakdown |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |


## getFollowerStats

> GetFollowerStats200Response getFollowerStats(accountIds, profileId, fromDate, toDate, granularity)

Get follower stats

Returns follower count history and growth metrics for connected social accounts. Requires analytics add-on subscription. Follower counts are refreshed once per day. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String accountIds = "accountIds_example"; // String | Comma-separated list of account IDs (optional, defaults to all user's accounts)
        String profileId = "profileId_example"; // String | Filter by profile ID
        LocalDate fromDate = LocalDate.now(); // LocalDate | Start date in YYYY-MM-DD format (defaults to 30 days ago)
        LocalDate toDate = LocalDate.now(); // LocalDate | End date in YYYY-MM-DD format (defaults to today)
        String granularity = "daily"; // String | Data aggregation level
        try {
            GetFollowerStats200Response result = apiInstance.getFollowerStats(accountIds, profileId, fromDate, toDate, granularity);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getFollowerStats");
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
| **accountIds** | **String**| Comma-separated list of account IDs (optional, defaults to all user&#39;s accounts) | [optional] |
| **profileId** | **String**| Filter by profile ID | [optional] |
| **fromDate** | **LocalDate**| Start date in YYYY-MM-DD format (defaults to 30 days ago) | [optional] |
| **toDate** | **LocalDate**| End date in YYYY-MM-DD format (defaults to today) | [optional] |
| **granularity** | **String**| Data aggregation level | [optional] [default to daily] [enum: daily, weekly, monthly] |

### Return type

[**GetFollowerStats200Response**](GetFollowerStats200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Follower stats |  -  |
| **401** | Unauthorized |  -  |
| **403** | Analytics add-on required |  -  |

## getFollowerStatsWithHttpInfo

> ApiResponse<GetFollowerStats200Response> getFollowerStats getFollowerStatsWithHttpInfo(accountIds, profileId, fromDate, toDate, granularity)

Get follower stats

Returns follower count history and growth metrics for connected social accounts. Requires analytics add-on subscription. Follower counts are refreshed once per day. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String accountIds = "accountIds_example"; // String | Comma-separated list of account IDs (optional, defaults to all user's accounts)
        String profileId = "profileId_example"; // String | Filter by profile ID
        LocalDate fromDate = LocalDate.now(); // LocalDate | Start date in YYYY-MM-DD format (defaults to 30 days ago)
        LocalDate toDate = LocalDate.now(); // LocalDate | End date in YYYY-MM-DD format (defaults to today)
        String granularity = "daily"; // String | Data aggregation level
        try {
            ApiResponse<GetFollowerStats200Response> response = apiInstance.getFollowerStatsWithHttpInfo(accountIds, profileId, fromDate, toDate, granularity);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getFollowerStats");
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
| **accountIds** | **String**| Comma-separated list of account IDs (optional, defaults to all user&#39;s accounts) | [optional] |
| **profileId** | **String**| Filter by profile ID | [optional] |
| **fromDate** | **LocalDate**| Start date in YYYY-MM-DD format (defaults to 30 days ago) | [optional] |
| **toDate** | **LocalDate**| End date in YYYY-MM-DD format (defaults to today) | [optional] |
| **granularity** | **String**| Data aggregation level | [optional] [default to daily] [enum: daily, weekly, monthly] |

### Return type

ApiResponse<[**GetFollowerStats200Response**](GetFollowerStats200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Follower stats |  -  |
| **401** | Unauthorized |  -  |
| **403** | Analytics add-on required |  -  |


## getLinkedInAggregateAnalytics

> GetLinkedInAggregateAnalytics200Response getLinkedInAggregateAnalytics(accountId, aggregation, startDate, endDate, metrics)

Get LinkedIn aggregate stats

Returns aggregate analytics across all posts for a LinkedIn personal account. Org accounts should use /v1/analytics instead. Requires r_member_postAnalytics scope.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String accountId = "accountId_example"; // String | The ID of the LinkedIn personal account
        String aggregation = "TOTAL"; // String | TOTAL (default, lifetime totals) or DAILY (time series). MEMBERS_REACHED not available with DAILY.
        LocalDate startDate = LocalDate.parse("2024-01-01"); // LocalDate | Start date (YYYY-MM-DD). If omitted, returns lifetime analytics.
        LocalDate endDate = LocalDate.parse("2024-01-31"); // LocalDate | End date (YYYY-MM-DD, exclusive). Defaults to today if omitted.
        String metrics = "IMPRESSION,REACTION,COMMENT"; // String | Comma-separated metrics: IMPRESSION, MEMBERS_REACHED, REACTION, COMMENT, RESHARE. Omit for all.
        try {
            GetLinkedInAggregateAnalytics200Response result = apiInstance.getLinkedInAggregateAnalytics(accountId, aggregation, startDate, endDate, metrics);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getLinkedInAggregateAnalytics");
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
| **accountId** | **String**| The ID of the LinkedIn personal account | |
| **aggregation** | **String**| TOTAL (default, lifetime totals) or DAILY (time series). MEMBERS_REACHED not available with DAILY. | [optional] [default to TOTAL] [enum: TOTAL, DAILY] |
| **startDate** | **LocalDate**| Start date (YYYY-MM-DD). If omitted, returns lifetime analytics. | [optional] |
| **endDate** | **LocalDate**| End date (YYYY-MM-DD, exclusive). Defaults to today if omitted. | [optional] |
| **metrics** | **String**| Comma-separated metrics: IMPRESSION, MEMBERS_REACHED, REACTION, COMMENT, RESHARE. Omit for all. | [optional] |

### Return type

[**GetLinkedInAggregateAnalytics200Response**](GetLinkedInAggregateAnalytics200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Aggregate analytics data |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **403** | Missing required LinkedIn scope |  -  |
| **404** | Account not found |  -  |

## getLinkedInAggregateAnalyticsWithHttpInfo

> ApiResponse<GetLinkedInAggregateAnalytics200Response> getLinkedInAggregateAnalytics getLinkedInAggregateAnalyticsWithHttpInfo(accountId, aggregation, startDate, endDate, metrics)

Get LinkedIn aggregate stats

Returns aggregate analytics across all posts for a LinkedIn personal account. Org accounts should use /v1/analytics instead. Requires r_member_postAnalytics scope.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String accountId = "accountId_example"; // String | The ID of the LinkedIn personal account
        String aggregation = "TOTAL"; // String | TOTAL (default, lifetime totals) or DAILY (time series). MEMBERS_REACHED not available with DAILY.
        LocalDate startDate = LocalDate.parse("2024-01-01"); // LocalDate | Start date (YYYY-MM-DD). If omitted, returns lifetime analytics.
        LocalDate endDate = LocalDate.parse("2024-01-31"); // LocalDate | End date (YYYY-MM-DD, exclusive). Defaults to today if omitted.
        String metrics = "IMPRESSION,REACTION,COMMENT"; // String | Comma-separated metrics: IMPRESSION, MEMBERS_REACHED, REACTION, COMMENT, RESHARE. Omit for all.
        try {
            ApiResponse<GetLinkedInAggregateAnalytics200Response> response = apiInstance.getLinkedInAggregateAnalyticsWithHttpInfo(accountId, aggregation, startDate, endDate, metrics);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getLinkedInAggregateAnalytics");
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
| **accountId** | **String**| The ID of the LinkedIn personal account | |
| **aggregation** | **String**| TOTAL (default, lifetime totals) or DAILY (time series). MEMBERS_REACHED not available with DAILY. | [optional] [default to TOTAL] [enum: TOTAL, DAILY] |
| **startDate** | **LocalDate**| Start date (YYYY-MM-DD). If omitted, returns lifetime analytics. | [optional] |
| **endDate** | **LocalDate**| End date (YYYY-MM-DD, exclusive). Defaults to today if omitted. | [optional] |
| **metrics** | **String**| Comma-separated metrics: IMPRESSION, MEMBERS_REACHED, REACTION, COMMENT, RESHARE. Omit for all. | [optional] |

### Return type

ApiResponse<[**GetLinkedInAggregateAnalytics200Response**](GetLinkedInAggregateAnalytics200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Aggregate analytics data |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **403** | Missing required LinkedIn scope |  -  |
| **404** | Account not found |  -  |


## getLinkedInPostAnalytics

> GetLinkedInPostAnalytics200Response getLinkedInPostAnalytics(accountId, urn)

Get LinkedIn post stats

Returns analytics for a specific LinkedIn post by URN. Works for both personal and organization accounts.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String accountId = "accountId_example"; // String | The ID of the LinkedIn account
        String urn = "urn:li:share:7123456789012345678"; // String | The LinkedIn post URN
        try {
            GetLinkedInPostAnalytics200Response result = apiInstance.getLinkedInPostAnalytics(accountId, urn);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getLinkedInPostAnalytics");
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
| **accountId** | **String**| The ID of the LinkedIn account | |
| **urn** | **String**| The LinkedIn post URN | |

### Return type

[**GetLinkedInPostAnalytics200Response**](GetLinkedInPostAnalytics200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Post analytics data |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **403** | Missing required LinkedIn scope |  -  |
| **404** | Account or post not found |  -  |

## getLinkedInPostAnalyticsWithHttpInfo

> ApiResponse<GetLinkedInPostAnalytics200Response> getLinkedInPostAnalytics getLinkedInPostAnalyticsWithHttpInfo(accountId, urn)

Get LinkedIn post stats

Returns analytics for a specific LinkedIn post by URN. Works for both personal and organization accounts.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String accountId = "accountId_example"; // String | The ID of the LinkedIn account
        String urn = "urn:li:share:7123456789012345678"; // String | The LinkedIn post URN
        try {
            ApiResponse<GetLinkedInPostAnalytics200Response> response = apiInstance.getLinkedInPostAnalyticsWithHttpInfo(accountId, urn);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getLinkedInPostAnalytics");
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
| **accountId** | **String**| The ID of the LinkedIn account | |
| **urn** | **String**| The LinkedIn post URN | |

### Return type

ApiResponse<[**GetLinkedInPostAnalytics200Response**](GetLinkedInPostAnalytics200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Post analytics data |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **403** | Missing required LinkedIn scope |  -  |
| **404** | Account or post not found |  -  |


## getPostingFrequency

> GetPostingFrequency200Response getPostingFrequency(platform, profileId)

Get posting frequency vs engagement

Returns the correlation between posting frequency (posts per week) and engagement rate, broken down by platform. Helps find the optimal posting cadence for each platform. Each row represents a specific (platform, posts_per_week) combination with the average engagement rate observed across all weeks matching that frequency. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String platform = "platform_example"; // String | Filter by platform (e.g. \"instagram\", \"tiktok\"). Omit for all platforms.
        String profileId = "profileId_example"; // String | Filter by profile ID. Omit for all profiles.
        try {
            GetPostingFrequency200Response result = apiInstance.getPostingFrequency(platform, profileId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getPostingFrequency");
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
| **platform** | **String**| Filter by platform (e.g. \&quot;instagram\&quot;, \&quot;tiktok\&quot;). Omit for all platforms. | [optional] |
| **profileId** | **String**| Filter by profile ID. Omit for all profiles. | [optional] |

### Return type

[**GetPostingFrequency200Response**](GetPostingFrequency200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Posting frequency data |  -  |
| **401** | Unauthorized |  -  |
| **403** | Analytics add-on required |  -  |

## getPostingFrequencyWithHttpInfo

> ApiResponse<GetPostingFrequency200Response> getPostingFrequency getPostingFrequencyWithHttpInfo(platform, profileId)

Get posting frequency vs engagement

Returns the correlation between posting frequency (posts per week) and engagement rate, broken down by platform. Helps find the optimal posting cadence for each platform. Each row represents a specific (platform, posts_per_week) combination with the average engagement rate observed across all weeks matching that frequency. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String platform = "platform_example"; // String | Filter by platform (e.g. \"instagram\", \"tiktok\"). Omit for all platforms.
        String profileId = "profileId_example"; // String | Filter by profile ID. Omit for all profiles.
        try {
            ApiResponse<GetPostingFrequency200Response> response = apiInstance.getPostingFrequencyWithHttpInfo(platform, profileId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getPostingFrequency");
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
| **platform** | **String**| Filter by platform (e.g. \&quot;instagram\&quot;, \&quot;tiktok\&quot;). Omit for all platforms. | [optional] |
| **profileId** | **String**| Filter by profile ID. Omit for all profiles. | [optional] |

### Return type

ApiResponse<[**GetPostingFrequency200Response**](GetPostingFrequency200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Posting frequency data |  -  |
| **401** | Unauthorized |  -  |
| **403** | Analytics add-on required |  -  |


## getYouTubeDailyViews

> YouTubeDailyViewsResponse getYouTubeDailyViews(videoId, accountId, startDate, endDate)

Get YouTube daily views

Returns daily view counts for a YouTube video including views, watch time, and subscriber changes. Requires yt-analytics.readonly scope (re-authorization may be needed). Data has a 2-3 day delay. Max 90 days, defaults to last 30 days. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String videoId = "videoId_example"; // String | The YouTube video ID (e.g., \"dQw4w9WgXcQ\")
        String accountId = "accountId_example"; // String | The Late account ID for the YouTube account
        LocalDate startDate = LocalDate.now(); // LocalDate | Start date (YYYY-MM-DD). Defaults to 30 days ago.
        LocalDate endDate = LocalDate.now(); // LocalDate | End date (YYYY-MM-DD). Defaults to 3 days ago (YouTube data latency).
        try {
            YouTubeDailyViewsResponse result = apiInstance.getYouTubeDailyViews(videoId, accountId, startDate, endDate);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getYouTubeDailyViews");
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
| **videoId** | **String**| The YouTube video ID (e.g., \&quot;dQw4w9WgXcQ\&quot;) | |
| **accountId** | **String**| The Late account ID for the YouTube account | |
| **startDate** | **LocalDate**| Start date (YYYY-MM-DD). Defaults to 30 days ago. | [optional] |
| **endDate** | **LocalDate**| End date (YYYY-MM-DD). Defaults to 3 days ago (YouTube data latency). | [optional] |

### Return type

[**YouTubeDailyViewsResponse**](YouTubeDailyViewsResponse.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Daily views breakdown |  -  |
| **400** | Bad request (missing or invalid parameters) |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **403** | Access denied to this account |  -  |
| **412** | Missing YouTube Analytics scope |  -  |
| **500** | Internal server error |  -  |

## getYouTubeDailyViewsWithHttpInfo

> ApiResponse<YouTubeDailyViewsResponse> getYouTubeDailyViews getYouTubeDailyViewsWithHttpInfo(videoId, accountId, startDate, endDate)

Get YouTube daily views

Returns daily view counts for a YouTube video including views, watch time, and subscriber changes. Requires yt-analytics.readonly scope (re-authorization may be needed). Data has a 2-3 day delay. Max 90 days, defaults to last 30 days. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String videoId = "videoId_example"; // String | The YouTube video ID (e.g., \"dQw4w9WgXcQ\")
        String accountId = "accountId_example"; // String | The Late account ID for the YouTube account
        LocalDate startDate = LocalDate.now(); // LocalDate | Start date (YYYY-MM-DD). Defaults to 30 days ago.
        LocalDate endDate = LocalDate.now(); // LocalDate | End date (YYYY-MM-DD). Defaults to 3 days ago (YouTube data latency).
        try {
            ApiResponse<YouTubeDailyViewsResponse> response = apiInstance.getYouTubeDailyViewsWithHttpInfo(videoId, accountId, startDate, endDate);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getYouTubeDailyViews");
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
| **videoId** | **String**| The YouTube video ID (e.g., \&quot;dQw4w9WgXcQ\&quot;) | |
| **accountId** | **String**| The Late account ID for the YouTube account | |
| **startDate** | **LocalDate**| Start date (YYYY-MM-DD). Defaults to 30 days ago. | [optional] |
| **endDate** | **LocalDate**| End date (YYYY-MM-DD). Defaults to 3 days ago (YouTube data latency). | [optional] |

### Return type

ApiResponse<[**YouTubeDailyViewsResponse**](YouTubeDailyViewsResponse.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Daily views breakdown |  -  |
| **400** | Bad request (missing or invalid parameters) |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **403** | Access denied to this account |  -  |
| **412** | Missing YouTube Analytics scope |  -  |
| **500** | Internal server error |  -  |

