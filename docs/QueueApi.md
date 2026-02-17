# QueueApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createQueueSlot**](QueueApi.md#createQueueSlot) | **POST** /v1/queue/slots | Create schedule |
| [**createQueueSlotWithHttpInfo**](QueueApi.md#createQueueSlotWithHttpInfo) | **POST** /v1/queue/slots | Create schedule |
| [**deleteQueueSlot**](QueueApi.md#deleteQueueSlot) | **DELETE** /v1/queue/slots | Delete schedule |
| [**deleteQueueSlotWithHttpInfo**](QueueApi.md#deleteQueueSlotWithHttpInfo) | **DELETE** /v1/queue/slots | Delete schedule |
| [**getNextQueueSlot**](QueueApi.md#getNextQueueSlot) | **GET** /v1/queue/next-slot | Get next available slot |
| [**getNextQueueSlotWithHttpInfo**](QueueApi.md#getNextQueueSlotWithHttpInfo) | **GET** /v1/queue/next-slot | Get next available slot |
| [**listQueueSlots**](QueueApi.md#listQueueSlots) | **GET** /v1/queue/slots | List schedules |
| [**listQueueSlotsWithHttpInfo**](QueueApi.md#listQueueSlotsWithHttpInfo) | **GET** /v1/queue/slots | List schedules |
| [**previewQueue**](QueueApi.md#previewQueue) | **GET** /v1/queue/preview | Preview upcoming slots |
| [**previewQueueWithHttpInfo**](QueueApi.md#previewQueueWithHttpInfo) | **GET** /v1/queue/preview | Preview upcoming slots |
| [**updateQueueSlot**](QueueApi.md#updateQueueSlot) | **PUT** /v1/queue/slots | Update schedule |
| [**updateQueueSlotWithHttpInfo**](QueueApi.md#updateQueueSlotWithHttpInfo) | **PUT** /v1/queue/slots | Update schedule |



## createQueueSlot

> CreateQueueSlot201Response createQueueSlot(createQueueSlotRequest)

Create schedule

Create an additional queue for a profile. The first queue created becomes the default. Subsequent queues are non-default unless explicitly set. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.QueueApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        QueueApi apiInstance = new QueueApi(defaultClient);
        CreateQueueSlotRequest createQueueSlotRequest = new CreateQueueSlotRequest(); // CreateQueueSlotRequest | 
        try {
            CreateQueueSlot201Response result = apiInstance.createQueueSlot(createQueueSlotRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling QueueApi#createQueueSlot");
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
| **createQueueSlotRequest** | [**CreateQueueSlotRequest**](CreateQueueSlotRequest.md)|  | |

### Return type

[**CreateQueueSlot201Response**](CreateQueueSlot201Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Queue created |  -  |
| **400** | Invalid request or validation error |  -  |
| **401** | Unauthorized |  -  |
| **404** | Profile not found |  -  |

## createQueueSlotWithHttpInfo

> ApiResponse<CreateQueueSlot201Response> createQueueSlot createQueueSlotWithHttpInfo(createQueueSlotRequest)

Create schedule

Create an additional queue for a profile. The first queue created becomes the default. Subsequent queues are non-default unless explicitly set. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.QueueApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        QueueApi apiInstance = new QueueApi(defaultClient);
        CreateQueueSlotRequest createQueueSlotRequest = new CreateQueueSlotRequest(); // CreateQueueSlotRequest | 
        try {
            ApiResponse<CreateQueueSlot201Response> response = apiInstance.createQueueSlotWithHttpInfo(createQueueSlotRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling QueueApi#createQueueSlot");
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
| **createQueueSlotRequest** | [**CreateQueueSlotRequest**](CreateQueueSlotRequest.md)|  | |

### Return type

ApiResponse<[**CreateQueueSlot201Response**](CreateQueueSlot201Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Queue created |  -  |
| **400** | Invalid request or validation error |  -  |
| **401** | Unauthorized |  -  |
| **404** | Profile not found |  -  |


## deleteQueueSlot

> DeleteQueueSlot200Response deleteQueueSlot(profileId, queueId)

Delete schedule

Delete a queue from a profile. Requires queueId to specify which queue to delete. If deleting the default queue, another queue will be promoted to default. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.QueueApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        QueueApi apiInstance = new QueueApi(defaultClient);
        String profileId = "profileId_example"; // String | 
        String queueId = "queueId_example"; // String | Queue ID to delete
        try {
            DeleteQueueSlot200Response result = apiInstance.deleteQueueSlot(profileId, queueId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling QueueApi#deleteQueueSlot");
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
| **profileId** | **String**|  | |
| **queueId** | **String**| Queue ID to delete | |

### Return type

[**DeleteQueueSlot200Response**](DeleteQueueSlot200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Queue schedule deleted |  -  |
| **400** | Missing profileId or queueId |  -  |
| **401** | Unauthorized |  -  |

## deleteQueueSlotWithHttpInfo

> ApiResponse<DeleteQueueSlot200Response> deleteQueueSlot deleteQueueSlotWithHttpInfo(profileId, queueId)

Delete schedule

Delete a queue from a profile. Requires queueId to specify which queue to delete. If deleting the default queue, another queue will be promoted to default. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.QueueApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        QueueApi apiInstance = new QueueApi(defaultClient);
        String profileId = "profileId_example"; // String | 
        String queueId = "queueId_example"; // String | Queue ID to delete
        try {
            ApiResponse<DeleteQueueSlot200Response> response = apiInstance.deleteQueueSlotWithHttpInfo(profileId, queueId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling QueueApi#deleteQueueSlot");
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
| **profileId** | **String**|  | |
| **queueId** | **String**| Queue ID to delete | |

### Return type

ApiResponse<[**DeleteQueueSlot200Response**](DeleteQueueSlot200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Queue schedule deleted |  -  |
| **400** | Missing profileId or queueId |  -  |
| **401** | Unauthorized |  -  |


## getNextQueueSlot

> GetNextQueueSlot200Response getNextQueueSlot(profileId, queueId)

Get next available slot

Returns the next available queue slot for preview/informational purposes. Do NOT use this response with scheduledFor to schedule a post, as that creates a manual post, not a queue post. Instead, use POST /v1/posts with queuedFromProfile (and optionally queueId). Useful for showing users when their next post will go out, debugging queue configuration, or building UI previews.  If no queueId is specified, uses the profile&#39;s default queue. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.QueueApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        QueueApi apiInstance = new QueueApi(defaultClient);
        String profileId = "profileId_example"; // String | 
        String queueId = "queueId_example"; // String | Specific queue ID (optional, defaults to profile's default queue)
        try {
            GetNextQueueSlot200Response result = apiInstance.getNextQueueSlot(profileId, queueId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling QueueApi#getNextQueueSlot");
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
| **profileId** | **String**|  | |
| **queueId** | **String**| Specific queue ID (optional, defaults to profile&#39;s default queue) | [optional] |

### Return type

[**GetNextQueueSlot200Response**](GetNextQueueSlot200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Next available slot |  -  |
| **400** | Invalid parameters or inactive queue |  -  |
| **401** | Unauthorized |  -  |
| **404** | Profile or queue schedule not found, or no available slots |  -  |

## getNextQueueSlotWithHttpInfo

> ApiResponse<GetNextQueueSlot200Response> getNextQueueSlot getNextQueueSlotWithHttpInfo(profileId, queueId)

Get next available slot

Returns the next available queue slot for preview/informational purposes. Do NOT use this response with scheduledFor to schedule a post, as that creates a manual post, not a queue post. Instead, use POST /v1/posts with queuedFromProfile (and optionally queueId). Useful for showing users when their next post will go out, debugging queue configuration, or building UI previews.  If no queueId is specified, uses the profile&#39;s default queue. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.QueueApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        QueueApi apiInstance = new QueueApi(defaultClient);
        String profileId = "profileId_example"; // String | 
        String queueId = "queueId_example"; // String | Specific queue ID (optional, defaults to profile's default queue)
        try {
            ApiResponse<GetNextQueueSlot200Response> response = apiInstance.getNextQueueSlotWithHttpInfo(profileId, queueId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling QueueApi#getNextQueueSlot");
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
| **profileId** | **String**|  | |
| **queueId** | **String**| Specific queue ID (optional, defaults to profile&#39;s default queue) | [optional] |

### Return type

ApiResponse<[**GetNextQueueSlot200Response**](GetNextQueueSlot200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Next available slot |  -  |
| **400** | Invalid parameters or inactive queue |  -  |
| **401** | Unauthorized |  -  |
| **404** | Profile or queue schedule not found, or no available slots |  -  |


## listQueueSlots

> ListQueueSlots200Response listQueueSlots(profileId, queueId, all)

List schedules

Retrieve queue schedules for a profile. Each profile can have multiple queues. Without all&#x3D;true, returns the default queue (or specific queue if queueId provided). With all&#x3D;true, returns all queues for the profile. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.QueueApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        QueueApi apiInstance = new QueueApi(defaultClient);
        String profileId = "profileId_example"; // String | Profile ID to get queues for
        String queueId = "queueId_example"; // String | Specific queue ID to retrieve (optional)
        String all = "true"; // String | Set to 'true' to list all queues for the profile
        try {
            ListQueueSlots200Response result = apiInstance.listQueueSlots(profileId, queueId, all);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling QueueApi#listQueueSlots");
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
| **profileId** | **String**| Profile ID to get queues for | |
| **queueId** | **String**| Specific queue ID to retrieve (optional) | [optional] |
| **all** | **String**| Set to &#39;true&#39; to list all queues for the profile | [optional] [enum: true] |

### Return type

[**ListQueueSlots200Response**](ListQueueSlots200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Queue schedule(s) retrieved |  -  |
| **400** | Missing profileId |  -  |
| **401** | Unauthorized |  -  |
| **404** | Profile not found |  -  |

## listQueueSlotsWithHttpInfo

> ApiResponse<ListQueueSlots200Response> listQueueSlots listQueueSlotsWithHttpInfo(profileId, queueId, all)

List schedules

Retrieve queue schedules for a profile. Each profile can have multiple queues. Without all&#x3D;true, returns the default queue (or specific queue if queueId provided). With all&#x3D;true, returns all queues for the profile. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.QueueApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        QueueApi apiInstance = new QueueApi(defaultClient);
        String profileId = "profileId_example"; // String | Profile ID to get queues for
        String queueId = "queueId_example"; // String | Specific queue ID to retrieve (optional)
        String all = "true"; // String | Set to 'true' to list all queues for the profile
        try {
            ApiResponse<ListQueueSlots200Response> response = apiInstance.listQueueSlotsWithHttpInfo(profileId, queueId, all);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling QueueApi#listQueueSlots");
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
| **profileId** | **String**| Profile ID to get queues for | |
| **queueId** | **String**| Specific queue ID to retrieve (optional) | [optional] |
| **all** | **String**| Set to &#39;true&#39; to list all queues for the profile | [optional] [enum: true] |

### Return type

ApiResponse<[**ListQueueSlots200Response**](ListQueueSlots200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Queue schedule(s) retrieved |  -  |
| **400** | Missing profileId |  -  |
| **401** | Unauthorized |  -  |
| **404** | Profile not found |  -  |


## previewQueue

> PreviewQueue200Response previewQueue(profileId, count)

Preview upcoming slots

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.QueueApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        QueueApi apiInstance = new QueueApi(defaultClient);
        String profileId = "profileId_example"; // String | 
        Integer count = 20; // Integer | 
        try {
            PreviewQueue200Response result = apiInstance.previewQueue(profileId, count);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling QueueApi#previewQueue");
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
| **profileId** | **String**|  | |
| **count** | **Integer**|  | [optional] [default to 20] |

### Return type

[**PreviewQueue200Response**](PreviewQueue200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Queue slots preview |  -  |
| **400** | Invalid parameters |  -  |
| **401** | Unauthorized |  -  |
| **404** | Profile or queue schedule not found |  -  |

## previewQueueWithHttpInfo

> ApiResponse<PreviewQueue200Response> previewQueue previewQueueWithHttpInfo(profileId, count)

Preview upcoming slots

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.QueueApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        QueueApi apiInstance = new QueueApi(defaultClient);
        String profileId = "profileId_example"; // String | 
        Integer count = 20; // Integer | 
        try {
            ApiResponse<PreviewQueue200Response> response = apiInstance.previewQueueWithHttpInfo(profileId, count);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling QueueApi#previewQueue");
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
| **profileId** | **String**|  | |
| **count** | **Integer**|  | [optional] [default to 20] |

### Return type

ApiResponse<[**PreviewQueue200Response**](PreviewQueue200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Queue slots preview |  -  |
| **400** | Invalid parameters |  -  |
| **401** | Unauthorized |  -  |
| **404** | Profile or queue schedule not found |  -  |


## updateQueueSlot

> UpdateQueueSlot200Response updateQueueSlot(updateQueueSlotRequest)

Update schedule

Create a new queue or update an existing one. Without queueId, creates/updates the default queue. With queueId, updates a specific queue. With setAsDefault&#x3D;true, makes this queue the default for the profile. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.QueueApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        QueueApi apiInstance = new QueueApi(defaultClient);
        UpdateQueueSlotRequest updateQueueSlotRequest = new UpdateQueueSlotRequest(); // UpdateQueueSlotRequest | 
        try {
            UpdateQueueSlot200Response result = apiInstance.updateQueueSlot(updateQueueSlotRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling QueueApi#updateQueueSlot");
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
| **updateQueueSlotRequest** | [**UpdateQueueSlotRequest**](UpdateQueueSlotRequest.md)|  | |

### Return type

[**UpdateQueueSlot200Response**](UpdateQueueSlot200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Queue schedule updated |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |
| **404** | Profile not found |  -  |

## updateQueueSlotWithHttpInfo

> ApiResponse<UpdateQueueSlot200Response> updateQueueSlot updateQueueSlotWithHttpInfo(updateQueueSlotRequest)

Update schedule

Create a new queue or update an existing one. Without queueId, creates/updates the default queue. With queueId, updates a specific queue. With setAsDefault&#x3D;true, makes this queue the default for the profile. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.QueueApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        QueueApi apiInstance = new QueueApi(defaultClient);
        UpdateQueueSlotRequest updateQueueSlotRequest = new UpdateQueueSlotRequest(); // UpdateQueueSlotRequest | 
        try {
            ApiResponse<UpdateQueueSlot200Response> response = apiInstance.updateQueueSlotWithHttpInfo(updateQueueSlotRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling QueueApi#updateQueueSlot");
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
| **updateQueueSlotRequest** | [**UpdateQueueSlotRequest**](UpdateQueueSlotRequest.md)|  | |

### Return type

ApiResponse<[**UpdateQueueSlot200Response**](UpdateQueueSlot200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Queue schedule updated |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |
| **404** | Profile not found |  -  |

