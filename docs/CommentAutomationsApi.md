# CommentAutomationsApi

All URIs are relative to *https://zernio.com/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createCommentAutomation**](CommentAutomationsApi.md#createCommentAutomation) | **POST** /v1/comment-automations | Create comment-to-DM automation |
| [**createCommentAutomationWithHttpInfo**](CommentAutomationsApi.md#createCommentAutomationWithHttpInfo) | **POST** /v1/comment-automations | Create comment-to-DM automation |
| [**deleteCommentAutomation**](CommentAutomationsApi.md#deleteCommentAutomation) | **DELETE** /v1/comment-automations/{automationId} | Delete automation |
| [**deleteCommentAutomationWithHttpInfo**](CommentAutomationsApi.md#deleteCommentAutomationWithHttpInfo) | **DELETE** /v1/comment-automations/{automationId} | Delete automation |
| [**getCommentAutomation**](CommentAutomationsApi.md#getCommentAutomation) | **GET** /v1/comment-automations/{automationId} | Get automation details |
| [**getCommentAutomationWithHttpInfo**](CommentAutomationsApi.md#getCommentAutomationWithHttpInfo) | **GET** /v1/comment-automations/{automationId} | Get automation details |
| [**listCommentAutomationLogs**](CommentAutomationsApi.md#listCommentAutomationLogs) | **GET** /v1/comment-automations/{automationId}/logs | List automation logs |
| [**listCommentAutomationLogsWithHttpInfo**](CommentAutomationsApi.md#listCommentAutomationLogsWithHttpInfo) | **GET** /v1/comment-automations/{automationId}/logs | List automation logs |
| [**listCommentAutomations**](CommentAutomationsApi.md#listCommentAutomations) | **GET** /v1/comment-automations | List comment-to-DM automations |
| [**listCommentAutomationsWithHttpInfo**](CommentAutomationsApi.md#listCommentAutomationsWithHttpInfo) | **GET** /v1/comment-automations | List comment-to-DM automations |
| [**updateCommentAutomation**](CommentAutomationsApi.md#updateCommentAutomation) | **PATCH** /v1/comment-automations/{automationId} | Update automation settings |
| [**updateCommentAutomationWithHttpInfo**](CommentAutomationsApi.md#updateCommentAutomationWithHttpInfo) | **PATCH** /v1/comment-automations/{automationId} | Update automation settings |



## createCommentAutomation

> CreateCommentAutomation200Response createCommentAutomation(createCommentAutomationRequest)

Create comment-to-DM automation

Create a keyword-triggered DM automation on an Instagram or Facebook post. When someone comments a matching keyword, they automatically receive a DM. Only one active automation per post is allowed. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CommentAutomationsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentAutomationsApi apiInstance = new CommentAutomationsApi(defaultClient);
        CreateCommentAutomationRequest createCommentAutomationRequest = new CreateCommentAutomationRequest(); // CreateCommentAutomationRequest | 
        try {
            CreateCommentAutomation200Response result = apiInstance.createCommentAutomation(createCommentAutomationRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentAutomationsApi#createCommentAutomation");
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
| **createCommentAutomationRequest** | [**CreateCommentAutomationRequest**](CreateCommentAutomationRequest.md)|  | |

### Return type

[**CreateCommentAutomation200Response**](CreateCommentAutomation200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Automation created |  -  |
| **400** | Validation error |  -  |
| **401** | Unauthorized |  -  |
| **409** | Active automation already exists for this post |  -  |

## createCommentAutomationWithHttpInfo

> ApiResponse<CreateCommentAutomation200Response> createCommentAutomation createCommentAutomationWithHttpInfo(createCommentAutomationRequest)

Create comment-to-DM automation

Create a keyword-triggered DM automation on an Instagram or Facebook post. When someone comments a matching keyword, they automatically receive a DM. Only one active automation per post is allowed. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CommentAutomationsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentAutomationsApi apiInstance = new CommentAutomationsApi(defaultClient);
        CreateCommentAutomationRequest createCommentAutomationRequest = new CreateCommentAutomationRequest(); // CreateCommentAutomationRequest | 
        try {
            ApiResponse<CreateCommentAutomation200Response> response = apiInstance.createCommentAutomationWithHttpInfo(createCommentAutomationRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentAutomationsApi#createCommentAutomation");
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
| **createCommentAutomationRequest** | [**CreateCommentAutomationRequest**](CreateCommentAutomationRequest.md)|  | |

### Return type

ApiResponse<[**CreateCommentAutomation200Response**](CreateCommentAutomation200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Automation created |  -  |
| **400** | Validation error |  -  |
| **401** | Unauthorized |  -  |
| **409** | Active automation already exists for this post |  -  |


## deleteCommentAutomation

> void deleteCommentAutomation(automationId)

Delete automation

Permanently delete an automation and all its trigger logs.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CommentAutomationsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentAutomationsApi apiInstance = new CommentAutomationsApi(defaultClient);
        String automationId = "automationId_example"; // String | 
        try {
            apiInstance.deleteCommentAutomation(automationId);
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentAutomationsApi#deleteCommentAutomation");
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
| **automationId** | **String**|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Automation deleted |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## deleteCommentAutomationWithHttpInfo

> ApiResponse<Void> deleteCommentAutomation deleteCommentAutomationWithHttpInfo(automationId)

Delete automation

Permanently delete an automation and all its trigger logs.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CommentAutomationsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentAutomationsApi apiInstance = new CommentAutomationsApi(defaultClient);
        String automationId = "automationId_example"; // String | 
        try {
            ApiResponse<Void> response = apiInstance.deleteCommentAutomationWithHttpInfo(automationId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentAutomationsApi#deleteCommentAutomation");
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
| **automationId** | **String**|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Automation deleted |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## getCommentAutomation

> GetCommentAutomation200Response getCommentAutomation(automationId)

Get automation details

Returns an automation with its configuration, stats, and recent trigger logs.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CommentAutomationsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentAutomationsApi apiInstance = new CommentAutomationsApi(defaultClient);
        String automationId = "automationId_example"; // String | 
        try {
            GetCommentAutomation200Response result = apiInstance.getCommentAutomation(automationId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentAutomationsApi#getCommentAutomation");
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
| **automationId** | **String**|  | |

### Return type

[**GetCommentAutomation200Response**](GetCommentAutomation200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Automation details with stats and recent trigger logs |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## getCommentAutomationWithHttpInfo

> ApiResponse<GetCommentAutomation200Response> getCommentAutomation getCommentAutomationWithHttpInfo(automationId)

Get automation details

Returns an automation with its configuration, stats, and recent trigger logs.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CommentAutomationsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentAutomationsApi apiInstance = new CommentAutomationsApi(defaultClient);
        String automationId = "automationId_example"; // String | 
        try {
            ApiResponse<GetCommentAutomation200Response> response = apiInstance.getCommentAutomationWithHttpInfo(automationId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentAutomationsApi#getCommentAutomation");
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
| **automationId** | **String**|  | |

### Return type

ApiResponse<[**GetCommentAutomation200Response**](GetCommentAutomation200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Automation details with stats and recent trigger logs |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## listCommentAutomationLogs

> ListCommentAutomationLogs200Response listCommentAutomationLogs(automationId, status, limit, skip)

List automation logs

Paginated list of every comment that triggered this automation, with send status and commenter info.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CommentAutomationsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentAutomationsApi apiInstance = new CommentAutomationsApi(defaultClient);
        String automationId = "automationId_example"; // String | 
        String status = "sent"; // String | Filter by result status
        Integer limit = 50; // Integer | 
        Integer skip = 0; // Integer | 
        try {
            ListCommentAutomationLogs200Response result = apiInstance.listCommentAutomationLogs(automationId, status, limit, skip);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentAutomationsApi#listCommentAutomationLogs");
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
| **automationId** | **String**|  | |
| **status** | **String**| Filter by result status | [optional] [enum: sent, failed, skipped] |
| **limit** | **Integer**|  | [optional] [default to 50] |
| **skip** | **Integer**|  | [optional] [default to 0] |

### Return type

[**ListCommentAutomationLogs200Response**](ListCommentAutomationLogs200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Trigger logs with pagination |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## listCommentAutomationLogsWithHttpInfo

> ApiResponse<ListCommentAutomationLogs200Response> listCommentAutomationLogs listCommentAutomationLogsWithHttpInfo(automationId, status, limit, skip)

List automation logs

Paginated list of every comment that triggered this automation, with send status and commenter info.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CommentAutomationsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentAutomationsApi apiInstance = new CommentAutomationsApi(defaultClient);
        String automationId = "automationId_example"; // String | 
        String status = "sent"; // String | Filter by result status
        Integer limit = 50; // Integer | 
        Integer skip = 0; // Integer | 
        try {
            ApiResponse<ListCommentAutomationLogs200Response> response = apiInstance.listCommentAutomationLogsWithHttpInfo(automationId, status, limit, skip);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentAutomationsApi#listCommentAutomationLogs");
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
| **automationId** | **String**|  | |
| **status** | **String**| Filter by result status | [optional] [enum: sent, failed, skipped] |
| **limit** | **Integer**|  | [optional] [default to 50] |
| **skip** | **Integer**|  | [optional] [default to 0] |

### Return type

ApiResponse<[**ListCommentAutomationLogs200Response**](ListCommentAutomationLogs200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Trigger logs with pagination |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## listCommentAutomations

> ListCommentAutomations200Response listCommentAutomations(profileId)

List comment-to-DM automations

List all comment-to-DM automations for a profile. Returns automations with their stats.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CommentAutomationsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentAutomationsApi apiInstance = new CommentAutomationsApi(defaultClient);
        String profileId = "profileId_example"; // String | Filter by profile. Omit to list across all profiles
        try {
            ListCommentAutomations200Response result = apiInstance.listCommentAutomations(profileId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentAutomationsApi#listCommentAutomations");
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
| **profileId** | **String**| Filter by profile. Omit to list across all profiles | [optional] |

### Return type

[**ListCommentAutomations200Response**](ListCommentAutomations200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Automations list |  -  |
| **401** | Unauthorized |  -  |

## listCommentAutomationsWithHttpInfo

> ApiResponse<ListCommentAutomations200Response> listCommentAutomations listCommentAutomationsWithHttpInfo(profileId)

List comment-to-DM automations

List all comment-to-DM automations for a profile. Returns automations with their stats.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CommentAutomationsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentAutomationsApi apiInstance = new CommentAutomationsApi(defaultClient);
        String profileId = "profileId_example"; // String | Filter by profile. Omit to list across all profiles
        try {
            ApiResponse<ListCommentAutomations200Response> response = apiInstance.listCommentAutomationsWithHttpInfo(profileId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentAutomationsApi#listCommentAutomations");
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
| **profileId** | **String**| Filter by profile. Omit to list across all profiles | [optional] |

### Return type

ApiResponse<[**ListCommentAutomations200Response**](ListCommentAutomations200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Automations list |  -  |
| **401** | Unauthorized |  -  |


## updateCommentAutomation

> UpdateCommentAutomation200Response updateCommentAutomation(automationId, updateCommentAutomationRequest)

Update automation settings

Update an automation&#39;s keywords, DM message, comment reply, or active status.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CommentAutomationsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentAutomationsApi apiInstance = new CommentAutomationsApi(defaultClient);
        String automationId = "automationId_example"; // String | 
        UpdateCommentAutomationRequest updateCommentAutomationRequest = new UpdateCommentAutomationRequest(); // UpdateCommentAutomationRequest | 
        try {
            UpdateCommentAutomation200Response result = apiInstance.updateCommentAutomation(automationId, updateCommentAutomationRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentAutomationsApi#updateCommentAutomation");
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
| **automationId** | **String**|  | |
| **updateCommentAutomationRequest** | [**UpdateCommentAutomationRequest**](UpdateCommentAutomationRequest.md)|  | [optional] |

### Return type

[**UpdateCommentAutomation200Response**](UpdateCommentAutomation200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Automation updated |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## updateCommentAutomationWithHttpInfo

> ApiResponse<UpdateCommentAutomation200Response> updateCommentAutomation updateCommentAutomationWithHttpInfo(automationId, updateCommentAutomationRequest)

Update automation settings

Update an automation&#39;s keywords, DM message, comment reply, or active status.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CommentAutomationsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentAutomationsApi apiInstance = new CommentAutomationsApi(defaultClient);
        String automationId = "automationId_example"; // String | 
        UpdateCommentAutomationRequest updateCommentAutomationRequest = new UpdateCommentAutomationRequest(); // UpdateCommentAutomationRequest | 
        try {
            ApiResponse<UpdateCommentAutomation200Response> response = apiInstance.updateCommentAutomationWithHttpInfo(automationId, updateCommentAutomationRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentAutomationsApi#updateCommentAutomation");
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
| **automationId** | **String**|  | |
| **updateCommentAutomationRequest** | [**UpdateCommentAutomationRequest**](UpdateCommentAutomationRequest.md)|  | [optional] |

### Return type

ApiResponse<[**UpdateCommentAutomation200Response**](UpdateCommentAutomation200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Automation updated |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

