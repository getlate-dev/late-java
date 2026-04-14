# AnalyticsApi

All URIs are relative to *https://zernio.com/api*

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
| [**getGoogleBusinessPerformance**](AnalyticsApi.md#getGoogleBusinessPerformance) | **GET** /v1/analytics/googlebusiness/performance | Get GBP performance metrics |
| [**getGoogleBusinessPerformanceWithHttpInfo**](AnalyticsApi.md#getGoogleBusinessPerformanceWithHttpInfo) | **GET** /v1/analytics/googlebusiness/performance | Get GBP performance metrics |
| [**getGoogleBusinessSearchKeywords**](AnalyticsApi.md#getGoogleBusinessSearchKeywords) | **GET** /v1/analytics/googlebusiness/search-keywords | Get GBP search keywords |
| [**getGoogleBusinessSearchKeywordsWithHttpInfo**](AnalyticsApi.md#getGoogleBusinessSearchKeywordsWithHttpInfo) | **GET** /v1/analytics/googlebusiness/search-keywords | Get GBP search keywords |
| [**getInstagramAccountInsights**](AnalyticsApi.md#getInstagramAccountInsights) | **GET** /v1/analytics/instagram/account-insights | Get Instagram insights |
| [**getInstagramAccountInsightsWithHttpInfo**](AnalyticsApi.md#getInstagramAccountInsightsWithHttpInfo) | **GET** /v1/analytics/instagram/account-insights | Get Instagram insights |
| [**getInstagramDemographics**](AnalyticsApi.md#getInstagramDemographics) | **GET** /v1/analytics/instagram/demographics | Get Instagram demographics |
| [**getInstagramDemographicsWithHttpInfo**](AnalyticsApi.md#getInstagramDemographicsWithHttpInfo) | **GET** /v1/analytics/instagram/demographics | Get Instagram demographics |
| [**getLinkedInAggregateAnalytics**](AnalyticsApi.md#getLinkedInAggregateAnalytics) | **GET** /v1/accounts/{accountId}/linkedin-aggregate-analytics | Get LinkedIn aggregate stats |
| [**getLinkedInAggregateAnalyticsWithHttpInfo**](AnalyticsApi.md#getLinkedInAggregateAnalyticsWithHttpInfo) | **GET** /v1/accounts/{accountId}/linkedin-aggregate-analytics | Get LinkedIn aggregate stats |
| [**getLinkedInPostAnalytics**](AnalyticsApi.md#getLinkedInPostAnalytics) | **GET** /v1/accounts/{accountId}/linkedin-post-analytics | Get LinkedIn post stats |
| [**getLinkedInPostAnalyticsWithHttpInfo**](AnalyticsApi.md#getLinkedInPostAnalyticsWithHttpInfo) | **GET** /v1/accounts/{accountId}/linkedin-post-analytics | Get LinkedIn post stats |
| [**getLinkedInPostReactions**](AnalyticsApi.md#getLinkedInPostReactions) | **GET** /v1/accounts/{accountId}/linkedin-post-reactions | Get LinkedIn post reactions |
| [**getLinkedInPostReactionsWithHttpInfo**](AnalyticsApi.md#getLinkedInPostReactionsWithHttpInfo) | **GET** /v1/accounts/{accountId}/linkedin-post-reactions | Get LinkedIn post reactions |
| [**getPostTimeline**](AnalyticsApi.md#getPostTimeline) | **GET** /v1/analytics/post-timeline | Get post analytics timeline |
| [**getPostTimelineWithHttpInfo**](AnalyticsApi.md#getPostTimelineWithHttpInfo) | **GET** /v1/analytics/post-timeline | Get post analytics timeline |
| [**getPostingFrequency**](AnalyticsApi.md#getPostingFrequency) | **GET** /v1/analytics/posting-frequency | Get frequency vs engagement |
| [**getPostingFrequencyWithHttpInfo**](AnalyticsApi.md#getPostingFrequencyWithHttpInfo) | **GET** /v1/analytics/posting-frequency | Get frequency vs engagement |
| [**getYouTubeDailyViews**](AnalyticsApi.md#getYouTubeDailyViews) | **GET** /v1/analytics/youtube/daily-views | Get YouTube daily views |
| [**getYouTubeDailyViewsWithHttpInfo**](AnalyticsApi.md#getYouTubeDailyViewsWithHttpInfo) | **GET** /v1/analytics/youtube/daily-views | Get YouTube daily views |
| [**getYouTubeDemographics**](AnalyticsApi.md#getYouTubeDemographics) | **GET** /v1/analytics/youtube/demographics | Get YouTube demographics |
| [**getYouTubeDemographicsWithHttpInfo**](AnalyticsApi.md#getYouTubeDemographicsWithHttpInfo) | **GET** /v1/analytics/youtube/demographics | Get YouTube demographics |



## getAnalytics

> GetAnalytics200Response getAnalytics(postId, platform, profileId, accountId, source, fromDate, toDate, limit, page, sortBy, order)

Get post analytics

Returns analytics for posts. With postId, returns a single post. Without it, returns a paginated list with overview stats. Accepts both Zernio Post IDs and External Post IDs (auto-resolved). fromDate defaults to 90 days ago if omitted, max range 366 days. Single post lookups may return 202 (sync pending) or 424 (all platforms failed). For follower stats, use /v1/accounts/follower-stats.  LinkedIn personal accounts: Analytics are only available for posts published through Zernio. LinkedIn&#39;s API only returns metrics for posts authored by the authenticated user. Organization/company page analytics work for all posts. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String postId = "postId_example"; // String | Returns analytics for a single post. Accepts both Zernio Post IDs and External Post IDs. Zernio IDs are auto-resolved to External Post analytics.
        String platform = "platform_example"; // String | Filter by platform (default \"all\")
        String profileId = "profileId_example"; // String | Filter by profile ID (default \"all\")
        String accountId = "accountId_example"; // String | Filter by social account ID
        String source = "all"; // String | Filter by post source: late (posted via Zernio API), external (synced from platform), all (default)
        LocalDate fromDate = LocalDate.now(); // LocalDate | Inclusive lower bound (YYYY-MM-DD). Defaults to 90 days ago if omitted. Max range is 366 days.
        LocalDate toDate = LocalDate.now(); // LocalDate | Inclusive upper bound (YYYY-MM-DD). Defaults to today if omitted.
        Integer limit = 50; // Integer | Page size (default 50)
        Integer page = 1; // Integer | Page number (default 1)
        String sortBy = "date"; // String | Sort by date, engagement, or a specific metric
        String order = "asc"; // String | Sort order
        try {
            GetAnalytics200Response result = apiInstance.getAnalytics(postId, platform, profileId, accountId, source, fromDate, toDate, limit, page, sortBy, order);
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
| **postId** | **String**| Returns analytics for a single post. Accepts both Zernio Post IDs and External Post IDs. Zernio IDs are auto-resolved to External Post analytics. | [optional] |
| **platform** | **String**| Filter by platform (default \&quot;all\&quot;) | [optional] |
| **profileId** | **String**| Filter by profile ID (default \&quot;all\&quot;) | [optional] |
| **accountId** | **String**| Filter by social account ID | [optional] |
| **source** | **String**| Filter by post source: late (posted via Zernio API), external (synced from platform), all (default) | [optional] [default to all] [enum: all, late, external] |
| **fromDate** | **LocalDate**| Inclusive lower bound (YYYY-MM-DD). Defaults to 90 days ago if omitted. Max range is 366 days. | [optional] |
| **toDate** | **LocalDate**| Inclusive upper bound (YYYY-MM-DD). Defaults to today if omitted. | [optional] |
| **limit** | **Integer**| Page size (default 50) | [optional] [default to 50] |
| **page** | **Integer**| Page number (default 1) | [optional] [default to 1] |
| **sortBy** | **String**| Sort by date, engagement, or a specific metric | [optional] [default to date] [enum: date, engagement, impressions, reach, likes, comments, shares, saves, clicks, views] |
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
| **202** | Analytics are being synced from the platform (single post lookup only). The response body matches AnalyticsSinglePostResponse with syncStatus \&quot;pending\&quot; and a message. |  -  |
| **400** | Validation error |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **404** | Resource not found |  -  |
| **424** | Post failed to publish on all platforms. Analytics are unavailable. (single post lookup only) |  -  |
| **500** | Internal server error |  -  |

## getAnalyticsWithHttpInfo

> ApiResponse<GetAnalytics200Response> getAnalytics getAnalyticsWithHttpInfo(postId, platform, profileId, accountId, source, fromDate, toDate, limit, page, sortBy, order)

Get post analytics

Returns analytics for posts. With postId, returns a single post. Without it, returns a paginated list with overview stats. Accepts both Zernio Post IDs and External Post IDs (auto-resolved). fromDate defaults to 90 days ago if omitted, max range 366 days. Single post lookups may return 202 (sync pending) or 424 (all platforms failed). For follower stats, use /v1/accounts/follower-stats.  LinkedIn personal accounts: Analytics are only available for posts published through Zernio. LinkedIn&#39;s API only returns metrics for posts authored by the authenticated user. Organization/company page analytics work for all posts. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String postId = "postId_example"; // String | Returns analytics for a single post. Accepts both Zernio Post IDs and External Post IDs. Zernio IDs are auto-resolved to External Post analytics.
        String platform = "platform_example"; // String | Filter by platform (default \"all\")
        String profileId = "profileId_example"; // String | Filter by profile ID (default \"all\")
        String accountId = "accountId_example"; // String | Filter by social account ID
        String source = "all"; // String | Filter by post source: late (posted via Zernio API), external (synced from platform), all (default)
        LocalDate fromDate = LocalDate.now(); // LocalDate | Inclusive lower bound (YYYY-MM-DD). Defaults to 90 days ago if omitted. Max range is 366 days.
        LocalDate toDate = LocalDate.now(); // LocalDate | Inclusive upper bound (YYYY-MM-DD). Defaults to today if omitted.
        Integer limit = 50; // Integer | Page size (default 50)
        Integer page = 1; // Integer | Page number (default 1)
        String sortBy = "date"; // String | Sort by date, engagement, or a specific metric
        String order = "asc"; // String | Sort order
        try {
            ApiResponse<GetAnalytics200Response> response = apiInstance.getAnalyticsWithHttpInfo(postId, platform, profileId, accountId, source, fromDate, toDate, limit, page, sortBy, order);
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
| **postId** | **String**| Returns analytics for a single post. Accepts both Zernio Post IDs and External Post IDs. Zernio IDs are auto-resolved to External Post analytics. | [optional] |
| **platform** | **String**| Filter by platform (default \&quot;all\&quot;) | [optional] |
| **profileId** | **String**| Filter by profile ID (default \&quot;all\&quot;) | [optional] |
| **accountId** | **String**| Filter by social account ID | [optional] |
| **source** | **String**| Filter by post source: late (posted via Zernio API), external (synced from platform), all (default) | [optional] [default to all] [enum: all, late, external] |
| **fromDate** | **LocalDate**| Inclusive lower bound (YYYY-MM-DD). Defaults to 90 days ago if omitted. Max range is 366 days. | [optional] |
| **toDate** | **LocalDate**| Inclusive upper bound (YYYY-MM-DD). Defaults to today if omitted. | [optional] |
| **limit** | **Integer**| Page size (default 50) | [optional] [default to 50] |
| **page** | **Integer**| Page number (default 1) | [optional] [default to 1] |
| **sortBy** | **String**| Sort by date, engagement, or a specific metric | [optional] [default to date] [enum: date, engagement, impressions, reach, likes, comments, shares, saves, clicks, views] |
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
| **202** | Analytics are being synced from the platform (single post lookup only). The response body matches AnalyticsSinglePostResponse with syncStatus \&quot;pending\&quot; and a message. |  -  |
| **400** | Validation error |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **404** | Resource not found |  -  |
| **424** | Post failed to publish on all platforms. Analytics are unavailable. (single post lookup only) |  -  |
| **500** | Internal server error |  -  |


## getBestTimeToPost

> GetBestTimeToPost200Response getBestTimeToPost(platform, profileId, source)

Get best times to post

Returns the best times to post based on historical engagement data. Groups all published posts by day of week and hour (UTC), calculating average engagement per slot. Use this to auto-schedule posts at optimal times. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String platform = "platform_example"; // String | Filter by platform (e.g. \"instagram\", \"tiktok\"). Omit for all platforms.
        String profileId = "profileId_example"; // String | Filter by profile ID. Omit for all profiles.
        String source = "all"; // String | Filter by post origin. \"late\" for posts published via Zernio, \"external\" for posts imported from platforms.
        try {
            GetBestTimeToPost200Response result = apiInstance.getBestTimeToPost(platform, profileId, source);
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
| **source** | **String**| Filter by post origin. \&quot;late\&quot; for posts published via Zernio, \&quot;external\&quot; for posts imported from platforms. | [optional] [default to all] [enum: all, late, external] |

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

> ApiResponse<GetBestTimeToPost200Response> getBestTimeToPost getBestTimeToPostWithHttpInfo(platform, profileId, source)

Get best times to post

Returns the best times to post based on historical engagement data. Groups all published posts by day of week and hour (UTC), calculating average engagement per slot. Use this to auto-schedule posts at optimal times. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String platform = "platform_example"; // String | Filter by platform (e.g. \"instagram\", \"tiktok\"). Omit for all platforms.
        String profileId = "profileId_example"; // String | Filter by profile ID. Omit for all profiles.
        String source = "all"; // String | Filter by post origin. \"late\" for posts published via Zernio, \"external\" for posts imported from platforms.
        try {
            ApiResponse<GetBestTimeToPost200Response> response = apiInstance.getBestTimeToPostWithHttpInfo(platform, profileId, source);
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
| **source** | **String**| Filter by post origin. \&quot;late\&quot; for posts published via Zernio, \&quot;external\&quot; for posts imported from platforms. | [optional] [default to all] [enum: all, late, external] |

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

> GetContentDecay200Response getContentDecay(platform, profileId, source)

Get content performance decay

Returns how engagement accumulates over time after a post is published. Each bucket shows what percentage of the post&#39;s total engagement had been reached by that time window. Useful for understanding content lifespan (e.g. \&quot;posts reach 78% of total engagement within 24 hours\&quot;). Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String platform = "platform_example"; // String | Filter by platform (e.g. \"instagram\", \"tiktok\"). Omit for all platforms.
        String profileId = "profileId_example"; // String | Filter by profile ID. Omit for all profiles.
        String source = "all"; // String | Filter by post origin. \"late\" for posts published via Zernio, \"external\" for posts imported from platforms.
        try {
            GetContentDecay200Response result = apiInstance.getContentDecay(platform, profileId, source);
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
| **source** | **String**| Filter by post origin. \&quot;late\&quot; for posts published via Zernio, \&quot;external\&quot; for posts imported from platforms. | [optional] [default to all] [enum: all, late, external] |

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

> ApiResponse<GetContentDecay200Response> getContentDecay getContentDecayWithHttpInfo(platform, profileId, source)

Get content performance decay

Returns how engagement accumulates over time after a post is published. Each bucket shows what percentage of the post&#39;s total engagement had been reached by that time window. Useful for understanding content lifespan (e.g. \&quot;posts reach 78% of total engagement within 24 hours\&quot;). Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String platform = "platform_example"; // String | Filter by platform (e.g. \"instagram\", \"tiktok\"). Omit for all platforms.
        String profileId = "profileId_example"; // String | Filter by profile ID. Omit for all profiles.
        String source = "all"; // String | Filter by post origin. \"late\" for posts published via Zernio, \"external\" for posts imported from platforms.
        try {
            ApiResponse<GetContentDecay200Response> response = apiInstance.getContentDecayWithHttpInfo(platform, profileId, source);
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
| **source** | **String**| Filter by post origin. \&quot;late\&quot; for posts published via Zernio, \&quot;external\&quot; for posts imported from platforms. | [optional] [default to all] [enum: all, late, external] |

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

> GetDailyMetrics200Response getDailyMetrics(platform, profileId, accountId, fromDate, toDate, source)

Get daily aggregated metrics

Returns daily aggregated analytics metrics and a per-platform breakdown. Each day includes post count, platform distribution, and summed metrics (impressions, reach, likes, comments, shares, saves, clicks, views). Defaults to the last 180 days. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String platform = "platform_example"; // String | Filter by platform (e.g. \"instagram\", \"tiktok\"). Omit for all platforms.
        String profileId = "profileId_example"; // String | Filter by profile ID. Omit for all profiles.
        String accountId = "accountId_example"; // String | Filter by social account ID
        OffsetDateTime fromDate = OffsetDateTime.now(); // OffsetDateTime | Inclusive start date (ISO 8601). Defaults to 180 days ago.
        OffsetDateTime toDate = OffsetDateTime.now(); // OffsetDateTime | Inclusive end date (ISO 8601). Defaults to now.
        String source = "all"; // String | Filter by post origin. \"late\" for posts published via Zernio, \"external\" for posts imported from platforms.
        try {
            GetDailyMetrics200Response result = apiInstance.getDailyMetrics(platform, profileId, accountId, fromDate, toDate, source);
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
| **accountId** | **String**| Filter by social account ID | [optional] |
| **fromDate** | **OffsetDateTime**| Inclusive start date (ISO 8601). Defaults to 180 days ago. | [optional] |
| **toDate** | **OffsetDateTime**| Inclusive end date (ISO 8601). Defaults to now. | [optional] |
| **source** | **String**| Filter by post origin. \&quot;late\&quot; for posts published via Zernio, \&quot;external\&quot; for posts imported from platforms. | [optional] [default to all] [enum: all, late, external] |

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

> ApiResponse<GetDailyMetrics200Response> getDailyMetrics getDailyMetricsWithHttpInfo(platform, profileId, accountId, fromDate, toDate, source)

Get daily aggregated metrics

Returns daily aggregated analytics metrics and a per-platform breakdown. Each day includes post count, platform distribution, and summed metrics (impressions, reach, likes, comments, shares, saves, clicks, views). Defaults to the last 180 days. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String platform = "platform_example"; // String | Filter by platform (e.g. \"instagram\", \"tiktok\"). Omit for all platforms.
        String profileId = "profileId_example"; // String | Filter by profile ID. Omit for all profiles.
        String accountId = "accountId_example"; // String | Filter by social account ID
        OffsetDateTime fromDate = OffsetDateTime.now(); // OffsetDateTime | Inclusive start date (ISO 8601). Defaults to 180 days ago.
        OffsetDateTime toDate = OffsetDateTime.now(); // OffsetDateTime | Inclusive end date (ISO 8601). Defaults to now.
        String source = "all"; // String | Filter by post origin. \"late\" for posts published via Zernio, \"external\" for posts imported from platforms.
        try {
            ApiResponse<GetDailyMetrics200Response> response = apiInstance.getDailyMetricsWithHttpInfo(platform, profileId, accountId, fromDate, toDate, source);
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
| **accountId** | **String**| Filter by social account ID | [optional] |
| **fromDate** | **OffsetDateTime**| Inclusive start date (ISO 8601). Defaults to 180 days ago. | [optional] |
| **toDate** | **OffsetDateTime**| Inclusive end date (ISO 8601). Defaults to now. | [optional] |
| **source** | **String**| Filter by post origin. \&quot;late\&quot; for posts published via Zernio, \&quot;external\&quot; for posts imported from platforms. | [optional] [default to all] [enum: all, late, external] |

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
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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


## getGoogleBusinessPerformance

> GetGoogleBusinessPerformance200Response getGoogleBusinessPerformance(accountId, metrics, startDate, endDate)

Get GBP performance metrics

Returns daily performance metrics for a Google Business Profile location. Metrics include impressions (Maps/Search, desktop/mobile), website clicks, call clicks, direction requests, conversations, bookings, and food orders. Data may be delayed 2-3 days. Max 18 months of historical data. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String accountId = "accountId_example"; // String | The Zernio SocialAccount ID for the Google Business Profile account.
        String metrics = "metrics_example"; // String | Comma-separated metric names. Defaults to all available metrics. Valid values: BUSINESS_IMPRESSIONS_DESKTOP_MAPS, BUSINESS_IMPRESSIONS_DESKTOP_SEARCH, BUSINESS_IMPRESSIONS_MOBILE_MAPS, BUSINESS_IMPRESSIONS_MOBILE_SEARCH, BUSINESS_CONVERSATIONS, BUSINESS_DIRECTION_REQUESTS, CALL_CLICKS, WEBSITE_CLICKS, BUSINESS_BOOKINGS, BUSINESS_FOOD_ORDERS, BUSINESS_FOOD_MENU_CLICKS 
        LocalDate startDate = LocalDate.now(); // LocalDate | Start date (YYYY-MM-DD). Defaults to 30 days ago. Max 18 months back.
        LocalDate endDate = LocalDate.now(); // LocalDate | End date (YYYY-MM-DD). Defaults to today.
        try {
            GetGoogleBusinessPerformance200Response result = apiInstance.getGoogleBusinessPerformance(accountId, metrics, startDate, endDate);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getGoogleBusinessPerformance");
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
| **accountId** | **String**| The Zernio SocialAccount ID for the Google Business Profile account. | |
| **metrics** | **String**| Comma-separated metric names. Defaults to all available metrics. Valid values: BUSINESS_IMPRESSIONS_DESKTOP_MAPS, BUSINESS_IMPRESSIONS_DESKTOP_SEARCH, BUSINESS_IMPRESSIONS_MOBILE_MAPS, BUSINESS_IMPRESSIONS_MOBILE_SEARCH, BUSINESS_CONVERSATIONS, BUSINESS_DIRECTION_REQUESTS, CALL_CLICKS, WEBSITE_CLICKS, BUSINESS_BOOKINGS, BUSINESS_FOOD_ORDERS, BUSINESS_FOOD_MENU_CLICKS  | [optional] |
| **startDate** | **LocalDate**| Start date (YYYY-MM-DD). Defaults to 30 days ago. Max 18 months back. | [optional] |
| **endDate** | **LocalDate**| End date (YYYY-MM-DD). Defaults to today. | [optional] |

### Return type

[**GetGoogleBusinessPerformance200Response**](GetGoogleBusinessPerformance200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Performance metrics with daily time series |  -  |
| **400** | Invalid parameters |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **403** | Access denied |  -  |

## getGoogleBusinessPerformanceWithHttpInfo

> ApiResponse<GetGoogleBusinessPerformance200Response> getGoogleBusinessPerformance getGoogleBusinessPerformanceWithHttpInfo(accountId, metrics, startDate, endDate)

Get GBP performance metrics

Returns daily performance metrics for a Google Business Profile location. Metrics include impressions (Maps/Search, desktop/mobile), website clicks, call clicks, direction requests, conversations, bookings, and food orders. Data may be delayed 2-3 days. Max 18 months of historical data. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String accountId = "accountId_example"; // String | The Zernio SocialAccount ID for the Google Business Profile account.
        String metrics = "metrics_example"; // String | Comma-separated metric names. Defaults to all available metrics. Valid values: BUSINESS_IMPRESSIONS_DESKTOP_MAPS, BUSINESS_IMPRESSIONS_DESKTOP_SEARCH, BUSINESS_IMPRESSIONS_MOBILE_MAPS, BUSINESS_IMPRESSIONS_MOBILE_SEARCH, BUSINESS_CONVERSATIONS, BUSINESS_DIRECTION_REQUESTS, CALL_CLICKS, WEBSITE_CLICKS, BUSINESS_BOOKINGS, BUSINESS_FOOD_ORDERS, BUSINESS_FOOD_MENU_CLICKS 
        LocalDate startDate = LocalDate.now(); // LocalDate | Start date (YYYY-MM-DD). Defaults to 30 days ago. Max 18 months back.
        LocalDate endDate = LocalDate.now(); // LocalDate | End date (YYYY-MM-DD). Defaults to today.
        try {
            ApiResponse<GetGoogleBusinessPerformance200Response> response = apiInstance.getGoogleBusinessPerformanceWithHttpInfo(accountId, metrics, startDate, endDate);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getGoogleBusinessPerformance");
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
| **accountId** | **String**| The Zernio SocialAccount ID for the Google Business Profile account. | |
| **metrics** | **String**| Comma-separated metric names. Defaults to all available metrics. Valid values: BUSINESS_IMPRESSIONS_DESKTOP_MAPS, BUSINESS_IMPRESSIONS_DESKTOP_SEARCH, BUSINESS_IMPRESSIONS_MOBILE_MAPS, BUSINESS_IMPRESSIONS_MOBILE_SEARCH, BUSINESS_CONVERSATIONS, BUSINESS_DIRECTION_REQUESTS, CALL_CLICKS, WEBSITE_CLICKS, BUSINESS_BOOKINGS, BUSINESS_FOOD_ORDERS, BUSINESS_FOOD_MENU_CLICKS  | [optional] |
| **startDate** | **LocalDate**| Start date (YYYY-MM-DD). Defaults to 30 days ago. Max 18 months back. | [optional] |
| **endDate** | **LocalDate**| End date (YYYY-MM-DD). Defaults to today. | [optional] |

### Return type

ApiResponse<[**GetGoogleBusinessPerformance200Response**](GetGoogleBusinessPerformance200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Performance metrics with daily time series |  -  |
| **400** | Invalid parameters |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **403** | Access denied |  -  |


## getGoogleBusinessSearchKeywords

> GetGoogleBusinessSearchKeywords200Response getGoogleBusinessSearchKeywords(accountId, startMonth, endMonth)

Get GBP search keywords

Returns search keywords that triggered impressions for a Google Business Profile location. Data is aggregated monthly. Keywords below a minimum impression threshold set by Google are excluded. Max 18 months of historical data. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String accountId = "accountId_example"; // String | The Zernio SocialAccount ID for the Google Business Profile account.
        String startMonth = "startMonth_example"; // String | Start month (YYYY-MM). Defaults to 3 months ago.
        String endMonth = "endMonth_example"; // String | End month (YYYY-MM). Defaults to current month.
        try {
            GetGoogleBusinessSearchKeywords200Response result = apiInstance.getGoogleBusinessSearchKeywords(accountId, startMonth, endMonth);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getGoogleBusinessSearchKeywords");
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
| **accountId** | **String**| The Zernio SocialAccount ID for the Google Business Profile account. | |
| **startMonth** | **String**| Start month (YYYY-MM). Defaults to 3 months ago. | [optional] |
| **endMonth** | **String**| End month (YYYY-MM). Defaults to current month. | [optional] |

### Return type

[**GetGoogleBusinessSearchKeywords200Response**](GetGoogleBusinessSearchKeywords200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Search keywords with impression counts |  -  |
| **400** | Invalid parameters |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **403** | Access denied |  -  |

## getGoogleBusinessSearchKeywordsWithHttpInfo

> ApiResponse<GetGoogleBusinessSearchKeywords200Response> getGoogleBusinessSearchKeywords getGoogleBusinessSearchKeywordsWithHttpInfo(accountId, startMonth, endMonth)

Get GBP search keywords

Returns search keywords that triggered impressions for a Google Business Profile location. Data is aggregated monthly. Keywords below a minimum impression threshold set by Google are excluded. Max 18 months of historical data. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String accountId = "accountId_example"; // String | The Zernio SocialAccount ID for the Google Business Profile account.
        String startMonth = "startMonth_example"; // String | Start month (YYYY-MM). Defaults to 3 months ago.
        String endMonth = "endMonth_example"; // String | End month (YYYY-MM). Defaults to current month.
        try {
            ApiResponse<GetGoogleBusinessSearchKeywords200Response> response = apiInstance.getGoogleBusinessSearchKeywordsWithHttpInfo(accountId, startMonth, endMonth);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getGoogleBusinessSearchKeywords");
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
| **accountId** | **String**| The Zernio SocialAccount ID for the Google Business Profile account. | |
| **startMonth** | **String**| Start month (YYYY-MM). Defaults to 3 months ago. | [optional] |
| **endMonth** | **String**| End month (YYYY-MM). Defaults to current month. | [optional] |

### Return type

ApiResponse<[**GetGoogleBusinessSearchKeywords200Response**](GetGoogleBusinessSearchKeywords200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Search keywords with impression counts |  -  |
| **400** | Invalid parameters |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **403** | Access denied |  -  |


## getInstagramAccountInsights

> InstagramAccountInsightsResponse getInstagramAccountInsights(accountId, metrics, since, until, metricType, breakdown)

Get Instagram insights

Returns account-level Instagram insights such as reach, views, accounts engaged, and total interactions. These metrics reflect the entire account&#39;s performance across all content surfaces (feed, stories, explore, profile), and are fundamentally different from post-level metrics. Data may be delayed up to 48 hours. Max 90 days, defaults to last 30 days. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String accountId = "accountId_example"; // String | The Zernio SocialAccount ID for the Instagram account
        String metrics = "metrics_example"; // String | Comma-separated list of metrics. Defaults to \"reach,views,accounts_engaged,total_interactions\". Valid metrics: reach, views, accounts_engaged, total_interactions, comments, likes, saves, shares, replies, reposts, follows_and_unfollows, profile_links_taps. Note: only \"reach\" supports metricType=time_series. All other metrics are total_value only. 
        LocalDate since = LocalDate.now(); // LocalDate | Start date (YYYY-MM-DD). Defaults to 30 days ago.
        LocalDate until = LocalDate.now(); // LocalDate | End date (YYYY-MM-DD). Defaults to today.
        String metricType = "time_series"; // String | \"total_value\" (default) returns aggregated totals and supports breakdowns. \"time_series\" returns daily values but only works with the \"reach\" metric. 
        String breakdown = "breakdown_example"; // String | Breakdown dimension (only valid with metricType=total_value). Valid values depend on the metric: media_product_type, follow_type, follower_type, contact_button_type. 
        try {
            InstagramAccountInsightsResponse result = apiInstance.getInstagramAccountInsights(accountId, metrics, since, until, metricType, breakdown);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getInstagramAccountInsights");
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
| **accountId** | **String**| The Zernio SocialAccount ID for the Instagram account | |
| **metrics** | **String**| Comma-separated list of metrics. Defaults to \&quot;reach,views,accounts_engaged,total_interactions\&quot;. Valid metrics: reach, views, accounts_engaged, total_interactions, comments, likes, saves, shares, replies, reposts, follows_and_unfollows, profile_links_taps. Note: only \&quot;reach\&quot; supports metricType&#x3D;time_series. All other metrics are total_value only.  | [optional] |
| **since** | **LocalDate**| Start date (YYYY-MM-DD). Defaults to 30 days ago. | [optional] |
| **until** | **LocalDate**| End date (YYYY-MM-DD). Defaults to today. | [optional] |
| **metricType** | **String**| \&quot;total_value\&quot; (default) returns aggregated totals and supports breakdowns. \&quot;time_series\&quot; returns daily values but only works with the \&quot;reach\&quot; metric.  | [optional] [default to total_value] [enum: time_series, total_value] |
| **breakdown** | **String**| Breakdown dimension (only valid with metricType&#x3D;total_value). Valid values depend on the metric: media_product_type, follow_type, follower_type, contact_button_type.  | [optional] |

### Return type

[**InstagramAccountInsightsResponse**](InstagramAccountInsightsResponse.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Account insights data |  -  |
| **400** | Bad request (invalid parameters) |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **403** | Access denied to this account |  -  |
| **404** | Account not found |  -  |

## getInstagramAccountInsightsWithHttpInfo

> ApiResponse<InstagramAccountInsightsResponse> getInstagramAccountInsights getInstagramAccountInsightsWithHttpInfo(accountId, metrics, since, until, metricType, breakdown)

Get Instagram insights

Returns account-level Instagram insights such as reach, views, accounts engaged, and total interactions. These metrics reflect the entire account&#39;s performance across all content surfaces (feed, stories, explore, profile), and are fundamentally different from post-level metrics. Data may be delayed up to 48 hours. Max 90 days, defaults to last 30 days. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String accountId = "accountId_example"; // String | The Zernio SocialAccount ID for the Instagram account
        String metrics = "metrics_example"; // String | Comma-separated list of metrics. Defaults to \"reach,views,accounts_engaged,total_interactions\". Valid metrics: reach, views, accounts_engaged, total_interactions, comments, likes, saves, shares, replies, reposts, follows_and_unfollows, profile_links_taps. Note: only \"reach\" supports metricType=time_series. All other metrics are total_value only. 
        LocalDate since = LocalDate.now(); // LocalDate | Start date (YYYY-MM-DD). Defaults to 30 days ago.
        LocalDate until = LocalDate.now(); // LocalDate | End date (YYYY-MM-DD). Defaults to today.
        String metricType = "time_series"; // String | \"total_value\" (default) returns aggregated totals and supports breakdowns. \"time_series\" returns daily values but only works with the \"reach\" metric. 
        String breakdown = "breakdown_example"; // String | Breakdown dimension (only valid with metricType=total_value). Valid values depend on the metric: media_product_type, follow_type, follower_type, contact_button_type. 
        try {
            ApiResponse<InstagramAccountInsightsResponse> response = apiInstance.getInstagramAccountInsightsWithHttpInfo(accountId, metrics, since, until, metricType, breakdown);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getInstagramAccountInsights");
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
| **accountId** | **String**| The Zernio SocialAccount ID for the Instagram account | |
| **metrics** | **String**| Comma-separated list of metrics. Defaults to \&quot;reach,views,accounts_engaged,total_interactions\&quot;. Valid metrics: reach, views, accounts_engaged, total_interactions, comments, likes, saves, shares, replies, reposts, follows_and_unfollows, profile_links_taps. Note: only \&quot;reach\&quot; supports metricType&#x3D;time_series. All other metrics are total_value only.  | [optional] |
| **since** | **LocalDate**| Start date (YYYY-MM-DD). Defaults to 30 days ago. | [optional] |
| **until** | **LocalDate**| End date (YYYY-MM-DD). Defaults to today. | [optional] |
| **metricType** | **String**| \&quot;total_value\&quot; (default) returns aggregated totals and supports breakdowns. \&quot;time_series\&quot; returns daily values but only works with the \&quot;reach\&quot; metric.  | [optional] [default to total_value] [enum: time_series, total_value] |
| **breakdown** | **String**| Breakdown dimension (only valid with metricType&#x3D;total_value). Valid values depend on the metric: media_product_type, follow_type, follower_type, contact_button_type.  | [optional] |

### Return type

ApiResponse<[**InstagramAccountInsightsResponse**](InstagramAccountInsightsResponse.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Account insights data |  -  |
| **400** | Bad request (invalid parameters) |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **403** | Access denied to this account |  -  |
| **404** | Account not found |  -  |


## getInstagramDemographics

> InstagramDemographicsResponse getInstagramDemographics(accountId, metric, breakdown, timeframe)

Get Instagram demographics

Returns audience demographic insights for an Instagram account, broken down by age, city, country, and/or gender. Requires at least 100 followers. Returns top 45 entries per dimension. Data may be delayed up to 48 hours. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String accountId = "accountId_example"; // String | The Zernio SocialAccount ID for the Instagram account
        String metric = "follower_demographics"; // String | \"follower_demographics\" for follower audience data, or \"engaged_audience_demographics\" for engaged viewers. 
        String breakdown = "breakdown_example"; // String | Comma-separated list of demographic dimensions: age, city, country, gender. Defaults to all four if omitted. 
        String timeframe = "this_week"; // String | Time period for demographic data. Defaults to \"this_month\". 
        try {
            InstagramDemographicsResponse result = apiInstance.getInstagramDemographics(accountId, metric, breakdown, timeframe);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getInstagramDemographics");
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
| **accountId** | **String**| The Zernio SocialAccount ID for the Instagram account | |
| **metric** | **String**| \&quot;follower_demographics\&quot; for follower audience data, or \&quot;engaged_audience_demographics\&quot; for engaged viewers.  | [optional] [default to follower_demographics] [enum: follower_demographics, engaged_audience_demographics] |
| **breakdown** | **String**| Comma-separated list of demographic dimensions: age, city, country, gender. Defaults to all four if omitted.  | [optional] |
| **timeframe** | **String**| Time period for demographic data. Defaults to \&quot;this_month\&quot;.  | [optional] [default to this_month] [enum: this_week, this_month] |

### Return type

[**InstagramDemographicsResponse**](InstagramDemographicsResponse.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Demographic insights data |  -  |
| **400** | Bad request (invalid parameters) |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **403** | Access denied to this account |  -  |
| **404** | Account not found |  -  |

## getInstagramDemographicsWithHttpInfo

> ApiResponse<InstagramDemographicsResponse> getInstagramDemographics getInstagramDemographicsWithHttpInfo(accountId, metric, breakdown, timeframe)

Get Instagram demographics

Returns audience demographic insights for an Instagram account, broken down by age, city, country, and/or gender. Requires at least 100 followers. Returns top 45 entries per dimension. Data may be delayed up to 48 hours. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String accountId = "accountId_example"; // String | The Zernio SocialAccount ID for the Instagram account
        String metric = "follower_demographics"; // String | \"follower_demographics\" for follower audience data, or \"engaged_audience_demographics\" for engaged viewers. 
        String breakdown = "breakdown_example"; // String | Comma-separated list of demographic dimensions: age, city, country, gender. Defaults to all four if omitted. 
        String timeframe = "this_week"; // String | Time period for demographic data. Defaults to \"this_month\". 
        try {
            ApiResponse<InstagramDemographicsResponse> response = apiInstance.getInstagramDemographicsWithHttpInfo(accountId, metric, breakdown, timeframe);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getInstagramDemographics");
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
| **accountId** | **String**| The Zernio SocialAccount ID for the Instagram account | |
| **metric** | **String**| \&quot;follower_demographics\&quot; for follower audience data, or \&quot;engaged_audience_demographics\&quot; for engaged viewers.  | [optional] [default to follower_demographics] [enum: follower_demographics, engaged_audience_demographics] |
| **breakdown** | **String**| Comma-separated list of demographic dimensions: age, city, country, gender. Defaults to all four if omitted.  | [optional] |
| **timeframe** | **String**| Time period for demographic data. Defaults to \&quot;this_month\&quot;.  | [optional] [default to this_month] [enum: this_week, this_month] |

### Return type

ApiResponse<[**InstagramDemographicsResponse**](InstagramDemographicsResponse.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Demographic insights data |  -  |
| **400** | Bad request (invalid parameters) |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **403** | Access denied to this account |  -  |
| **404** | Account not found |  -  |


## getLinkedInAggregateAnalytics

> GetLinkedInAggregateAnalytics200Response getLinkedInAggregateAnalytics(accountId, aggregation, startDate, endDate, metrics)

Get LinkedIn aggregate stats

Returns aggregate analytics across all posts for a LinkedIn personal account. Only includes posts published through Zernio (LinkedIn API limitation). Org accounts should use /v1/analytics instead. Requires r_member_postAnalytics scope.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Returns aggregate analytics across all posts for a LinkedIn personal account. Only includes posts published through Zernio (LinkedIn API limitation). Org accounts should use /v1/analytics instead. Requires r_member_postAnalytics scope.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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


## getLinkedInPostReactions

> GetLinkedInPostReactions200Response getLinkedInPostReactions(accountId, urn, limit, cursor)

Get LinkedIn post reactions

Returns individual reactions for a specific LinkedIn post, including reactor profiles (name, headline/job title, profile picture, profile URL, reaction type). Only works for organization/company page accounts. LinkedIn restricts reaction data for personal profiles (r_member_social_feed is a closed permission). 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String accountId = "accountId_example"; // String | The ID of the LinkedIn organization account
        String urn = "urn:li:share:7123456789012345678"; // String | The LinkedIn post URN
        Integer limit = 25; // Integer | Maximum number of reactions to return per page
        String cursor = "cursor_example"; // String | Offset-based pagination start index
        try {
            GetLinkedInPostReactions200Response result = apiInstance.getLinkedInPostReactions(accountId, urn, limit, cursor);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getLinkedInPostReactions");
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
| **accountId** | **String**| The ID of the LinkedIn organization account | |
| **urn** | **String**| The LinkedIn post URN | |
| **limit** | **Integer**| Maximum number of reactions to return per page | [optional] [default to 25] |
| **cursor** | **String**| Offset-based pagination start index | [optional] |

### Return type

[**GetLinkedInPostReactions200Response**](GetLinkedInPostReactions200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Reactions with reactor profiles |  -  |
| **400** | Invalid request or platform limitation |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **403** | Missing required LinkedIn scope |  -  |
| **404** | Account or post not found |  -  |

## getLinkedInPostReactionsWithHttpInfo

> ApiResponse<GetLinkedInPostReactions200Response> getLinkedInPostReactions getLinkedInPostReactionsWithHttpInfo(accountId, urn, limit, cursor)

Get LinkedIn post reactions

Returns individual reactions for a specific LinkedIn post, including reactor profiles (name, headline/job title, profile picture, profile URL, reaction type). Only works for organization/company page accounts. LinkedIn restricts reaction data for personal profiles (r_member_social_feed is a closed permission). 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String accountId = "accountId_example"; // String | The ID of the LinkedIn organization account
        String urn = "urn:li:share:7123456789012345678"; // String | The LinkedIn post URN
        Integer limit = 25; // Integer | Maximum number of reactions to return per page
        String cursor = "cursor_example"; // String | Offset-based pagination start index
        try {
            ApiResponse<GetLinkedInPostReactions200Response> response = apiInstance.getLinkedInPostReactionsWithHttpInfo(accountId, urn, limit, cursor);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getLinkedInPostReactions");
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
| **accountId** | **String**| The ID of the LinkedIn organization account | |
| **urn** | **String**| The LinkedIn post URN | |
| **limit** | **Integer**| Maximum number of reactions to return per page | [optional] [default to 25] |
| **cursor** | **String**| Offset-based pagination start index | [optional] |

### Return type

ApiResponse<[**GetLinkedInPostReactions200Response**](GetLinkedInPostReactions200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Reactions with reactor profiles |  -  |
| **400** | Invalid request or platform limitation |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **403** | Missing required LinkedIn scope |  -  |
| **404** | Account or post not found |  -  |


## getPostTimeline

> GetPostTimeline200Response getPostTimeline(postId, fromDate, toDate)

Get post analytics timeline

Returns a daily timeline of analytics metrics for a specific post, showing how impressions, likes, and other metrics evolved day-by-day since publishing. Each row represents one day of data per platform. For multi-platform Zernio posts, returns separate rows for each platform. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String postId = "postId_example"; // String | The post to fetch timeline for. Accepts an ExternalPost ID, a platformPostId, or a Zernio Post ID. 
        OffsetDateTime fromDate = OffsetDateTime.now(); // OffsetDateTime | Start of date range (ISO 8601). Defaults to 90 days ago.
        OffsetDateTime toDate = OffsetDateTime.now(); // OffsetDateTime | End of date range (ISO 8601). Defaults to now.
        try {
            GetPostTimeline200Response result = apiInstance.getPostTimeline(postId, fromDate, toDate);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getPostTimeline");
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
| **postId** | **String**| The post to fetch timeline for. Accepts an ExternalPost ID, a platformPostId, or a Zernio Post ID.  | |
| **fromDate** | **OffsetDateTime**| Start of date range (ISO 8601). Defaults to 90 days ago. | [optional] |
| **toDate** | **OffsetDateTime**| End of date range (ISO 8601). Defaults to now. | [optional] |

### Return type

[**GetPostTimeline200Response**](GetPostTimeline200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Daily analytics timeline |  -  |
| **400** | Missing required postId parameter |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **403** | Forbidden (post belongs to another user or API key scope violation) |  -  |
| **404** | Post not found |  -  |

## getPostTimelineWithHttpInfo

> ApiResponse<GetPostTimeline200Response> getPostTimeline getPostTimelineWithHttpInfo(postId, fromDate, toDate)

Get post analytics timeline

Returns a daily timeline of analytics metrics for a specific post, showing how impressions, likes, and other metrics evolved day-by-day since publishing. Each row represents one day of data per platform. For multi-platform Zernio posts, returns separate rows for each platform. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String postId = "postId_example"; // String | The post to fetch timeline for. Accepts an ExternalPost ID, a platformPostId, or a Zernio Post ID. 
        OffsetDateTime fromDate = OffsetDateTime.now(); // OffsetDateTime | Start of date range (ISO 8601). Defaults to 90 days ago.
        OffsetDateTime toDate = OffsetDateTime.now(); // OffsetDateTime | End of date range (ISO 8601). Defaults to now.
        try {
            ApiResponse<GetPostTimeline200Response> response = apiInstance.getPostTimelineWithHttpInfo(postId, fromDate, toDate);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getPostTimeline");
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
| **postId** | **String**| The post to fetch timeline for. Accepts an ExternalPost ID, a platformPostId, or a Zernio Post ID.  | |
| **fromDate** | **OffsetDateTime**| Start of date range (ISO 8601). Defaults to 90 days ago. | [optional] |
| **toDate** | **OffsetDateTime**| End of date range (ISO 8601). Defaults to now. | [optional] |

### Return type

ApiResponse<[**GetPostTimeline200Response**](GetPostTimeline200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Daily analytics timeline |  -  |
| **400** | Missing required postId parameter |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **403** | Forbidden (post belongs to another user or API key scope violation) |  -  |
| **404** | Post not found |  -  |


## getPostingFrequency

> GetPostingFrequency200Response getPostingFrequency(platform, profileId, source)

Get frequency vs engagement

Returns the correlation between posting frequency (posts per week) and engagement rate, broken down by platform. Helps find the optimal posting cadence for each platform. Each row represents a specific (platform, posts_per_week) combination with the average engagement rate observed across all weeks matching that frequency. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String platform = "platform_example"; // String | Filter by platform (e.g. \"instagram\", \"tiktok\"). Omit for all platforms.
        String profileId = "profileId_example"; // String | Filter by profile ID. Omit for all profiles.
        String source = "all"; // String | Filter by post origin. \"late\" for posts published via Zernio, \"external\" for posts imported from platforms.
        try {
            GetPostingFrequency200Response result = apiInstance.getPostingFrequency(platform, profileId, source);
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
| **source** | **String**| Filter by post origin. \&quot;late\&quot; for posts published via Zernio, \&quot;external\&quot; for posts imported from platforms. | [optional] [default to all] [enum: all, late, external] |

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

> ApiResponse<GetPostingFrequency200Response> getPostingFrequency getPostingFrequencyWithHttpInfo(platform, profileId, source)

Get frequency vs engagement

Returns the correlation between posting frequency (posts per week) and engagement rate, broken down by platform. Helps find the optimal posting cadence for each platform. Each row represents a specific (platform, posts_per_week) combination with the average engagement rate observed across all weeks matching that frequency. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String platform = "platform_example"; // String | Filter by platform (e.g. \"instagram\", \"tiktok\"). Omit for all platforms.
        String profileId = "profileId_example"; // String | Filter by profile ID. Omit for all profiles.
        String source = "all"; // String | Filter by post origin. \"late\" for posts published via Zernio, \"external\" for posts imported from platforms.
        try {
            ApiResponse<GetPostingFrequency200Response> response = apiInstance.getPostingFrequencyWithHttpInfo(platform, profileId, source);
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
| **source** | **String**| Filter by post origin. \&quot;late\&quot; for posts published via Zernio, \&quot;external\&quot; for posts imported from platforms. | [optional] [default to all] [enum: all, late, external] |

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
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String videoId = "videoId_example"; // String | The YouTube video ID (e.g., \"dQw4w9WgXcQ\")
        String accountId = "accountId_example"; // String | The Zernio account ID for the YouTube account
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
| **accountId** | **String**| The Zernio account ID for the YouTube account | |
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
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String videoId = "videoId_example"; // String | The YouTube video ID (e.g., \"dQw4w9WgXcQ\")
        String accountId = "accountId_example"; // String | The Zernio account ID for the YouTube account
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
| **accountId** | **String**| The Zernio account ID for the YouTube account | |
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


## getYouTubeDemographics

> YouTubeDemographicsResponse getYouTubeDemographics(accountId, breakdown, startDate, endDate)

Get YouTube demographics

Returns audience demographic insights for a YouTube channel, broken down by age, gender, and/or country. Age and gender values are viewer percentages (0-100). Country values are view counts. Data is based on signed-in viewers only, with a 2-3 day delay. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String accountId = "accountId_example"; // String | The Zernio SocialAccount ID for the YouTube account
        String breakdown = "breakdown_example"; // String | Comma-separated list of demographic dimensions: age, gender, country. Defaults to all three if omitted. 
        LocalDate startDate = LocalDate.now(); // LocalDate | Start date in YYYY-MM-DD format. Defaults to 90 days ago. 
        LocalDate endDate = LocalDate.now(); // LocalDate | End date in YYYY-MM-DD format. Defaults to 3 days ago (YouTube data latency). 
        try {
            YouTubeDemographicsResponse result = apiInstance.getYouTubeDemographics(accountId, breakdown, startDate, endDate);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getYouTubeDemographics");
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
| **accountId** | **String**| The Zernio SocialAccount ID for the YouTube account | |
| **breakdown** | **String**| Comma-separated list of demographic dimensions: age, gender, country. Defaults to all three if omitted.  | [optional] |
| **startDate** | **LocalDate**| Start date in YYYY-MM-DD format. Defaults to 90 days ago.  | [optional] |
| **endDate** | **LocalDate**| End date in YYYY-MM-DD format. Defaults to 3 days ago (YouTube data latency).  | [optional] |

### Return type

[**YouTubeDemographicsResponse**](YouTubeDemographicsResponse.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Demographic insights data |  -  |
| **400** | Bad request (invalid parameters or not a YouTube account) |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **403** | Access denied to this account |  -  |
| **404** | Account not found |  -  |
| **412** | YouTube Analytics scope not granted |  -  |

## getYouTubeDemographicsWithHttpInfo

> ApiResponse<YouTubeDemographicsResponse> getYouTubeDemographics getYouTubeDemographicsWithHttpInfo(accountId, breakdown, startDate, endDate)

Get YouTube demographics

Returns audience demographic insights for a YouTube channel, broken down by age, gender, and/or country. Age and gender values are viewer percentages (0-100). Country values are view counts. Data is based on signed-in viewers only, with a 2-3 day delay. Requires the Analytics add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AnalyticsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AnalyticsApi apiInstance = new AnalyticsApi(defaultClient);
        String accountId = "accountId_example"; // String | The Zernio SocialAccount ID for the YouTube account
        String breakdown = "breakdown_example"; // String | Comma-separated list of demographic dimensions: age, gender, country. Defaults to all three if omitted. 
        LocalDate startDate = LocalDate.now(); // LocalDate | Start date in YYYY-MM-DD format. Defaults to 90 days ago. 
        LocalDate endDate = LocalDate.now(); // LocalDate | End date in YYYY-MM-DD format. Defaults to 3 days ago (YouTube data latency). 
        try {
            ApiResponse<YouTubeDemographicsResponse> response = apiInstance.getYouTubeDemographicsWithHttpInfo(accountId, breakdown, startDate, endDate);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AnalyticsApi#getYouTubeDemographics");
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
| **accountId** | **String**| The Zernio SocialAccount ID for the YouTube account | |
| **breakdown** | **String**| Comma-separated list of demographic dimensions: age, gender, country. Defaults to all three if omitted.  | [optional] |
| **startDate** | **LocalDate**| Start date in YYYY-MM-DD format. Defaults to 90 days ago.  | [optional] |
| **endDate** | **LocalDate**| End date in YYYY-MM-DD format. Defaults to 3 days ago (YouTube data latency).  | [optional] |

### Return type

ApiResponse<[**YouTubeDemographicsResponse**](YouTubeDemographicsResponse.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Demographic insights data |  -  |
| **400** | Bad request (invalid parameters or not a YouTube account) |  -  |
| **401** | Unauthorized |  -  |
| **402** | Analytics add-on required |  -  |
| **403** | Access denied to this account |  -  |
| **404** | Account not found |  -  |
| **412** | YouTube Analytics scope not granted |  -  |

