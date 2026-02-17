# GmbAttributesApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getGoogleBusinessAttributes**](GmbAttributesApi.md#getGoogleBusinessAttributes) | **GET** /v1/accounts/{accountId}/gmb-attributes | Get attributes |
| [**getGoogleBusinessAttributesWithHttpInfo**](GmbAttributesApi.md#getGoogleBusinessAttributesWithHttpInfo) | **GET** /v1/accounts/{accountId}/gmb-attributes | Get attributes |
| [**updateGoogleBusinessAttributes**](GmbAttributesApi.md#updateGoogleBusinessAttributes) | **PUT** /v1/accounts/{accountId}/gmb-attributes | Update attributes |
| [**updateGoogleBusinessAttributesWithHttpInfo**](GmbAttributesApi.md#updateGoogleBusinessAttributesWithHttpInfo) | **PUT** /v1/accounts/{accountId}/gmb-attributes | Update attributes |



## getGoogleBusinessAttributes

> GetGoogleBusinessAttributes200Response getGoogleBusinessAttributes(accountId)

Get attributes

Fetches location attributes such as amenities, services, and accessibility features. Common attributes include dining options (has_dine_in, has_takeout, has_delivery), amenities (has_outdoor_seating, has_wifi), accessibility, and payment types. Available attributes vary by business category. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbAttributesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbAttributesApi apiInstance = new GmbAttributesApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        try {
            GetGoogleBusinessAttributes200Response result = apiInstance.getGoogleBusinessAttributes(accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbAttributesApi#getGoogleBusinessAttributes");
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
| **accountId** | **String**|  | |

### Return type

[**GetGoogleBusinessAttributes200Response**](GetGoogleBusinessAttributes200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Attributes fetched successfully |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |

## getGoogleBusinessAttributesWithHttpInfo

> ApiResponse<GetGoogleBusinessAttributes200Response> getGoogleBusinessAttributes getGoogleBusinessAttributesWithHttpInfo(accountId)

Get attributes

Fetches location attributes such as amenities, services, and accessibility features. Common attributes include dining options (has_dine_in, has_takeout, has_delivery), amenities (has_outdoor_seating, has_wifi), accessibility, and payment types. Available attributes vary by business category. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbAttributesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbAttributesApi apiInstance = new GmbAttributesApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        try {
            ApiResponse<GetGoogleBusinessAttributes200Response> response = apiInstance.getGoogleBusinessAttributesWithHttpInfo(accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbAttributesApi#getGoogleBusinessAttributes");
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
| **accountId** | **String**|  | |

### Return type

ApiResponse<[**GetGoogleBusinessAttributes200Response**](GetGoogleBusinessAttributes200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Attributes fetched successfully |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |


## updateGoogleBusinessAttributes

> UpdateGoogleBusinessAttributes200Response updateGoogleBusinessAttributes(accountId, updateGoogleBusinessAttributesRequest)

Update attributes

Updates location attributes (amenities, services, etc.).  The attributeMask specifies which attributes to update (comma-separated). 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbAttributesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbAttributesApi apiInstance = new GmbAttributesApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        UpdateGoogleBusinessAttributesRequest updateGoogleBusinessAttributesRequest = new UpdateGoogleBusinessAttributesRequest(); // UpdateGoogleBusinessAttributesRequest | 
        try {
            UpdateGoogleBusinessAttributes200Response result = apiInstance.updateGoogleBusinessAttributes(accountId, updateGoogleBusinessAttributesRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbAttributesApi#updateGoogleBusinessAttributes");
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
| **accountId** | **String**|  | |
| **updateGoogleBusinessAttributesRequest** | [**UpdateGoogleBusinessAttributesRequest**](UpdateGoogleBusinessAttributesRequest.md)|  | |

### Return type

[**UpdateGoogleBusinessAttributes200Response**](UpdateGoogleBusinessAttributes200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Attributes updated successfully |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |

## updateGoogleBusinessAttributesWithHttpInfo

> ApiResponse<UpdateGoogleBusinessAttributes200Response> updateGoogleBusinessAttributes updateGoogleBusinessAttributesWithHttpInfo(accountId, updateGoogleBusinessAttributesRequest)

Update attributes

Updates location attributes (amenities, services, etc.).  The attributeMask specifies which attributes to update (comma-separated). 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbAttributesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbAttributesApi apiInstance = new GmbAttributesApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        UpdateGoogleBusinessAttributesRequest updateGoogleBusinessAttributesRequest = new UpdateGoogleBusinessAttributesRequest(); // UpdateGoogleBusinessAttributesRequest | 
        try {
            ApiResponse<UpdateGoogleBusinessAttributes200Response> response = apiInstance.updateGoogleBusinessAttributesWithHttpInfo(accountId, updateGoogleBusinessAttributesRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbAttributesApi#updateGoogleBusinessAttributes");
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
| **accountId** | **String**|  | |
| **updateGoogleBusinessAttributesRequest** | [**UpdateGoogleBusinessAttributesRequest**](UpdateGoogleBusinessAttributesRequest.md)|  | |

### Return type

ApiResponse<[**UpdateGoogleBusinessAttributes200Response**](UpdateGoogleBusinessAttributes200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Attributes updated successfully |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |

