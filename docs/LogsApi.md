# LogsApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getLog**](LogsApi.md#getLog) | **GET** /v1/logs/{logId} | Get a single log entry |
| [**getLogWithHttpInfo**](LogsApi.md#getLogWithHttpInfo) | **GET** /v1/logs/{logId} | Get a single log entry |
| [**getPostLogs**](LogsApi.md#getPostLogs) | **GET** /v1/posts/{postId}/logs | Get logs for a specific post |
| [**getPostLogsWithHttpInfo**](LogsApi.md#getPostLogsWithHttpInfo) | **GET** /v1/posts/{postId}/logs | Get logs for a specific post |
| [**listLogs**](LogsApi.md#listLogs) | **GET** /v1/logs | Get publishing logs |
| [**listLogsWithHttpInfo**](LogsApi.md#listLogsWithHttpInfo) | **GET** /v1/logs | Get publishing logs |



## getLog

> GetLog200Response getLog(logId)

Get a single log entry

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

Get a single log entry

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

Get logs for a specific post

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

Get logs for a specific post

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


## listLogs

> ListLogs200Response listLogs(status, platform, action, days, limit, skip)

Get publishing logs

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

Get publishing logs

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

