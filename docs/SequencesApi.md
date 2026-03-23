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

> ActivateSequence200Response activateSequence(sequenceId)

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
            ActivateSequence200Response result = apiInstance.activateSequence(sequenceId);
            System.out.println(result);
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

[**ActivateSequence200Response**](ActivateSequence200Response.md)


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

> ApiResponse<ActivateSequence200Response> activateSequence activateSequenceWithHttpInfo(sequenceId)

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
            ApiResponse<ActivateSequence200Response> response = apiInstance.activateSequenceWithHttpInfo(sequenceId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
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

ApiResponse<[**ActivateSequence200Response**](ActivateSequence200Response.md)>


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

> CreateSequence200Response createSequence(createSequenceRequest)

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
            CreateSequence200Response result = apiInstance.createSequence(createSequenceRequest);
            System.out.println(result);
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

[**CreateSequence200Response**](CreateSequence200Response.md)


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

> ApiResponse<CreateSequence200Response> createSequence createSequenceWithHttpInfo(createSequenceRequest)

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
            ApiResponse<CreateSequence200Response> response = apiInstance.createSequenceWithHttpInfo(createSequenceRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
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

ApiResponse<[**CreateSequence200Response**](CreateSequence200Response.md)>


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

> EnrollContacts200Response enrollContacts(sequenceId, enrollContactsRequest)

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
            EnrollContacts200Response result = apiInstance.enrollContacts(sequenceId, enrollContactsRequest);
            System.out.println(result);
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

[**EnrollContacts200Response**](EnrollContacts200Response.md)


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

> ApiResponse<EnrollContacts200Response> enrollContacts enrollContactsWithHttpInfo(sequenceId, enrollContactsRequest)

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
            ApiResponse<EnrollContacts200Response> response = apiInstance.enrollContactsWithHttpInfo(sequenceId, enrollContactsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
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

ApiResponse<[**EnrollContacts200Response**](EnrollContacts200Response.md)>


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

> GetSequence200Response getSequence(sequenceId)

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
            GetSequence200Response result = apiInstance.getSequence(sequenceId);
            System.out.println(result);
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

[**GetSequence200Response**](GetSequence200Response.md)


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

> ApiResponse<GetSequence200Response> getSequence getSequenceWithHttpInfo(sequenceId)

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
            ApiResponse<GetSequence200Response> response = apiInstance.getSequenceWithHttpInfo(sequenceId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
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

ApiResponse<[**GetSequence200Response**](GetSequence200Response.md)>


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

> ListSequenceEnrollments200Response listSequenceEnrollments(sequenceId, status, limit, skip)

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
            ListSequenceEnrollments200Response result = apiInstance.listSequenceEnrollments(sequenceId, status, limit, skip);
            System.out.println(result);
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

[**ListSequenceEnrollments200Response**](ListSequenceEnrollments200Response.md)


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

> ApiResponse<ListSequenceEnrollments200Response> listSequenceEnrollments listSequenceEnrollmentsWithHttpInfo(sequenceId, status, limit, skip)

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
            ApiResponse<ListSequenceEnrollments200Response> response = apiInstance.listSequenceEnrollmentsWithHttpInfo(sequenceId, status, limit, skip);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
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

ApiResponse<[**ListSequenceEnrollments200Response**](ListSequenceEnrollments200Response.md)>


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

> ListSequences200Response listSequences(profileId, status, limit, skip)

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
        String profileId = "profileId_example"; // String | Filter by profile. Omit to list across all profiles
        String status = "draft"; // String | 
        Integer limit = 50; // Integer | 
        Integer skip = 0; // Integer | 
        try {
            ListSequences200Response result = apiInstance.listSequences(profileId, status, limit, skip);
            System.out.println(result);
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
| **profileId** | **String**| Filter by profile. Omit to list across all profiles | [optional] |
| **status** | **String**|  | [optional] [enum: draft, active, paused] |
| **limit** | **Integer**|  | [optional] [default to 50] |
| **skip** | **Integer**|  | [optional] [default to 0] |

### Return type

[**ListSequences200Response**](ListSequences200Response.md)


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

> ApiResponse<ListSequences200Response> listSequences listSequencesWithHttpInfo(profileId, status, limit, skip)

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
        String profileId = "profileId_example"; // String | Filter by profile. Omit to list across all profiles
        String status = "draft"; // String | 
        Integer limit = 50; // Integer | 
        Integer skip = 0; // Integer | 
        try {
            ApiResponse<ListSequences200Response> response = apiInstance.listSequencesWithHttpInfo(profileId, status, limit, skip);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
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
| **profileId** | **String**| Filter by profile. Omit to list across all profiles | [optional] |
| **status** | **String**|  | [optional] [enum: draft, active, paused] |
| **limit** | **Integer**|  | [optional] [default to 50] |
| **skip** | **Integer**|  | [optional] [default to 0] |

### Return type

ApiResponse<[**ListSequences200Response**](ListSequences200Response.md)>


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

> ActivateSequence200Response pauseSequence(sequenceId)

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
            ActivateSequence200Response result = apiInstance.pauseSequence(sequenceId);
            System.out.println(result);
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

[**ActivateSequence200Response**](ActivateSequence200Response.md)


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

> ApiResponse<ActivateSequence200Response> pauseSequence pauseSequenceWithHttpInfo(sequenceId)

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
            ApiResponse<ActivateSequence200Response> response = apiInstance.pauseSequenceWithHttpInfo(sequenceId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
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

ApiResponse<[**ActivateSequence200Response**](ActivateSequence200Response.md)>


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

> UpdateSequence200Response updateSequence(sequenceId)

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
            UpdateSequence200Response result = apiInstance.updateSequence(sequenceId);
            System.out.println(result);
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

[**UpdateSequence200Response**](UpdateSequence200Response.md)


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

> ApiResponse<UpdateSequence200Response> updateSequence updateSequenceWithHttpInfo(sequenceId)

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
            ApiResponse<UpdateSequence200Response> response = apiInstance.updateSequenceWithHttpInfo(sequenceId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
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

ApiResponse<[**UpdateSequence200Response**](UpdateSequence200Response.md)>


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

