# BroadcastsApi

All URIs are relative to *https://zernio.com/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addBroadcastRecipients**](BroadcastsApi.md#addBroadcastRecipients) | **POST** /v1/broadcasts/{broadcastId}/recipients | Add recipients to a broadcast |
| [**addBroadcastRecipientsWithHttpInfo**](BroadcastsApi.md#addBroadcastRecipientsWithHttpInfo) | **POST** /v1/broadcasts/{broadcastId}/recipients | Add recipients to a broadcast |
| [**cancelBroadcast**](BroadcastsApi.md#cancelBroadcast) | **POST** /v1/broadcasts/{broadcastId}/cancel | Cancel broadcast |
| [**cancelBroadcastWithHttpInfo**](BroadcastsApi.md#cancelBroadcastWithHttpInfo) | **POST** /v1/broadcasts/{broadcastId}/cancel | Cancel broadcast |
| [**createBroadcast**](BroadcastsApi.md#createBroadcast) | **POST** /v1/broadcasts | Create broadcast draft |
| [**createBroadcastWithHttpInfo**](BroadcastsApi.md#createBroadcastWithHttpInfo) | **POST** /v1/broadcasts | Create broadcast draft |
| [**deleteBroadcast**](BroadcastsApi.md#deleteBroadcast) | **DELETE** /v1/broadcasts/{broadcastId} | Delete broadcast |
| [**deleteBroadcastWithHttpInfo**](BroadcastsApi.md#deleteBroadcastWithHttpInfo) | **DELETE** /v1/broadcasts/{broadcastId} | Delete broadcast |
| [**getBroadcast**](BroadcastsApi.md#getBroadcast) | **GET** /v1/broadcasts/{broadcastId} | Get broadcast details |
| [**getBroadcastWithHttpInfo**](BroadcastsApi.md#getBroadcastWithHttpInfo) | **GET** /v1/broadcasts/{broadcastId} | Get broadcast details |
| [**listBroadcastRecipients**](BroadcastsApi.md#listBroadcastRecipients) | **GET** /v1/broadcasts/{broadcastId}/recipients | List broadcast recipients |
| [**listBroadcastRecipientsWithHttpInfo**](BroadcastsApi.md#listBroadcastRecipientsWithHttpInfo) | **GET** /v1/broadcasts/{broadcastId}/recipients | List broadcast recipients |
| [**listBroadcasts**](BroadcastsApi.md#listBroadcasts) | **GET** /v1/broadcasts | List broadcasts |
| [**listBroadcastsWithHttpInfo**](BroadcastsApi.md#listBroadcastsWithHttpInfo) | **GET** /v1/broadcasts | List broadcasts |
| [**scheduleBroadcast**](BroadcastsApi.md#scheduleBroadcast) | **POST** /v1/broadcasts/{broadcastId}/schedule | Schedule broadcast for later |
| [**scheduleBroadcastWithHttpInfo**](BroadcastsApi.md#scheduleBroadcastWithHttpInfo) | **POST** /v1/broadcasts/{broadcastId}/schedule | Schedule broadcast for later |
| [**sendBroadcast**](BroadcastsApi.md#sendBroadcast) | **POST** /v1/broadcasts/{broadcastId}/send | Send broadcast now |
| [**sendBroadcastWithHttpInfo**](BroadcastsApi.md#sendBroadcastWithHttpInfo) | **POST** /v1/broadcasts/{broadcastId}/send | Send broadcast now |
| [**updateBroadcast**](BroadcastsApi.md#updateBroadcast) | **PATCH** /v1/broadcasts/{broadcastId} | Update broadcast |
| [**updateBroadcastWithHttpInfo**](BroadcastsApi.md#updateBroadcastWithHttpInfo) | **PATCH** /v1/broadcasts/{broadcastId} | Update broadcast |



## addBroadcastRecipients

> AddBroadcastRecipients200Response addBroadcastRecipients(broadcastId, addBroadcastRecipientsRequest)

Add recipients to a broadcast

Add recipients by contact IDs, raw phone numbers, or from the broadcast&#39;s segment filters.

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
            AddBroadcastRecipients200Response result = apiInstance.addBroadcastRecipients(broadcastId, addBroadcastRecipientsRequest);
            System.out.println(result);
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

[**AddBroadcastRecipients200Response**](AddBroadcastRecipients200Response.md)


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

> ApiResponse<AddBroadcastRecipients200Response> addBroadcastRecipients addBroadcastRecipientsWithHttpInfo(broadcastId, addBroadcastRecipientsRequest)

Add recipients to a broadcast

Add recipients by contact IDs, raw phone numbers, or from the broadcast&#39;s segment filters.

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
            ApiResponse<AddBroadcastRecipients200Response> response = apiInstance.addBroadcastRecipientsWithHttpInfo(broadcastId, addBroadcastRecipientsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
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

ApiResponse<[**AddBroadcastRecipients200Response**](AddBroadcastRecipients200Response.md)>


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

> CancelBroadcast200Response cancelBroadcast(broadcastId)

Cancel broadcast

Cancel a scheduled or in-progress broadcast. Already-sent messages are not affected.

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
            CancelBroadcast200Response result = apiInstance.cancelBroadcast(broadcastId);
            System.out.println(result);
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

[**CancelBroadcast200Response**](CancelBroadcast200Response.md)


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

> ApiResponse<CancelBroadcast200Response> cancelBroadcast cancelBroadcastWithHttpInfo(broadcastId)

Cancel broadcast

Cancel a scheduled or in-progress broadcast. Already-sent messages are not affected.

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
            ApiResponse<CancelBroadcast200Response> response = apiInstance.cancelBroadcastWithHttpInfo(broadcastId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
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

ApiResponse<[**CancelBroadcast200Response**](CancelBroadcast200Response.md)>


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

> CreateBroadcast200Response createBroadcast(createBroadcastRequest)

Create broadcast draft

Create a broadcast in draft status. Add recipients and then send or schedule it.

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
            CreateBroadcast200Response result = apiInstance.createBroadcast(createBroadcastRequest);
            System.out.println(result);
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

[**CreateBroadcast200Response**](CreateBroadcast200Response.md)


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

> ApiResponse<CreateBroadcast200Response> createBroadcast createBroadcastWithHttpInfo(createBroadcastRequest)

Create broadcast draft

Create a broadcast in draft status. Add recipients and then send or schedule it.

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
            ApiResponse<CreateBroadcast200Response> response = apiInstance.createBroadcastWithHttpInfo(createBroadcastRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
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

ApiResponse<[**CreateBroadcast200Response**](CreateBroadcast200Response.md)>


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

Delete broadcast

Permanently delete a broadcast. Only drafts can be deleted.

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

Delete broadcast

Permanently delete a broadcast. Only drafts can be deleted.

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

> GetBroadcast200Response getBroadcast(broadcastId)

Get broadcast details

Returns a broadcast with its full configuration and delivery stats.

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
            GetBroadcast200Response result = apiInstance.getBroadcast(broadcastId);
            System.out.println(result);
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

[**GetBroadcast200Response**](GetBroadcast200Response.md)


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

> ApiResponse<GetBroadcast200Response> getBroadcast getBroadcastWithHttpInfo(broadcastId)

Get broadcast details

Returns a broadcast with its full configuration and delivery stats.

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
            ApiResponse<GetBroadcast200Response> response = apiInstance.getBroadcastWithHttpInfo(broadcastId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
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

ApiResponse<[**GetBroadcast200Response**](GetBroadcast200Response.md)>


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

> ListBroadcastRecipients200Response listBroadcastRecipients(broadcastId, status, limit, skip)

List broadcast recipients

Returns recipients for a broadcast with individual delivery status. Filter by status.

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
            ListBroadcastRecipients200Response result = apiInstance.listBroadcastRecipients(broadcastId, status, limit, skip);
            System.out.println(result);
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

[**ListBroadcastRecipients200Response**](ListBroadcastRecipients200Response.md)


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

> ApiResponse<ListBroadcastRecipients200Response> listBroadcastRecipients listBroadcastRecipientsWithHttpInfo(broadcastId, status, limit, skip)

List broadcast recipients

Returns recipients for a broadcast with individual delivery status. Filter by status.

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
            ApiResponse<ListBroadcastRecipients200Response> response = apiInstance.listBroadcastRecipientsWithHttpInfo(broadcastId, status, limit, skip);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
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

ApiResponse<[**ListBroadcastRecipients200Response**](ListBroadcastRecipients200Response.md)>


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

> ListBroadcasts200Response listBroadcasts(profileId, status, platform, limit, skip)

List broadcasts

Returns broadcasts with delivery stats. Filter by status, platform, or profile.

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
            ListBroadcasts200Response result = apiInstance.listBroadcasts(profileId, status, platform, limit, skip);
            System.out.println(result);
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

[**ListBroadcasts200Response**](ListBroadcasts200Response.md)


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

> ApiResponse<ListBroadcasts200Response> listBroadcasts listBroadcastsWithHttpInfo(profileId, status, platform, limit, skip)

List broadcasts

Returns broadcasts with delivery stats. Filter by status, platform, or profile.

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
            ApiResponse<ListBroadcasts200Response> response = apiInstance.listBroadcastsWithHttpInfo(profileId, status, platform, limit, skip);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
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

ApiResponse<[**ListBroadcasts200Response**](ListBroadcasts200Response.md)>


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

> ScheduleBroadcast200Response scheduleBroadcast(broadcastId, scheduleBroadcastRequest)

Schedule broadcast for later

Schedule a draft broadcast to be sent at a future date and time.

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
            ScheduleBroadcast200Response result = apiInstance.scheduleBroadcast(broadcastId, scheduleBroadcastRequest);
            System.out.println(result);
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

[**ScheduleBroadcast200Response**](ScheduleBroadcast200Response.md)


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

> ApiResponse<ScheduleBroadcast200Response> scheduleBroadcast scheduleBroadcastWithHttpInfo(broadcastId, scheduleBroadcastRequest)

Schedule broadcast for later

Schedule a draft broadcast to be sent at a future date and time.

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
            ApiResponse<ScheduleBroadcast200Response> response = apiInstance.scheduleBroadcastWithHttpInfo(broadcastId, scheduleBroadcastRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
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

ApiResponse<[**ScheduleBroadcast200Response**](ScheduleBroadcast200Response.md)>


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

> SendBroadcast200Response sendBroadcast(broadcastId)

Send broadcast now

Immediately start sending a draft broadcast to its recipients.

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
            SendBroadcast200Response result = apiInstance.sendBroadcast(broadcastId);
            System.out.println(result);
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

[**SendBroadcast200Response**](SendBroadcast200Response.md)


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

> ApiResponse<SendBroadcast200Response> sendBroadcast sendBroadcastWithHttpInfo(broadcastId)

Send broadcast now

Immediately start sending a draft broadcast to its recipients.

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
            ApiResponse<SendBroadcast200Response> response = apiInstance.sendBroadcastWithHttpInfo(broadcastId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
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

ApiResponse<[**SendBroadcast200Response**](SendBroadcast200Response.md)>


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

> UpdateBroadcast200Response updateBroadcast(broadcastId)

Update broadcast

Update a broadcast&#39;s name, message, template, or segment filters. Only draft broadcasts can be updated.

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
            UpdateBroadcast200Response result = apiInstance.updateBroadcast(broadcastId);
            System.out.println(result);
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

[**UpdateBroadcast200Response**](UpdateBroadcast200Response.md)


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

> ApiResponse<UpdateBroadcast200Response> updateBroadcast updateBroadcastWithHttpInfo(broadcastId)

Update broadcast

Update a broadcast&#39;s name, message, template, or segment filters. Only draft broadcasts can be updated.

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
            ApiResponse<UpdateBroadcast200Response> response = apiInstance.updateBroadcastWithHttpInfo(broadcastId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
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

ApiResponse<[**UpdateBroadcast200Response**](UpdateBroadcast200Response.md)>


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

