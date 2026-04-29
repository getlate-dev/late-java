# GmbLocationDetailsApi

All URIs are relative to *https://zernio.com/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getGoogleBusinessLocationDetails**](GmbLocationDetailsApi.md#getGoogleBusinessLocationDetails) | **GET** /v1/accounts/{accountId}/gmb-location-details | Get location details |
| [**getGoogleBusinessLocationDetailsWithHttpInfo**](GmbLocationDetailsApi.md#getGoogleBusinessLocationDetailsWithHttpInfo) | **GET** /v1/accounts/{accountId}/gmb-location-details | Get location details |
| [**updateGoogleBusinessLocationDetails**](GmbLocationDetailsApi.md#updateGoogleBusinessLocationDetails) | **PUT** /v1/accounts/{accountId}/gmb-location-details | Update location details |
| [**updateGoogleBusinessLocationDetailsWithHttpInfo**](GmbLocationDetailsApi.md#updateGoogleBusinessLocationDetailsWithHttpInfo) | **PUT** /v1/accounts/{accountId}/gmb-location-details | Update location details |



## getGoogleBusinessLocationDetails

> GetGoogleBusinessLocationDetails200Response getGoogleBusinessLocationDetails(accountId, locationId, readMask)

Get location details

Returns detailed GBP location info (hours, description, phone, website, categories, services). Use readMask to request specific fields.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.GmbLocationDetailsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbLocationDetailsApi apiInstance = new GmbLocationDetailsApi(defaultClient);
        String accountId = "accountId_example"; // String | The Zernio account ID (from /v1/accounts)
        String locationId = "locationId_example"; // String | Override which location to query. If omitted, uses the account's selected location. Use GET /gmb-locations to list valid IDs.
        String readMask = "readMask_example"; // String | Comma-separated fields to return. Available: name, title, phoneNumbers, categories, storefrontAddress, websiteUri, regularHours, specialHours, serviceArea, serviceItems, profile, openInfo, metadata, moreHours. `title` and `metadata` are always included in the response so the `location` summary block can be populated, even if you omit them here. Note: `location` is a derived response field, not a Google readMask value, passing it returns 400. 
        try {
            GetGoogleBusinessLocationDetails200Response result = apiInstance.getGoogleBusinessLocationDetails(accountId, locationId, readMask);
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
| **accountId** | **String**| The Zernio account ID (from /v1/accounts) | |
| **locationId** | **String**| Override which location to query. If omitted, uses the account&#39;s selected location. Use GET /gmb-locations to list valid IDs. | [optional] |
| **readMask** | **String**| Comma-separated fields to return. Available: name, title, phoneNumbers, categories, storefrontAddress, websiteUri, regularHours, specialHours, serviceArea, serviceItems, profile, openInfo, metadata, moreHours. &#x60;title&#x60; and &#x60;metadata&#x60; are always included in the response so the &#x60;location&#x60; summary block can be populated, even if you omit them here. Note: &#x60;location&#x60; is a derived response field, not a Google readMask value, passing it returns 400.  | [optional] |

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
| **400** | Invalid request. Most commonly raised when the readMask query includes a value that is not a valid Google Business Information field (e.g. &#x60;location&#x60;, which is a response-only derived field).  |  -  |
| **401** | Unauthorized or token expired |  -  |
| **404** | Resource not found |  -  |

## getGoogleBusinessLocationDetailsWithHttpInfo

> ApiResponse<GetGoogleBusinessLocationDetails200Response> getGoogleBusinessLocationDetails getGoogleBusinessLocationDetailsWithHttpInfo(accountId, locationId, readMask)

Get location details

Returns detailed GBP location info (hours, description, phone, website, categories, services). Use readMask to request specific fields.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.GmbLocationDetailsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbLocationDetailsApi apiInstance = new GmbLocationDetailsApi(defaultClient);
        String accountId = "accountId_example"; // String | The Zernio account ID (from /v1/accounts)
        String locationId = "locationId_example"; // String | Override which location to query. If omitted, uses the account's selected location. Use GET /gmb-locations to list valid IDs.
        String readMask = "readMask_example"; // String | Comma-separated fields to return. Available: name, title, phoneNumbers, categories, storefrontAddress, websiteUri, regularHours, specialHours, serviceArea, serviceItems, profile, openInfo, metadata, moreHours. `title` and `metadata` are always included in the response so the `location` summary block can be populated, even if you omit them here. Note: `location` is a derived response field, not a Google readMask value, passing it returns 400. 
        try {
            ApiResponse<GetGoogleBusinessLocationDetails200Response> response = apiInstance.getGoogleBusinessLocationDetailsWithHttpInfo(accountId, locationId, readMask);
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
| **accountId** | **String**| The Zernio account ID (from /v1/accounts) | |
| **locationId** | **String**| Override which location to query. If omitted, uses the account&#39;s selected location. Use GET /gmb-locations to list valid IDs. | [optional] |
| **readMask** | **String**| Comma-separated fields to return. Available: name, title, phoneNumbers, categories, storefrontAddress, websiteUri, regularHours, specialHours, serviceArea, serviceItems, profile, openInfo, metadata, moreHours. &#x60;title&#x60; and &#x60;metadata&#x60; are always included in the response so the &#x60;location&#x60; summary block can be populated, even if you omit them here. Note: &#x60;location&#x60; is a derived response field, not a Google readMask value, passing it returns 400.  | [optional] |

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
| **400** | Invalid request. Most commonly raised when the readMask query includes a value that is not a valid Google Business Information field (e.g. &#x60;location&#x60;, which is a response-only derived field).  |  -  |
| **401** | Unauthorized or token expired |  -  |
| **404** | Resource not found |  -  |


## updateGoogleBusinessLocationDetails

> UpdateGoogleBusinessLocationDetails200Response updateGoogleBusinessLocationDetails(accountId, updateGoogleBusinessLocationDetailsRequest, locationId)

Update location details

Updates GBP location details. The updateMask field is required and specifies which fields to update. This endpoint proxies Google&#39;s Business Information API locations.patch, so any valid updateMask field is supported. Common fields: regularHours, specialHours, profile.description, websiteUri, phoneNumbers, categories, serviceItems. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.GmbLocationDetailsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbLocationDetailsApi apiInstance = new GmbLocationDetailsApi(defaultClient);
        String accountId = "accountId_example"; // String | The Zernio account ID (from /v1/accounts)
        UpdateGoogleBusinessLocationDetailsRequest updateGoogleBusinessLocationDetailsRequest = new UpdateGoogleBusinessLocationDetailsRequest(); // UpdateGoogleBusinessLocationDetailsRequest | 
        String locationId = "locationId_example"; // String | Override which location to target. If omitted, uses the account's selected location. Use GET /gmb-locations to list valid IDs.
        try {
            UpdateGoogleBusinessLocationDetails200Response result = apiInstance.updateGoogleBusinessLocationDetails(accountId, updateGoogleBusinessLocationDetailsRequest, locationId);
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
| **accountId** | **String**| The Zernio account ID (from /v1/accounts) | |
| **updateGoogleBusinessLocationDetailsRequest** | [**UpdateGoogleBusinessLocationDetailsRequest**](UpdateGoogleBusinessLocationDetailsRequest.md)|  | |
| **locationId** | **String**| Override which location to target. If omitted, uses the account&#39;s selected location. Use GET /gmb-locations to list valid IDs. | [optional] |

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

> ApiResponse<UpdateGoogleBusinessLocationDetails200Response> updateGoogleBusinessLocationDetails updateGoogleBusinessLocationDetailsWithHttpInfo(accountId, updateGoogleBusinessLocationDetailsRequest, locationId)

Update location details

Updates GBP location details. The updateMask field is required and specifies which fields to update. This endpoint proxies Google&#39;s Business Information API locations.patch, so any valid updateMask field is supported. Common fields: regularHours, specialHours, profile.description, websiteUri, phoneNumbers, categories, serviceItems. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.GmbLocationDetailsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbLocationDetailsApi apiInstance = new GmbLocationDetailsApi(defaultClient);
        String accountId = "accountId_example"; // String | The Zernio account ID (from /v1/accounts)
        UpdateGoogleBusinessLocationDetailsRequest updateGoogleBusinessLocationDetailsRequest = new UpdateGoogleBusinessLocationDetailsRequest(); // UpdateGoogleBusinessLocationDetailsRequest | 
        String locationId = "locationId_example"; // String | Override which location to target. If omitted, uses the account's selected location. Use GET /gmb-locations to list valid IDs.
        try {
            ApiResponse<UpdateGoogleBusinessLocationDetails200Response> response = apiInstance.updateGoogleBusinessLocationDetailsWithHttpInfo(accountId, updateGoogleBusinessLocationDetailsRequest, locationId);
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
| **accountId** | **String**| The Zernio account ID (from /v1/accounts) | |
| **updateGoogleBusinessLocationDetailsRequest** | [**UpdateGoogleBusinessLocationDetailsRequest**](UpdateGoogleBusinessLocationDetailsRequest.md)|  | |
| **locationId** | **String**| Override which location to target. If omitted, uses the account&#39;s selected location. Use GET /gmb-locations to list valid IDs. | [optional] |

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

