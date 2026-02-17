# LogsApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getLog**](LogsApi.md#getLog) | **GET** /v1/logs/{logId} | Get log entry |
| [**getLogWithHttpInfo**](LogsApi.md#getLogWithHttpInfo) | **GET** /v1/logs/{logId} | Get log entry |
| [**getPostLogs**](LogsApi.md#getPostLogs) | **GET** /v1/posts/{postId}/logs | Get post logs |
| [**getPostLogsWithHttpInfo**](LogsApi.md#getPostLogsWithHttpInfo) | **GET** /v1/posts/{postId}/logs | Get post logs |
| [**listConnectionLogs**](LogsApi.md#listConnectionLogs) | **GET** /v1/connections/logs | List connection logs |
| [**listConnectionLogsWithHttpInfo**](LogsApi.md#listConnectionLogsWithHttpInfo) | **GET** /v1/connections/logs | List connection logs |
| [**listLogs**](LogsApi.md#listLogs) | **GET** /v1/logs | List publishing logs (deprecated) |
| [**listLogsWithHttpInfo**](LogsApi.md#listLogsWithHttpInfo) | **GET** /v1/logs | List publishing logs (deprecated) |
| [**listPostsLogs**](LogsApi.md#listPostsLogs) | **GET** /v1/posts/logs | List publishing logs |
| [**listPostsLogsWithHttpInfo**](LogsApi.md#listPostsLogsWithHttpInfo) | **GET** /v1/posts/logs | List publishing logs |



## getLog

> GetLog200Response getLog(logId)

Get log entry

Retrieve detailed information about a specific log entry, including full request and response bodies for debugging. 

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
        String logId = "logId_example"; // String | The log entry ID
        try {
            GetLog200Response result = apiInstance.getLog(logId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling LogsApi#getLog");
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
| **logId** | **String**| The log entry ID | |

### Return type

[**GetLog200Response**](GetLog200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Log entry retrieved successfully |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden - not authorized to view this log |  -  |
| **404** | Resource not found |  -  |

## getLogWithHttpInfo

> ApiResponse<GetLog200Response> getLog getLogWithHttpInfo(logId)

Get log entry

Retrieve detailed information about a specific log entry, including full request and response bodies for debugging. 

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
        String logId = "logId_example"; // String | The log entry ID
        try {
            ApiResponse<GetLog200Response> response = apiInstance.getLogWithHttpInfo(logId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling LogsApi#getLog");
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
| **logId** | **String**| The log entry ID | |

### Return type

ApiResponse<[**GetLog200Response**](GetLog200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Log entry retrieved successfully |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden - not authorized to view this log |  -  |
| **404** | Resource not found |  -  |


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

Retrieve connection event logs showing account connection and disconnection history. Useful for debugging OAuth issues and tracking account lifecycle.  **Event Types:** - &#x60;connect_success&#x60; - New account connected successfully - &#x60;connect_failed&#x60; - Connection attempt failed - &#x60;disconnect&#x60; - Account was disconnected - &#x60;reconnect_success&#x60; - Existing account reconnected - &#x60;reconnect_failed&#x60; - Reconnection attempt failed  **Retention:** Logs are automatically deleted after 7 days. 

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

Retrieve connection event logs showing account connection and disconnection history. Useful for debugging OAuth issues and tracking account lifecycle.  **Event Types:** - &#x60;connect_success&#x60; - New account connected successfully - &#x60;connect_failed&#x60; - Connection attempt failed - &#x60;disconnect&#x60; - Account was disconnected - &#x60;reconnect_success&#x60; - Existing account reconnected - &#x60;reconnect_failed&#x60; - Reconnection attempt failed  **Retention:** Logs are automatically deleted after 7 days. 

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


## listLogs

> ListLogs200Response listLogs(status, platform, action, days, limit, skip)

List publishing logs (deprecated)

**Deprecated:** Use &#x60;/v1/posts/logs&#x60; instead. This endpoint is maintained for backwards compatibility.  Retrieve publishing logs for all posts. Logs show detailed information about each publishing attempt including API requests, responses, and timing data.  **Filtering:** - Filter by status (success, failed, pending, skipped) - Filter by platform (instagram, twitter, linkedin, etc.) - Filter by action (publish, retry, rate_limit_pause, etc.)  **Retention:** Logs are automatically deleted after 7 days. 

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
            ListLogs200Response result = apiInstance.listLogs(status, platform, action, days, limit, skip);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling LogsApi#listLogs");
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

[**ListLogs200Response**](ListLogs200Response.md)


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

## listLogsWithHttpInfo

> ApiResponse<ListLogs200Response> listLogs listLogsWithHttpInfo(status, platform, action, days, limit, skip)

List publishing logs (deprecated)

**Deprecated:** Use &#x60;/v1/posts/logs&#x60; instead. This endpoint is maintained for backwards compatibility.  Retrieve publishing logs for all posts. Logs show detailed information about each publishing attempt including API requests, responses, and timing data.  **Filtering:** - Filter by status (success, failed, pending, skipped) - Filter by platform (instagram, twitter, linkedin, etc.) - Filter by action (publish, retry, rate_limit_pause, etc.)  **Retention:** Logs are automatically deleted after 7 days. 

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
            ApiResponse<ListLogs200Response> response = apiInstance.listLogsWithHttpInfo(status, platform, action, days, limit, skip);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling LogsApi#listLogs");
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

ApiResponse<[**ListLogs200Response**](ListLogs200Response.md)>


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


## listPostsLogs

> ListLogs200Response listPostsLogs(status, platform, action, days, limit, skip)

List publishing logs

Retrieve publishing logs for all posts. Logs show detailed information about each publishing attempt including API requests, responses, and timing data.  **Filtering:** - Filter by status (success, failed, pending, skipped) - Filter by platform (instagram, twitter, linkedin, etc.) - Filter by action (publish, retry, rate_limit_pause, etc.)  **Retention:** Logs are automatically deleted after 7 days. 

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
            ListLogs200Response result = apiInstance.listPostsLogs(status, platform, action, days, limit, skip);
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

[**ListLogs200Response**](ListLogs200Response.md)


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

> ApiResponse<ListLogs200Response> listPostsLogs listPostsLogsWithHttpInfo(status, platform, action, days, limit, skip)

List publishing logs

Retrieve publishing logs for all posts. Logs show detailed information about each publishing attempt including API requests, responses, and timing data.  **Filtering:** - Filter by status (success, failed, pending, skipped) - Filter by platform (instagram, twitter, linkedin, etc.) - Filter by action (publish, retry, rate_limit_pause, etc.)  **Retention:** Logs are automatically deleted after 7 days. 

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
            ApiResponse<ListLogs200Response> response = apiInstance.listPostsLogsWithHttpInfo(status, platform, action, days, limit, skip);
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

ApiResponse<[**ListLogs200Response**](ListLogs200Response.md)>


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

