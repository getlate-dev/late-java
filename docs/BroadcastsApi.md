# BroadcastsApi

All URIs are relative to *https://zernio.com/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addBroadcastRecipients**](BroadcastsApi.md#addBroadcastRecipients) | **POST** /v1/broadcasts/{broadcastId}/recipients | Add recipients to a broadcast |
| [**addBroadcastRecipientsWithHttpInfo**](BroadcastsApi.md#addBroadcastRecipientsWithHttpInfo) | **POST** /v1/broadcasts/{broadcastId}/recipients | Add recipients to a broadcast |
| [**cancelBroadcast**](BroadcastsApi.md#cancelBroadcast) | **POST** /v1/broadcasts/{broadcastId}/cancel | Cancel a broadcast |
| [**cancelBroadcastWithHttpInfo**](BroadcastsApi.md#cancelBroadcastWithHttpInfo) | **POST** /v1/broadcasts/{broadcastId}/cancel | Cancel a broadcast |
| [**createBroadcast**](BroadcastsApi.md#createBroadcast) | **POST** /v1/broadcasts | Create a broadcast draft |
| [**createBroadcastWithHttpInfo**](BroadcastsApi.md#createBroadcastWithHttpInfo) | **POST** /v1/broadcasts | Create a broadcast draft |
| [**deleteBroadcast**](BroadcastsApi.md#deleteBroadcast) | **DELETE** /v1/broadcasts/{broadcastId} | Delete a broadcast (draft only) |
| [**deleteBroadcastWithHttpInfo**](BroadcastsApi.md#deleteBroadcastWithHttpInfo) | **DELETE** /v1/broadcasts/{broadcastId} | Delete a broadcast (draft only) |
| [**getBroadcast**](BroadcastsApi.md#getBroadcast) | **GET** /v1/broadcasts/{broadcastId} | Get broadcast details |
| [**getBroadcastWithHttpInfo**](BroadcastsApi.md#getBroadcastWithHttpInfo) | **GET** /v1/broadcasts/{broadcastId} | Get broadcast details |
| [**listBroadcastRecipients**](BroadcastsApi.md#listBroadcastRecipients) | **GET** /v1/broadcasts/{broadcastId}/recipients | List broadcast recipients |
| [**listBroadcastRecipientsWithHttpInfo**](BroadcastsApi.md#listBroadcastRecipientsWithHttpInfo) | **GET** /v1/broadcasts/{broadcastId}/recipients | List broadcast recipients |
| [**listBroadcasts**](BroadcastsApi.md#listBroadcasts) | **GET** /v1/broadcasts | List broadcasts |
| [**listBroadcastsWithHttpInfo**](BroadcastsApi.md#listBroadcastsWithHttpInfo) | **GET** /v1/broadcasts | List broadcasts |
| [**scheduleBroadcast**](BroadcastsApi.md#scheduleBroadcast) | **POST** /v1/broadcasts/{broadcastId}/schedule | Schedule broadcast for later |
| [**scheduleBroadcastWithHttpInfo**](BroadcastsApi.md#scheduleBroadcastWithHttpInfo) | **POST** /v1/broadcasts/{broadcastId}/schedule | Schedule broadcast for later |
| [**sendBroadcast**](BroadcastsApi.md#sendBroadcast) | **POST** /v1/broadcasts/{broadcastId}/send | Trigger immediate send |
| [**sendBroadcastWithHttpInfo**](BroadcastsApi.md#sendBroadcastWithHttpInfo) | **POST** /v1/broadcasts/{broadcastId}/send | Trigger immediate send |
| [**updateBroadcast**](BroadcastsApi.md#updateBroadcast) | **PATCH** /v1/broadcasts/{broadcastId} | Update a broadcast |
| [**updateBroadcastWithHttpInfo**](BroadcastsApi.md#updateBroadcastWithHttpInfo) | **PATCH** /v1/broadcasts/{broadcastId} | Update a broadcast |



## addBroadcastRecipients

> void addBroadcastRecipients(broadcastId, addBroadcastRecipientsRequest)

Add recipients to a broadcast

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.BroadcastsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        BroadcastsApi apiInstance = new BroadcastsApi(defaultClient);
        String broadcastId = "broadcastId_example"; // String | 
        AddBroadcastRecipientsRequest addBroadcastRecipientsRequest = new AddBroadcastRecipientsRequest(); // AddBroadcastRecipientsRequest | 
        try {
            apiInstance.addBroadcastRecipients(broadcastId, addBroadcastRecipientsRequest);
        } catch (ApiException e) {
            System.err.println("Exception when calling BroadcastsApi#addBroadcastRecipients");
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
| **broadcastId** | **String**|  | |
| **addBroadcastRecipientsRequest** | [**AddBroadcastRecipientsRequest**](AddBroadcastRecipientsRequest.md)|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Recipients added |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## addBroadcastRecipientsWithHttpInfo

> ApiResponse<Void> addBroadcastRecipients addBroadcastRecipientsWithHttpInfo(broadcastId, addBroadcastRecipientsRequest)

Add recipients to a broadcast

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.BroadcastsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        BroadcastsApi apiInstance = new BroadcastsApi(defaultClient);
        String broadcastId = "broadcastId_example"; // String | 
        AddBroadcastRecipientsRequest addBroadcastRecipientsRequest = new AddBroadcastRecipientsRequest(); // AddBroadcastRecipientsRequest | 
        try {
            ApiResponse<Void> response = apiInstance.addBroadcastRecipientsWithHttpInfo(broadcastId, addBroadcastRecipientsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling BroadcastsApi#addBroadcastRecipients");
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
| **broadcastId** | **String**|  | |
| **addBroadcastRecipientsRequest** | [**AddBroadcastRecipientsRequest**](AddBroadcastRecipientsRequest.md)|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Recipients added |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## cancelBroadcast

> void cancelBroadcast(broadcastId)

Cancel a broadcast

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.BroadcastsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        BroadcastsApi apiInstance = new BroadcastsApi(defaultClient);
        String broadcastId = "broadcastId_example"; // String | 
        try {
            apiInstance.cancelBroadcast(broadcastId);
        } catch (ApiException e) {
            System.err.println("Exception when calling BroadcastsApi#cancelBroadcast");
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
| **broadcastId** | **String**|  | |

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
| **200** | Broadcast cancelled |  -  |
| **400** | Cannot cancel in current status |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## cancelBroadcastWithHttpInfo

> ApiResponse<Void> cancelBroadcast cancelBroadcastWithHttpInfo(broadcastId)

Cancel a broadcast

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.BroadcastsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        BroadcastsApi apiInstance = new BroadcastsApi(defaultClient);
        String broadcastId = "broadcastId_example"; // String | 
        try {
            ApiResponse<Void> response = apiInstance.cancelBroadcastWithHttpInfo(broadcastId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling BroadcastsApi#cancelBroadcast");
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
| **broadcastId** | **String**|  | |

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
| **200** | Broadcast cancelled |  -  |
| **400** | Cannot cancel in current status |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## createBroadcast

> void createBroadcast(createBroadcastRequest)

Create a broadcast draft

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.BroadcastsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        BroadcastsApi apiInstance = new BroadcastsApi(defaultClient);
        CreateBroadcastRequest createBroadcastRequest = new CreateBroadcastRequest(); // CreateBroadcastRequest | 
        try {
            apiInstance.createBroadcast(createBroadcastRequest);
        } catch (ApiException e) {
            System.err.println("Exception when calling BroadcastsApi#createBroadcast");
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
| **createBroadcastRequest** | [**CreateBroadcastRequest**](CreateBroadcastRequest.md)|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Broadcast created |  -  |
| **401** | Unauthorized |  -  |

## createBroadcastWithHttpInfo

> ApiResponse<Void> createBroadcast createBroadcastWithHttpInfo(createBroadcastRequest)

Create a broadcast draft

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.BroadcastsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        BroadcastsApi apiInstance = new BroadcastsApi(defaultClient);
        CreateBroadcastRequest createBroadcastRequest = new CreateBroadcastRequest(); // CreateBroadcastRequest | 
        try {
            ApiResponse<Void> response = apiInstance.createBroadcastWithHttpInfo(createBroadcastRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling BroadcastsApi#createBroadcast");
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
| **createBroadcastRequest** | [**CreateBroadcastRequest**](CreateBroadcastRequest.md)|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Broadcast created |  -  |
| **401** | Unauthorized |  -  |


## deleteBroadcast

> void deleteBroadcast(broadcastId)

Delete a broadcast (draft only)

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.BroadcastsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        BroadcastsApi apiInstance = new BroadcastsApi(defaultClient);
        String broadcastId = "broadcastId_example"; // String | 
        try {
            apiInstance.deleteBroadcast(broadcastId);
        } catch (ApiException e) {
            System.err.println("Exception when calling BroadcastsApi#deleteBroadcast");
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
| **broadcastId** | **String**|  | |

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
| **200** | Broadcast deleted |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## deleteBroadcastWithHttpInfo

> ApiResponse<Void> deleteBroadcast deleteBroadcastWithHttpInfo(broadcastId)

Delete a broadcast (draft only)

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.BroadcastsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        BroadcastsApi apiInstance = new BroadcastsApi(defaultClient);
        String broadcastId = "broadcastId_example"; // String | 
        try {
            ApiResponse<Void> response = apiInstance.deleteBroadcastWithHttpInfo(broadcastId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling BroadcastsApi#deleteBroadcast");
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
| **broadcastId** | **String**|  | |

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
| **200** | Broadcast deleted |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## getBroadcast

> void getBroadcast(broadcastId)

Get broadcast details

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.BroadcastsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        BroadcastsApi apiInstance = new BroadcastsApi(defaultClient);
        String broadcastId = "broadcastId_example"; // String | 
        try {
            apiInstance.getBroadcast(broadcastId);
        } catch (ApiException e) {
            System.err.println("Exception when calling BroadcastsApi#getBroadcast");
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
| **broadcastId** | **String**|  | |

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
| **200** | Broadcast details with stats |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## getBroadcastWithHttpInfo

> ApiResponse<Void> getBroadcast getBroadcastWithHttpInfo(broadcastId)

Get broadcast details

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.BroadcastsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        BroadcastsApi apiInstance = new BroadcastsApi(defaultClient);
        String broadcastId = "broadcastId_example"; // String | 
        try {
            ApiResponse<Void> response = apiInstance.getBroadcastWithHttpInfo(broadcastId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling BroadcastsApi#getBroadcast");
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
| **broadcastId** | **String**|  | |

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
| **200** | Broadcast details with stats |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## listBroadcastRecipients

> void listBroadcastRecipients(broadcastId, status, limit, skip)

List broadcast recipients

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.BroadcastsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        BroadcastsApi apiInstance = new BroadcastsApi(defaultClient);
        String broadcastId = "broadcastId_example"; // String | 
        String status = "pending"; // String | 
        Integer limit = 50; // Integer | 
        Integer skip = 0; // Integer | 
        try {
            apiInstance.listBroadcastRecipients(broadcastId, status, limit, skip);
        } catch (ApiException e) {
            System.err.println("Exception when calling BroadcastsApi#listBroadcastRecipients");
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
| **broadcastId** | **String**|  | |
| **status** | **String**|  | [optional] [enum: pending, sent, delivered, read, failed] |
| **limit** | **Integer**|  | [optional] [default to 50] |
| **skip** | **Integer**|  | [optional] [default to 0] |

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
| **200** | Recipients list with delivery status |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## listBroadcastRecipientsWithHttpInfo

> ApiResponse<Void> listBroadcastRecipients listBroadcastRecipientsWithHttpInfo(broadcastId, status, limit, skip)

List broadcast recipients

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.BroadcastsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        BroadcastsApi apiInstance = new BroadcastsApi(defaultClient);
        String broadcastId = "broadcastId_example"; // String | 
        String status = "pending"; // String | 
        Integer limit = 50; // Integer | 
        Integer skip = 0; // Integer | 
        try {
            ApiResponse<Void> response = apiInstance.listBroadcastRecipientsWithHttpInfo(broadcastId, status, limit, skip);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling BroadcastsApi#listBroadcastRecipients");
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
| **broadcastId** | **String**|  | |
| **status** | **String**|  | [optional] [enum: pending, sent, delivered, read, failed] |
| **limit** | **Integer**|  | [optional] [default to 50] |
| **skip** | **Integer**|  | [optional] [default to 0] |

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
| **200** | Recipients list with delivery status |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## listBroadcasts

> void listBroadcasts(profileId, status, platform, limit, skip)

List broadcasts

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.BroadcastsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        BroadcastsApi apiInstance = new BroadcastsApi(defaultClient);
        String profileId = "profileId_example"; // String | Filter by profile. Omit to list across all profiles
        String status = "draft"; // String | 
        String platform = "platform_example"; // String | 
        Integer limit = 50; // Integer | 
        Integer skip = 0; // Integer | 
        try {
            apiInstance.listBroadcasts(profileId, status, platform, limit, skip);
        } catch (ApiException e) {
            System.err.println("Exception when calling BroadcastsApi#listBroadcasts");
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
| **status** | **String**|  | [optional] [enum: draft, scheduled, sending, completed, failed, cancelled] |
| **platform** | **String**|  | [optional] |
| **limit** | **Integer**|  | [optional] [default to 50] |
| **skip** | **Integer**|  | [optional] [default to 0] |

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
| **200** | Broadcasts list |  -  |
| **401** | Unauthorized |  -  |

## listBroadcastsWithHttpInfo

> ApiResponse<Void> listBroadcasts listBroadcastsWithHttpInfo(profileId, status, platform, limit, skip)

List broadcasts

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.BroadcastsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        BroadcastsApi apiInstance = new BroadcastsApi(defaultClient);
        String profileId = "profileId_example"; // String | Filter by profile. Omit to list across all profiles
        String status = "draft"; // String | 
        String platform = "platform_example"; // String | 
        Integer limit = 50; // Integer | 
        Integer skip = 0; // Integer | 
        try {
            ApiResponse<Void> response = apiInstance.listBroadcastsWithHttpInfo(profileId, status, platform, limit, skip);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling BroadcastsApi#listBroadcasts");
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
| **status** | **String**|  | [optional] [enum: draft, scheduled, sending, completed, failed, cancelled] |
| **platform** | **String**|  | [optional] |
| **limit** | **Integer**|  | [optional] [default to 50] |
| **skip** | **Integer**|  | [optional] [default to 0] |

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
| **200** | Broadcasts list |  -  |
| **401** | Unauthorized |  -  |


## scheduleBroadcast

> void scheduleBroadcast(broadcastId, scheduleBroadcastRequest)

Schedule broadcast for later

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.BroadcastsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        BroadcastsApi apiInstance = new BroadcastsApi(defaultClient);
        String broadcastId = "broadcastId_example"; // String | 
        ScheduleBroadcastRequest scheduleBroadcastRequest = new ScheduleBroadcastRequest(); // ScheduleBroadcastRequest | 
        try {
            apiInstance.scheduleBroadcast(broadcastId, scheduleBroadcastRequest);
        } catch (ApiException e) {
            System.err.println("Exception when calling BroadcastsApi#scheduleBroadcast");
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
| **broadcastId** | **String**|  | |
| **scheduleBroadcastRequest** | [**ScheduleBroadcastRequest**](ScheduleBroadcastRequest.md)|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Broadcast scheduled |  -  |
| **400** | Invalid date or status |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## scheduleBroadcastWithHttpInfo

> ApiResponse<Void> scheduleBroadcast scheduleBroadcastWithHttpInfo(broadcastId, scheduleBroadcastRequest)

Schedule broadcast for later

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.BroadcastsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        BroadcastsApi apiInstance = new BroadcastsApi(defaultClient);
        String broadcastId = "broadcastId_example"; // String | 
        ScheduleBroadcastRequest scheduleBroadcastRequest = new ScheduleBroadcastRequest(); // ScheduleBroadcastRequest | 
        try {
            ApiResponse<Void> response = apiInstance.scheduleBroadcastWithHttpInfo(broadcastId, scheduleBroadcastRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling BroadcastsApi#scheduleBroadcast");
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
| **broadcastId** | **String**|  | |
| **scheduleBroadcastRequest** | [**ScheduleBroadcastRequest**](ScheduleBroadcastRequest.md)|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Broadcast scheduled |  -  |
| **400** | Invalid date or status |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## sendBroadcast

> void sendBroadcast(broadcastId)

Trigger immediate send

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.BroadcastsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        BroadcastsApi apiInstance = new BroadcastsApi(defaultClient);
        String broadcastId = "broadcastId_example"; // String | 
        try {
            apiInstance.sendBroadcast(broadcastId);
        } catch (ApiException e) {
            System.err.println("Exception when calling BroadcastsApi#sendBroadcast");
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
| **broadcastId** | **String**|  | |

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
| **200** | Broadcast sending started |  -  |
| **400** | Invalid status or no recipients |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## sendBroadcastWithHttpInfo

> ApiResponse<Void> sendBroadcast sendBroadcastWithHttpInfo(broadcastId)

Trigger immediate send

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.BroadcastsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        BroadcastsApi apiInstance = new BroadcastsApi(defaultClient);
        String broadcastId = "broadcastId_example"; // String | 
        try {
            ApiResponse<Void> response = apiInstance.sendBroadcastWithHttpInfo(broadcastId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling BroadcastsApi#sendBroadcast");
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
| **broadcastId** | **String**|  | |

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
| **200** | Broadcast sending started |  -  |
| **400** | Invalid status or no recipients |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## updateBroadcast

> void updateBroadcast(broadcastId)

Update a broadcast

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.BroadcastsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        BroadcastsApi apiInstance = new BroadcastsApi(defaultClient);
        String broadcastId = "broadcastId_example"; // String | 
        try {
            apiInstance.updateBroadcast(broadcastId);
        } catch (ApiException e) {
            System.err.println("Exception when calling BroadcastsApi#updateBroadcast");
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
| **broadcastId** | **String**|  | |

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
| **200** | Broadcast updated |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## updateBroadcastWithHttpInfo

> ApiResponse<Void> updateBroadcast updateBroadcastWithHttpInfo(broadcastId)

Update a broadcast

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.BroadcastsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        BroadcastsApi apiInstance = new BroadcastsApi(defaultClient);
        String broadcastId = "broadcastId_example"; // String | 
        try {
            ApiResponse<Void> response = apiInstance.updateBroadcastWithHttpInfo(broadcastId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling BroadcastsApi#updateBroadcast");
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
| **broadcastId** | **String**|  | |

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
| **200** | Broadcast updated |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

