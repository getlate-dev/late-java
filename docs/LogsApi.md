# LogsApi

All URIs are relative to *https://zernio.com/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getPostLogs**](LogsApi.md#getPostLogs) | **GET** /v1/posts/{postId}/logs | Get post logs |
| [**getPostLogsWithHttpInfo**](LogsApi.md#getPostLogsWithHttpInfo) | **GET** /v1/posts/{postId}/logs | Get post logs |
| [**listLogs**](LogsApi.md#listLogs) | **GET** /v1/logs | List activity logs |
| [**listLogsWithHttpInfo**](LogsApi.md#listLogsWithHttpInfo) | **GET** /v1/logs | List activity logs |



## getPostLogs

> GetPostLogs200Response getPostLogs(postId, limit)

Get post logs

Retrieve all publishing logs for a specific post. Shows the complete history of publishing attempts for that post across all platforms. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LogsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LogsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

> ListLogs200Response listLogs(type, status, platform, action, search, days, limit, skip)

List activity logs

Unified logs endpoint. Returns logs for publishing, connections, webhooks, and messaging. Filter by type, platform, status, and time range. Logs are retained for 90 days. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LogsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LogsApi apiInstance = new LogsApi(defaultClient);
        String type = "publishing"; // String | Log category to query
        String status = "success"; // String | Filter by status
        String platform = "tiktok"; // String | Filter by platform
        String action = "action_example"; // String | Filter by action (e.g., post.published, message.sent, account.connected, webhook.delivered)
        String search = "search_example"; // String | Free-text search across log fields
        Integer days = 90; // Integer | Number of days to look back (max 90)
        Integer limit = 50; // Integer | Maximum number of logs to return (max 100)
        Integer skip = 0; // Integer | Number of logs to skip (for pagination)
        try {
            ListLogs200Response result = apiInstance.listLogs(type, status, platform, action, search, days, limit, skip);
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
| **type** | **String**| Log category to query | [optional] [default to publishing] [enum: publishing, connections, webhooks, messaging] |
| **status** | **String**| Filter by status | [optional] [enum: success, failed, pending, skipped, all] |
| **platform** | **String**| Filter by platform | [optional] [enum: tiktok, instagram, whatsapp, facebook, youtube, linkedin, twitter, threads, pinterest, reddit, bluesky, googlebusiness, telegram, snapchat, all] |
| **action** | **String**| Filter by action (e.g., post.published, message.sent, account.connected, webhook.delivered) | [optional] |
| **search** | **String**| Free-text search across log fields | [optional] |
| **days** | **Integer**| Number of days to look back (max 90) | [optional] [default to 90] |
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
| **200** | Logs retrieved successfully |  -  |
| **401** | Unauthorized |  -  |

## listLogsWithHttpInfo

> ApiResponse<ListLogs200Response> listLogs listLogsWithHttpInfo(type, status, platform, action, search, days, limit, skip)

List activity logs

Unified logs endpoint. Returns logs for publishing, connections, webhooks, and messaging. Filter by type, platform, status, and time range. Logs are retained for 90 days. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LogsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LogsApi apiInstance = new LogsApi(defaultClient);
        String type = "publishing"; // String | Log category to query
        String status = "success"; // String | Filter by status
        String platform = "tiktok"; // String | Filter by platform
        String action = "action_example"; // String | Filter by action (e.g., post.published, message.sent, account.connected, webhook.delivered)
        String search = "search_example"; // String | Free-text search across log fields
        Integer days = 90; // Integer | Number of days to look back (max 90)
        Integer limit = 50; // Integer | Maximum number of logs to return (max 100)
        Integer skip = 0; // Integer | Number of logs to skip (for pagination)
        try {
            ApiResponse<ListLogs200Response> response = apiInstance.listLogsWithHttpInfo(type, status, platform, action, search, days, limit, skip);
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
| **type** | **String**| Log category to query | [optional] [default to publishing] [enum: publishing, connections, webhooks, messaging] |
| **status** | **String**| Filter by status | [optional] [enum: success, failed, pending, skipped, all] |
| **platform** | **String**| Filter by platform | [optional] [enum: tiktok, instagram, whatsapp, facebook, youtube, linkedin, twitter, threads, pinterest, reddit, bluesky, googlebusiness, telegram, snapchat, all] |
| **action** | **String**| Filter by action (e.g., post.published, message.sent, account.connected, webhook.delivered) | [optional] |
| **search** | **String**| Free-text search across log fields | [optional] |
| **days** | **Integer**| Number of days to look back (max 90) | [optional] [default to 90] |
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
| **200** | Logs retrieved successfully |  -  |
| **401** | Unauthorized |  -  |

