# SequencesApi

All URIs are relative to *https://zernio.com/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**activateSequence**](SequencesApi.md#activateSequence) | **POST** /v1/sequences/{sequenceId}/activate | Activate a sequence |
| [**activateSequenceWithHttpInfo**](SequencesApi.md#activateSequenceWithHttpInfo) | **POST** /v1/sequences/{sequenceId}/activate | Activate a sequence |
| [**createSequence**](SequencesApi.md#createSequence) | **POST** /v1/sequences | Create a sequence |
| [**createSequenceWithHttpInfo**](SequencesApi.md#createSequenceWithHttpInfo) | **POST** /v1/sequences | Create a sequence |
| [**deleteSequence**](SequencesApi.md#deleteSequence) | **DELETE** /v1/sequences/{sequenceId} | Delete a sequence |
| [**deleteSequenceWithHttpInfo**](SequencesApi.md#deleteSequenceWithHttpInfo) | **DELETE** /v1/sequences/{sequenceId} | Delete a sequence |
| [**enrollContacts**](SequencesApi.md#enrollContacts) | **POST** /v1/sequences/{sequenceId}/enroll | Enroll contacts in a sequence |
| [**enrollContactsWithHttpInfo**](SequencesApi.md#enrollContactsWithHttpInfo) | **POST** /v1/sequences/{sequenceId}/enroll | Enroll contacts in a sequence |
| [**getSequence**](SequencesApi.md#getSequence) | **GET** /v1/sequences/{sequenceId} | Get sequence with steps |
| [**getSequenceWithHttpInfo**](SequencesApi.md#getSequenceWithHttpInfo) | **GET** /v1/sequences/{sequenceId} | Get sequence with steps |
| [**listSequenceEnrollments**](SequencesApi.md#listSequenceEnrollments) | **GET** /v1/sequences/{sequenceId}/enrollments | List enrollments for a sequence |
| [**listSequenceEnrollmentsWithHttpInfo**](SequencesApi.md#listSequenceEnrollmentsWithHttpInfo) | **GET** /v1/sequences/{sequenceId}/enrollments | List enrollments for a sequence |
| [**listSequences**](SequencesApi.md#listSequences) | **GET** /v1/sequences | List sequences |
| [**listSequencesWithHttpInfo**](SequencesApi.md#listSequencesWithHttpInfo) | **GET** /v1/sequences | List sequences |
| [**pauseSequence**](SequencesApi.md#pauseSequence) | **POST** /v1/sequences/{sequenceId}/pause | Pause a sequence |
| [**pauseSequenceWithHttpInfo**](SequencesApi.md#pauseSequenceWithHttpInfo) | **POST** /v1/sequences/{sequenceId}/pause | Pause a sequence |
| [**unenrollContact**](SequencesApi.md#unenrollContact) | **DELETE** /v1/sequences/{sequenceId}/enroll/{contactId} | Unenroll a contact from a sequence |
| [**unenrollContactWithHttpInfo**](SequencesApi.md#unenrollContactWithHttpInfo) | **DELETE** /v1/sequences/{sequenceId}/enroll/{contactId} | Unenroll a contact from a sequence |
| [**updateSequence**](SequencesApi.md#updateSequence) | **PATCH** /v1/sequences/{sequenceId} | Update a sequence |
| [**updateSequenceWithHttpInfo**](SequencesApi.md#updateSequenceWithHttpInfo) | **PATCH** /v1/sequences/{sequenceId} | Update a sequence |



## activateSequence

> void activateSequence(sequenceId)

Activate a sequence

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.SequencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        SequencesApi apiInstance = new SequencesApi(defaultClient);
        String sequenceId = "sequenceId_example"; // String | 
        try {
            apiInstance.activateSequence(sequenceId);
        } catch (ApiException e) {
            System.err.println("Exception when calling SequencesApi#activateSequence");
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
| **sequenceId** | **String**|  | |

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
| **200** | Sequence activated |  -  |
| **400** | Invalid status or no steps |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## activateSequenceWithHttpInfo

> ApiResponse<Void> activateSequence activateSequenceWithHttpInfo(sequenceId)

Activate a sequence

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.SequencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        SequencesApi apiInstance = new SequencesApi(defaultClient);
        String sequenceId = "sequenceId_example"; // String | 
        try {
            ApiResponse<Void> response = apiInstance.activateSequenceWithHttpInfo(sequenceId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling SequencesApi#activateSequence");
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
| **sequenceId** | **String**|  | |

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
| **200** | Sequence activated |  -  |
| **400** | Invalid status or no steps |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## createSequence

> void createSequence(createSequenceRequest)

Create a sequence

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.SequencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        SequencesApi apiInstance = new SequencesApi(defaultClient);
        CreateSequenceRequest createSequenceRequest = new CreateSequenceRequest(); // CreateSequenceRequest | 
        try {
            apiInstance.createSequence(createSequenceRequest);
        } catch (ApiException e) {
            System.err.println("Exception when calling SequencesApi#createSequence");
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
| **createSequenceRequest** | [**CreateSequenceRequest**](CreateSequenceRequest.md)|  | |

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
| **200** | Sequence created |  -  |
| **401** | Unauthorized |  -  |

## createSequenceWithHttpInfo

> ApiResponse<Void> createSequence createSequenceWithHttpInfo(createSequenceRequest)

Create a sequence

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.SequencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        SequencesApi apiInstance = new SequencesApi(defaultClient);
        CreateSequenceRequest createSequenceRequest = new CreateSequenceRequest(); // CreateSequenceRequest | 
        try {
            ApiResponse<Void> response = apiInstance.createSequenceWithHttpInfo(createSequenceRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling SequencesApi#createSequence");
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
| **createSequenceRequest** | [**CreateSequenceRequest**](CreateSequenceRequest.md)|  | |

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
| **200** | Sequence created |  -  |
| **401** | Unauthorized |  -  |


## deleteSequence

> void deleteSequence(sequenceId)

Delete a sequence

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.SequencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        SequencesApi apiInstance = new SequencesApi(defaultClient);
        String sequenceId = "sequenceId_example"; // String | 
        try {
            apiInstance.deleteSequence(sequenceId);
        } catch (ApiException e) {
            System.err.println("Exception when calling SequencesApi#deleteSequence");
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
| **sequenceId** | **String**|  | |

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
| **200** | Sequence deleted |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## deleteSequenceWithHttpInfo

> ApiResponse<Void> deleteSequence deleteSequenceWithHttpInfo(sequenceId)

Delete a sequence

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.SequencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        SequencesApi apiInstance = new SequencesApi(defaultClient);
        String sequenceId = "sequenceId_example"; // String | 
        try {
            ApiResponse<Void> response = apiInstance.deleteSequenceWithHttpInfo(sequenceId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling SequencesApi#deleteSequence");
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
| **sequenceId** | **String**|  | |

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
| **200** | Sequence deleted |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## enrollContacts

> void enrollContacts(sequenceId, enrollContactsRequest)

Enroll contacts in a sequence

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.SequencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        SequencesApi apiInstance = new SequencesApi(defaultClient);
        String sequenceId = "sequenceId_example"; // String | 
        EnrollContactsRequest enrollContactsRequest = new EnrollContactsRequest(); // EnrollContactsRequest | 
        try {
            apiInstance.enrollContacts(sequenceId, enrollContactsRequest);
        } catch (ApiException e) {
            System.err.println("Exception when calling SequencesApi#enrollContacts");
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
| **sequenceId** | **String**|  | |
| **enrollContactsRequest** | [**EnrollContactsRequest**](EnrollContactsRequest.md)|  | |

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
| **200** | Enrollment results |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## enrollContactsWithHttpInfo

> ApiResponse<Void> enrollContacts enrollContactsWithHttpInfo(sequenceId, enrollContactsRequest)

Enroll contacts in a sequence

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.SequencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        SequencesApi apiInstance = new SequencesApi(defaultClient);
        String sequenceId = "sequenceId_example"; // String | 
        EnrollContactsRequest enrollContactsRequest = new EnrollContactsRequest(); // EnrollContactsRequest | 
        try {
            ApiResponse<Void> response = apiInstance.enrollContactsWithHttpInfo(sequenceId, enrollContactsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling SequencesApi#enrollContacts");
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
| **sequenceId** | **String**|  | |
| **enrollContactsRequest** | [**EnrollContactsRequest**](EnrollContactsRequest.md)|  | |

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
| **200** | Enrollment results |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## getSequence

> void getSequence(sequenceId)

Get sequence with steps

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.SequencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        SequencesApi apiInstance = new SequencesApi(defaultClient);
        String sequenceId = "sequenceId_example"; // String | 
        try {
            apiInstance.getSequence(sequenceId);
        } catch (ApiException e) {
            System.err.println("Exception when calling SequencesApi#getSequence");
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
| **sequenceId** | **String**|  | |

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
| **200** | Sequence details with steps |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## getSequenceWithHttpInfo

> ApiResponse<Void> getSequence getSequenceWithHttpInfo(sequenceId)

Get sequence with steps

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.SequencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        SequencesApi apiInstance = new SequencesApi(defaultClient);
        String sequenceId = "sequenceId_example"; // String | 
        try {
            ApiResponse<Void> response = apiInstance.getSequenceWithHttpInfo(sequenceId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling SequencesApi#getSequence");
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
| **sequenceId** | **String**|  | |

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
| **200** | Sequence details with steps |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## listSequenceEnrollments

> void listSequenceEnrollments(sequenceId, status, limit, skip)

List enrollments for a sequence

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.SequencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        SequencesApi apiInstance = new SequencesApi(defaultClient);
        String sequenceId = "sequenceId_example"; // String | 
        String status = "active"; // String | 
        Integer limit = 50; // Integer | 
        Integer skip = 0; // Integer | 
        try {
            apiInstance.listSequenceEnrollments(sequenceId, status, limit, skip);
        } catch (ApiException e) {
            System.err.println("Exception when calling SequencesApi#listSequenceEnrollments");
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
| **sequenceId** | **String**|  | |
| **status** | **String**|  | [optional] [enum: active, completed, exited, paused] |
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
| **200** | Enrollments list with progress |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## listSequenceEnrollmentsWithHttpInfo

> ApiResponse<Void> listSequenceEnrollments listSequenceEnrollmentsWithHttpInfo(sequenceId, status, limit, skip)

List enrollments for a sequence

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.SequencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        SequencesApi apiInstance = new SequencesApi(defaultClient);
        String sequenceId = "sequenceId_example"; // String | 
        String status = "active"; // String | 
        Integer limit = 50; // Integer | 
        Integer skip = 0; // Integer | 
        try {
            ApiResponse<Void> response = apiInstance.listSequenceEnrollmentsWithHttpInfo(sequenceId, status, limit, skip);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling SequencesApi#listSequenceEnrollments");
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
| **sequenceId** | **String**|  | |
| **status** | **String**|  | [optional] [enum: active, completed, exited, paused] |
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
| **200** | Enrollments list with progress |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## listSequences

> void listSequences(profileId, status, limit, skip)

List sequences

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.SequencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        SequencesApi apiInstance = new SequencesApi(defaultClient);
        String profileId = "profileId_example"; // String | 
        String status = "draft"; // String | 
        Integer limit = 50; // Integer | 
        Integer skip = 0; // Integer | 
        try {
            apiInstance.listSequences(profileId, status, limit, skip);
        } catch (ApiException e) {
            System.err.println("Exception when calling SequencesApi#listSequences");
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
| **status** | **String**|  | [optional] [enum: draft, active, paused] |
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
| **200** | Sequences list |  -  |
| **401** | Unauthorized |  -  |

## listSequencesWithHttpInfo

> ApiResponse<Void> listSequences listSequencesWithHttpInfo(profileId, status, limit, skip)

List sequences

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.SequencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        SequencesApi apiInstance = new SequencesApi(defaultClient);
        String profileId = "profileId_example"; // String | 
        String status = "draft"; // String | 
        Integer limit = 50; // Integer | 
        Integer skip = 0; // Integer | 
        try {
            ApiResponse<Void> response = apiInstance.listSequencesWithHttpInfo(profileId, status, limit, skip);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling SequencesApi#listSequences");
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
| **status** | **String**|  | [optional] [enum: draft, active, paused] |
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
| **200** | Sequences list |  -  |
| **401** | Unauthorized |  -  |


## pauseSequence

> void pauseSequence(sequenceId)

Pause a sequence

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.SequencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        SequencesApi apiInstance = new SequencesApi(defaultClient);
        String sequenceId = "sequenceId_example"; // String | 
        try {
            apiInstance.pauseSequence(sequenceId);
        } catch (ApiException e) {
            System.err.println("Exception when calling SequencesApi#pauseSequence");
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
| **sequenceId** | **String**|  | |

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
| **200** | Sequence paused |  -  |
| **400** | Sequence is not active |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## pauseSequenceWithHttpInfo

> ApiResponse<Void> pauseSequence pauseSequenceWithHttpInfo(sequenceId)

Pause a sequence

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.SequencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        SequencesApi apiInstance = new SequencesApi(defaultClient);
        String sequenceId = "sequenceId_example"; // String | 
        try {
            ApiResponse<Void> response = apiInstance.pauseSequenceWithHttpInfo(sequenceId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling SequencesApi#pauseSequence");
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
| **sequenceId** | **String**|  | |

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
| **200** | Sequence paused |  -  |
| **400** | Sequence is not active |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## unenrollContact

> void unenrollContact(sequenceId, contactId)

Unenroll a contact from a sequence

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.SequencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        SequencesApi apiInstance = new SequencesApi(defaultClient);
        String sequenceId = "sequenceId_example"; // String | 
        String contactId = "contactId_example"; // String | 
        try {
            apiInstance.unenrollContact(sequenceId, contactId);
        } catch (ApiException e) {
            System.err.println("Exception when calling SequencesApi#unenrollContact");
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
| **sequenceId** | **String**|  | |
| **contactId** | **String**|  | |

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
| **200** | Contact unenrolled |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## unenrollContactWithHttpInfo

> ApiResponse<Void> unenrollContact unenrollContactWithHttpInfo(sequenceId, contactId)

Unenroll a contact from a sequence

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.SequencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        SequencesApi apiInstance = new SequencesApi(defaultClient);
        String sequenceId = "sequenceId_example"; // String | 
        String contactId = "contactId_example"; // String | 
        try {
            ApiResponse<Void> response = apiInstance.unenrollContactWithHttpInfo(sequenceId, contactId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling SequencesApi#unenrollContact");
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
| **sequenceId** | **String**|  | |
| **contactId** | **String**|  | |

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
| **200** | Contact unenrolled |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## updateSequence

> void updateSequence(sequenceId)

Update a sequence

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.SequencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        SequencesApi apiInstance = new SequencesApi(defaultClient);
        String sequenceId = "sequenceId_example"; // String | 
        try {
            apiInstance.updateSequence(sequenceId);
        } catch (ApiException e) {
            System.err.println("Exception when calling SequencesApi#updateSequence");
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
| **sequenceId** | **String**|  | |

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
| **200** | Sequence updated |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## updateSequenceWithHttpInfo

> ApiResponse<Void> updateSequence updateSequenceWithHttpInfo(sequenceId)

Update a sequence

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.SequencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        SequencesApi apiInstance = new SequencesApi(defaultClient);
        String sequenceId = "sequenceId_example"; // String | 
        try {
            ApiResponse<Void> response = apiInstance.updateSequenceWithHttpInfo(sequenceId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling SequencesApi#updateSequence");
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
| **sequenceId** | **String**|  | |

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
| **200** | Sequence updated |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

