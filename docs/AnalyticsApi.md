# AnalyticsApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getAnalytics**](AnalyticsApi.md#getAnalytics) | **GET** /v1/analytics | Get post analytics |
| [**getAnalyticsWithHttpInfo**](AnalyticsApi.md#getAnalyticsWithHttpInfo) | **GET** /v1/analytics | Get post analytics |
| [**getFollowerStats**](AnalyticsApi.md#getFollowerStats) | **GET** /v1/accounts/follower-stats | Get follower stats |
| [**getFollowerStatsWithHttpInfo**](AnalyticsApi.md#getFollowerStatsWithHttpInfo) | **GET** /v1/accounts/follower-stats | Get follower stats |
| [**getLinkedInAggregateAnalytics**](AnalyticsApi.md#getLinkedInAggregateAnalytics) | **GET** /v1/accounts/{accountId}/linkedin-aggregate-analytics | Get LinkedIn aggregate stats |
| [**getLinkedInAggregateAnalyticsWithHttpInfo**](AnalyticsApi.md#getLinkedInAggregateAnalyticsWithHttpInfo) | **GET** /v1/accounts/{accountId}/linkedin-aggregate-analytics | Get LinkedIn aggregate stats |
| [**getLinkedInPostAnalytics**](AnalyticsApi.md#getLinkedInPostAnalytics) | **GET** /v1/accounts/{accountId}/linkedin-post-analytics | Get LinkedIn post stats |
| [**getLinkedInPostAnalyticsWithHttpInfo**](AnalyticsApi.md#getLinkedInPostAnalyticsWithHttpInfo) | **GET** /v1/accounts/{accountId}/linkedin-post-analytics | Get LinkedIn post stats |
| [**getYouTubeDailyViews**](AnalyticsApi.md#getYouTubeDailyViews) | **GET** /v1/analytics/youtube/daily-views | Get YouTube daily views |
| [**getYouTubeDailyViewsWithHttpInfo**](AnalyticsApi.md#getYouTubeDailyViewsWithHttpInfo) | **GET** /v1/analytics/youtube/daily-views | Get YouTube daily views |



## getAnalytics

> GetAnalytics200Response getAnalytics(postId, platform, profileId, source, fromDate, toDate, limit, page, sortBy, order)

Get post analytics

Returns analytics for posts. With postId, returns a single post. Without it, returns a paginated list with overview stats. This endpoint returns External Post IDs by default. The postId parameter accepts both Late Post IDs and External Post IDs, auto-resolving Late IDs to External Post analytics. Use latePostId in responses to link back to your original post, or platformPostUrl as a stable identifier. isExternal indicates post origin (true &#x3D; synced from platform). For follower stats, use /v1/accounts/follower-stats. LinkedIn personal accounts: per-post analytics only for Late-published posts. Telegram: not available. Data is cached and refreshed at most once per hour. 

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

Returns analytics for posts. With postId, returns a single post. Without it, returns a paginated list with overview stats. This endpoint returns External Post IDs by default. The postId parameter accepts both Late Post IDs and External Post IDs, auto-resolving Late IDs to External Post analytics. Use latePostId in responses to link back to your original post, or platformPostUrl as a stable identifier. isExternal indicates post origin (true &#x3D; synced from platform). For follower stats, use /v1/accounts/follower-stats. LinkedIn personal accounts: per-post analytics only for Late-published posts. Telegram: not available. Data is cached and refreshed at most once per hour. 

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

Returns aggregate analytics across all posts for a LinkedIn personal account. Org accounts should use /v1/analytics instead. Required scope: r_member_postAnalytics (missing scope returns 403). Aggregation: TOTAL (default, lifetime totals) or DAILY (time series). Use startDate/endDate to filter. MEMBERS_REACHED is not available with DAILY aggregation. 

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
        String aggregation = "TOTAL"; // String | Type of aggregation: TOTAL (default, returns single totals) or DAILY (returns daily breakdown). Note: MEMBERS_REACHED is not available with DAILY aggregation. 
        LocalDate startDate = LocalDate.parse("2024-01-01"); // LocalDate | Start date for analytics data in YYYY-MM-DD format. If provided without endDate, endDate defaults to today. If omitted entirely, returns lifetime analytics. 
        LocalDate endDate = LocalDate.parse("2024-01-31"); // LocalDate | End date for analytics data in YYYY-MM-DD format (exclusive). If provided without startDate, startDate defaults to 30 days before endDate. 
        String metrics = "IMPRESSION,REACTION,COMMENT"; // String | Comma-separated list of metrics to fetch. If omitted, fetches all available metrics. Valid values: IMPRESSION, MEMBERS_REACHED, REACTION, COMMENT, RESHARE 
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
| **aggregation** | **String**| Type of aggregation: TOTAL (default, returns single totals) or DAILY (returns daily breakdown). Note: MEMBERS_REACHED is not available with DAILY aggregation.  | [optional] [default to TOTAL] [enum: TOTAL, DAILY] |
| **startDate** | **LocalDate**| Start date for analytics data in YYYY-MM-DD format. If provided without endDate, endDate defaults to today. If omitted entirely, returns lifetime analytics.  | [optional] |
| **endDate** | **LocalDate**| End date for analytics data in YYYY-MM-DD format (exclusive). If provided without startDate, startDate defaults to 30 days before endDate.  | [optional] |
| **metrics** | **String**| Comma-separated list of metrics to fetch. If omitted, fetches all available metrics. Valid values: IMPRESSION, MEMBERS_REACHED, REACTION, COMMENT, RESHARE  | [optional] |

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

Returns aggregate analytics across all posts for a LinkedIn personal account. Org accounts should use /v1/analytics instead. Required scope: r_member_postAnalytics (missing scope returns 403). Aggregation: TOTAL (default, lifetime totals) or DAILY (time series). Use startDate/endDate to filter. MEMBERS_REACHED is not available with DAILY aggregation. 

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
        String aggregation = "TOTAL"; // String | Type of aggregation: TOTAL (default, returns single totals) or DAILY (returns daily breakdown). Note: MEMBERS_REACHED is not available with DAILY aggregation. 
        LocalDate startDate = LocalDate.parse("2024-01-01"); // LocalDate | Start date for analytics data in YYYY-MM-DD format. If provided without endDate, endDate defaults to today. If omitted entirely, returns lifetime analytics. 
        LocalDate endDate = LocalDate.parse("2024-01-31"); // LocalDate | End date for analytics data in YYYY-MM-DD format (exclusive). If provided without startDate, startDate defaults to 30 days before endDate. 
        String metrics = "IMPRESSION,REACTION,COMMENT"; // String | Comma-separated list of metrics to fetch. If omitted, fetches all available metrics. Valid values: IMPRESSION, MEMBERS_REACHED, REACTION, COMMENT, RESHARE 
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
| **aggregation** | **String**| Type of aggregation: TOTAL (default, returns single totals) or DAILY (returns daily breakdown). Note: MEMBERS_REACHED is not available with DAILY aggregation.  | [optional] [default to TOTAL] [enum: TOTAL, DAILY] |
| **startDate** | **LocalDate**| Start date for analytics data in YYYY-MM-DD format. If provided without endDate, endDate defaults to today. If omitted entirely, returns lifetime analytics.  | [optional] |
| **endDate** | **LocalDate**| End date for analytics data in YYYY-MM-DD format (exclusive). If provided without startDate, startDate defaults to 30 days before endDate.  | [optional] |
| **metrics** | **String**| Comma-separated list of metrics to fetch. If omitted, fetches all available metrics. Valid values: IMPRESSION, MEMBERS_REACHED, REACTION, COMMENT, RESHARE  | [optional] |

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

Returns analytics for a specific LinkedIn post using its URN. Works for both personal and organization accounts. Useful for fetching analytics of posts not published through Late. Personal accounts require r_member_postAnalytics scope and return impressions, reach, likes, comments, shares, and video views (clicks not available). Organization accounts require r_organization_social scope and additionally return clicks and engagement rate. 

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

Returns analytics for a specific LinkedIn post using its URN. Works for both personal and organization accounts. Useful for fetching analytics of posts not published through Late. Personal accounts require r_member_postAnalytics scope and return impressions, reach, likes, comments, shares, and video views (clicks not available). Organization accounts require r_organization_social scope and additionally return clicks and engagement rate. 

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


## getYouTubeDailyViews

> YouTubeDailyViewsResponse getYouTubeDailyViews(videoId, accountId, startDate, endDate)

Get YouTube daily views

Returns historical daily view counts for a specific YouTube video. Uses YouTube Analytics API v2 to fetch daily breakdowns including views, watch time, and subscriber changes.  Requires the yt-analytics.readonly OAuth scope. Existing YouTube accounts may need to re-authorize. If the scope is missing, the response includes a reauthorizeUrl. Data has a 2-3 day delay; endDate is automatically capped to 3 days ago. Maximum 90 days of historical data. Defaults to last 30 days. 

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

Returns historical daily view counts for a specific YouTube video. Uses YouTube Analytics API v2 to fetch daily breakdowns including views, watch time, and subscriber changes.  Requires the yt-analytics.readonly OAuth scope. Existing YouTube accounts may need to re-authorize. If the scope is missing, the response includes a reauthorizeUrl. Data has a 2-3 day delay; endDate is automatically capped to 3 days ago. Maximum 90 days of historical data. Defaults to last 30 days. 

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

