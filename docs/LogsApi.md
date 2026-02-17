# LogsApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getPostLogs**](LogsApi.md#getPostLogs) | **GET** /v1/posts/{postId}/logs | Get post logs |
| [**getPostLogsWithHttpInfo**](LogsApi.md#getPostLogsWithHttpInfo) | **GET** /v1/posts/{postId}/logs | Get post logs |
| [**listConnectionLogs**](LogsApi.md#listConnectionLogs) | **GET** /v1/connections/logs | List connection logs |
| [**listConnectionLogsWithHttpInfo**](LogsApi.md#listConnectionLogsWithHttpInfo) | **GET** /v1/connections/logs | List connection logs |
| [**listPostsLogs**](LogsApi.md#listPostsLogs) | **GET** /v1/posts/logs | List publishing logs |
| [**listPostsLogsWithHttpInfo**](LogsApi.md#listPostsLogsWithHttpInfo) | **GET** /v1/posts/logs | List publishing logs |



## getPostLogs

> GetPostLogs200Response getPostLogs(postId, limit)

Get post logs

Retrieve all publishing logs for a specific post. Shows the complete history of publishing attempts for that post across all platforms. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.LogsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LogsApi apiInstance = new LogsApi(defaultClient);
        String postId = "postId_example"; // String | The post ID
        Integer limit = 50; // Integer | Maximum number of logs to return (max 100)
        try {
            GetPostLogs200Response result = apiInstance.getPostLogs(postId, limit);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling LogsApi#getPostLogs");
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
| **postId** | **String**| The post ID | |
| **limit** | **Integer**| Maximum number of logs to return (max 100) | [optional] [default to 50] |

### Return type

[**GetPostLogs200Response**](GetPostLogs200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Post logs retrieved successfully |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden - not authorized to view this post |  -  |
| **404** | Resource not found |  -  |

## getPostLogsWithHttpInfo

> ApiResponse<GetPostLogs200Response> getPostLogs getPostLogsWithHttpInfo(postId, limit)

Get post logs

Retrieve all publishing logs for a specific post. Shows the complete history of publishing attempts for that post across all platforms. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.LogsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LogsApi apiInstance = new LogsApi(defaultClient);
        String postId = "postId_example"; // String | The post ID
        Integer limit = 50; // Integer | Maximum number of logs to return (max 100)
        try {
            ApiResponse<GetPostLogs200Response> response = apiInstance.getPostLogsWithHttpInfo(postId, limit);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling LogsApi#getPostLogs");
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
| **postId** | **String**| The post ID | |
| **limit** | **Integer**| Maximum number of logs to return (max 100) | [optional] [default to 50] |

### Return type

ApiResponse<[**GetPostLogs200Response**](GetPostLogs200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Post logs retrieved successfully |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden - not authorized to view this post |  -  |
| **404** | Resource not found |  -  |


## listConnectionLogs

> ListConnectionLogs200Response listConnectionLogs(platform, eventType, status, days, limit, skip)

List connection logs

Retrieve connection event logs showing account connection and disconnection history. Event types: connect_success, connect_failed, disconnect, reconnect_success, reconnect_failed. Logs are automatically deleted after 7 days. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.LogsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LogsApi apiInstance = new LogsApi(defaultClient);
        String platform = "tiktok"; // String | Filter by platform
        String eventType = "connect_success"; // String | Filter by event type
        String status = "success"; // String | Filter by status (shorthand for event types)
        Integer days = 7; // Integer | Number of days to look back (max 7)
        Integer limit = 50; // Integer | Maximum number of logs to return (max 100)
        Integer skip = 0; // Integer | Number of logs to skip (for pagination)
        try {
            ListConnectionLogs200Response result = apiInstance.listConnectionLogs(platform, eventType, status, days, limit, skip);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling LogsApi#listConnectionLogs");
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
| **platform** | **String**| Filter by platform | [optional] [enum: tiktok, instagram, facebook, youtube, linkedin, twitter, threads, pinterest, reddit, bluesky, googlebusiness, telegram, snapchat, all] |
| **eventType** | **String**| Filter by event type | [optional] [enum: connect_success, connect_failed, disconnect, reconnect_success, reconnect_failed, all] |
| **status** | **String**| Filter by status (shorthand for event types) | [optional] [enum: success, failed, all] |
| **days** | **Integer**| Number of days to look back (max 7) | [optional] [default to 7] |
| **limit** | **Integer**| Maximum number of logs to return (max 100) | [optional] [default to 50] |
| **skip** | **Integer**| Number of logs to skip (for pagination) | [optional] [default to 0] |

### Return type

[**ListConnectionLogs200Response**](ListConnectionLogs200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Connection logs retrieved successfully |  -  |
| **401** | Unauthorized |  -  |

## listConnectionLogsWithHttpInfo

> ApiResponse<ListConnectionLogs200Response> listConnectionLogs listConnectionLogsWithHttpInfo(platform, eventType, status, days, limit, skip)

List connection logs

Retrieve connection event logs showing account connection and disconnection history. Event types: connect_success, connect_failed, disconnect, reconnect_success, reconnect_failed. Logs are automatically deleted after 7 days. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.LogsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LogsApi apiInstance = new LogsApi(defaultClient);
        String platform = "tiktok"; // String | Filter by platform
        String eventType = "connect_success"; // String | Filter by event type
        String status = "success"; // String | Filter by status (shorthand for event types)
        Integer days = 7; // Integer | Number of days to look back (max 7)
        Integer limit = 50; // Integer | Maximum number of logs to return (max 100)
        Integer skip = 0; // Integer | Number of logs to skip (for pagination)
        try {
            ApiResponse<ListConnectionLogs200Response> response = apiInstance.listConnectionLogsWithHttpInfo(platform, eventType, status, days, limit, skip);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling LogsApi#listConnectionLogs");
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
| **platform** | **String**| Filter by platform | [optional] [enum: tiktok, instagram, facebook, youtube, linkedin, twitter, threads, pinterest, reddit, bluesky, googlebusiness, telegram, snapchat, all] |
| **eventType** | **String**| Filter by event type | [optional] [enum: connect_success, connect_failed, disconnect, reconnect_success, reconnect_failed, all] |
| **status** | **String**| Filter by status (shorthand for event types) | [optional] [enum: success, failed, all] |
| **days** | **Integer**| Number of days to look back (max 7) | [optional] [default to 7] |
| **limit** | **Integer**| Maximum number of logs to return (max 100) | [optional] [default to 50] |
| **skip** | **Integer**| Number of logs to skip (for pagination) | [optional] [default to 0] |

### Return type

ApiResponse<[**ListConnectionLogs200Response**](ListConnectionLogs200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Connection logs retrieved successfully |  -  |
| **401** | Unauthorized |  -  |


## listPostsLogs

> ListPostsLogs200Response listPostsLogs(status, platform, action, days, limit, skip)

List publishing logs

Retrieve publishing logs for all posts with detailed information about each publishing attempt. Filter by status, platform, or action. Logs are automatically deleted after 7 days. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.LogsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LogsApi apiInstance = new LogsApi(defaultClient);
        String status = "success"; // String | Filter by log status
        String platform = "tiktok"; // String | Filter by platform
        String action = "publish"; // String | Filter by action type
        Integer days = 7; // Integer | Number of days to look back (max 7)
        Integer limit = 50; // Integer | Maximum number of logs to return (max 100)
        Integer skip = 0; // Integer | Number of logs to skip (for pagination)
        try {
            ListPostsLogs200Response result = apiInstance.listPostsLogs(status, platform, action, days, limit, skip);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling LogsApi#listPostsLogs");
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
| **status** | **String**| Filter by log status | [optional] [enum: success, failed, pending, skipped, all] |
| **platform** | **String**| Filter by platform | [optional] [enum: tiktok, instagram, facebook, youtube, linkedin, twitter, threads, pinterest, reddit, bluesky, googlebusiness, telegram, snapchat, all] |
| **action** | **String**| Filter by action type | [optional] [enum: publish, retry, media_upload, rate_limit_pause, token_refresh, cancelled, all] |
| **days** | **Integer**| Number of days to look back (max 7) | [optional] [default to 7] |
| **limit** | **Integer**| Maximum number of logs to return (max 100) | [optional] [default to 50] |
| **skip** | **Integer**| Number of logs to skip (for pagination) | [optional] [default to 0] |

### Return type

[**ListPostsLogs200Response**](ListPostsLogs200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Publishing logs retrieved successfully |  -  |
| **401** | Unauthorized |  -  |

## listPostsLogsWithHttpInfo

> ApiResponse<ListPostsLogs200Response> listPostsLogs listPostsLogsWithHttpInfo(status, platform, action, days, limit, skip)

List publishing logs

Retrieve publishing logs for all posts with detailed information about each publishing attempt. Filter by status, platform, or action. Logs are automatically deleted after 7 days. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.LogsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LogsApi apiInstance = new LogsApi(defaultClient);
        String status = "success"; // String | Filter by log status
        String platform = "tiktok"; // String | Filter by platform
        String action = "publish"; // String | Filter by action type
        Integer days = 7; // Integer | Number of days to look back (max 7)
        Integer limit = 50; // Integer | Maximum number of logs to return (max 100)
        Integer skip = 0; // Integer | Number of logs to skip (for pagination)
        try {
            ApiResponse<ListPostsLogs200Response> response = apiInstance.listPostsLogsWithHttpInfo(status, platform, action, days, limit, skip);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling LogsApi#listPostsLogs");
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
| **status** | **String**| Filter by log status | [optional] [enum: success, failed, pending, skipped, all] |
| **platform** | **String**| Filter by platform | [optional] [enum: tiktok, instagram, facebook, youtube, linkedin, twitter, threads, pinterest, reddit, bluesky, googlebusiness, telegram, snapchat, all] |
| **action** | **String**| Filter by action type | [optional] [enum: publish, retry, media_upload, rate_limit_pause, token_refresh, cancelled, all] |
| **days** | **Integer**| Number of days to look back (max 7) | [optional] [default to 7] |
| **limit** | **Integer**| Maximum number of logs to return (max 100) | [optional] [default to 50] |
| **skip** | **Integer**| Number of logs to skip (for pagination) | [optional] [default to 0] |

### Return type

ApiResponse<[**ListPostsLogs200Response**](ListPostsLogs200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Publishing logs retrieved successfully |  -  |
| **401** | Unauthorized |  -  |

