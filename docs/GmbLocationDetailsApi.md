# GmbLocationDetailsApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getGoogleBusinessLocationDetails**](GmbLocationDetailsApi.md#getGoogleBusinessLocationDetails) | **GET** /v1/accounts/{accountId}/gmb-location-details | Get location details |
| [**getGoogleBusinessLocationDetailsWithHttpInfo**](GmbLocationDetailsApi.md#getGoogleBusinessLocationDetailsWithHttpInfo) | **GET** /v1/accounts/{accountId}/gmb-location-details | Get location details |
| [**updateGoogleBusinessLocationDetails**](GmbLocationDetailsApi.md#updateGoogleBusinessLocationDetails) | **PUT** /v1/accounts/{accountId}/gmb-location-details | Update location details |
| [**updateGoogleBusinessLocationDetailsWithHttpInfo**](GmbLocationDetailsApi.md#updateGoogleBusinessLocationDetailsWithHttpInfo) | **PUT** /v1/accounts/{accountId}/gmb-location-details | Update location details |



## getGoogleBusinessLocationDetails

> GetGoogleBusinessLocationDetails200Response getGoogleBusinessLocationDetails(accountId, readMask)

Get location details

Returns detailed GBP location info (hours, description, phone, website, categories). Use readMask to request specific fields.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbLocationDetailsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbLocationDetailsApi apiInstance = new GmbLocationDetailsApi(defaultClient);
        String accountId = "accountId_example"; // String | The Late account ID (from /v1/accounts)
        String readMask = "readMask_example"; // String | Comma-separated fields to return. Available: name, title, phoneNumbers, categories, storefrontAddress, websiteUri, regularHours, specialHours, serviceArea, profile, openInfo, metadata, moreHours.
        try {
            GetGoogleBusinessLocationDetails200Response result = apiInstance.getGoogleBusinessLocationDetails(accountId, readMask);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbLocationDetailsApi#getGoogleBusinessLocationDetails");
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
| **accountId** | **String**| The Late account ID (from /v1/accounts) | |
| **readMask** | **String**| Comma-separated fields to return. Available: name, title, phoneNumbers, categories, storefrontAddress, websiteUri, regularHours, specialHours, serviceArea, profile, openInfo, metadata, moreHours. | [optional] |

### Return type

[**GetGoogleBusinessLocationDetails200Response**](GetGoogleBusinessLocationDetails200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Location details fetched successfully |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized or token expired |  -  |
| **404** | Resource not found |  -  |

## getGoogleBusinessLocationDetailsWithHttpInfo

> ApiResponse<GetGoogleBusinessLocationDetails200Response> getGoogleBusinessLocationDetails getGoogleBusinessLocationDetailsWithHttpInfo(accountId, readMask)

Get location details

Returns detailed GBP location info (hours, description, phone, website, categories). Use readMask to request specific fields.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbLocationDetailsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbLocationDetailsApi apiInstance = new GmbLocationDetailsApi(defaultClient);
        String accountId = "accountId_example"; // String | The Late account ID (from /v1/accounts)
        String readMask = "readMask_example"; // String | Comma-separated fields to return. Available: name, title, phoneNumbers, categories, storefrontAddress, websiteUri, regularHours, specialHours, serviceArea, profile, openInfo, metadata, moreHours.
        try {
            ApiResponse<GetGoogleBusinessLocationDetails200Response> response = apiInstance.getGoogleBusinessLocationDetailsWithHttpInfo(accountId, readMask);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbLocationDetailsApi#getGoogleBusinessLocationDetails");
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
| **accountId** | **String**| The Late account ID (from /v1/accounts) | |
| **readMask** | **String**| Comma-separated fields to return. Available: name, title, phoneNumbers, categories, storefrontAddress, websiteUri, regularHours, specialHours, serviceArea, profile, openInfo, metadata, moreHours. | [optional] |

### Return type

ApiResponse<[**GetGoogleBusinessLocationDetails200Response**](GetGoogleBusinessLocationDetails200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Location details fetched successfully |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized or token expired |  -  |
| **404** | Resource not found |  -  |


## updateGoogleBusinessLocationDetails

> UpdateGoogleBusinessLocationDetails200Response updateGoogleBusinessLocationDetails(accountId, updateGoogleBusinessLocationDetailsRequest)

Update location details

Updates GBP location details (hours, description, phone, website). The updateMask field is required and specifies which fields to update.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbLocationDetailsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbLocationDetailsApi apiInstance = new GmbLocationDetailsApi(defaultClient);
        String accountId = "accountId_example"; // String | The Late account ID (from /v1/accounts)
        UpdateGoogleBusinessLocationDetailsRequest updateGoogleBusinessLocationDetailsRequest = new UpdateGoogleBusinessLocationDetailsRequest(); // UpdateGoogleBusinessLocationDetailsRequest | 
        try {
            UpdateGoogleBusinessLocationDetails200Response result = apiInstance.updateGoogleBusinessLocationDetails(accountId, updateGoogleBusinessLocationDetailsRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbLocationDetailsApi#updateGoogleBusinessLocationDetails");
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
| **accountId** | **String**| The Late account ID (from /v1/accounts) | |
| **updateGoogleBusinessLocationDetailsRequest** | [**UpdateGoogleBusinessLocationDetailsRequest**](UpdateGoogleBusinessLocationDetailsRequest.md)|  | |

### Return type

[**UpdateGoogleBusinessLocationDetails200Response**](UpdateGoogleBusinessLocationDetails200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Location updated successfully |  -  |
| **400** | Invalid request or missing updateMask |  -  |
| **401** | Unauthorized or token expired |  -  |
| **404** | Resource not found |  -  |

## updateGoogleBusinessLocationDetailsWithHttpInfo

> ApiResponse<UpdateGoogleBusinessLocationDetails200Response> updateGoogleBusinessLocationDetails updateGoogleBusinessLocationDetailsWithHttpInfo(accountId, updateGoogleBusinessLocationDetailsRequest)

Update location details

Updates GBP location details (hours, description, phone, website). The updateMask field is required and specifies which fields to update.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbLocationDetailsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbLocationDetailsApi apiInstance = new GmbLocationDetailsApi(defaultClient);
        String accountId = "accountId_example"; // String | The Late account ID (from /v1/accounts)
        UpdateGoogleBusinessLocationDetailsRequest updateGoogleBusinessLocationDetailsRequest = new UpdateGoogleBusinessLocationDetailsRequest(); // UpdateGoogleBusinessLocationDetailsRequest | 
        try {
            ApiResponse<UpdateGoogleBusinessLocationDetails200Response> response = apiInstance.updateGoogleBusinessLocationDetailsWithHttpInfo(accountId, updateGoogleBusinessLocationDetailsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbLocationDetailsApi#updateGoogleBusinessLocationDetails");
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
| **accountId** | **String**| The Late account ID (from /v1/accounts) | |
| **updateGoogleBusinessLocationDetailsRequest** | [**UpdateGoogleBusinessLocationDetailsRequest**](UpdateGoogleBusinessLocationDetailsRequest.md)|  | |

### Return type

ApiResponse<[**UpdateGoogleBusinessLocationDetails200Response**](UpdateGoogleBusinessLocationDetails200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Location updated successfully |  -  |
| **400** | Invalid request or missing updateMask |  -  |
| **401** | Unauthorized or token expired |  -  |
| **404** | Resource not found |  -  |

