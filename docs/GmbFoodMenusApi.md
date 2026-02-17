# GmbFoodMenusApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getGoogleBusinessFoodMenus**](GmbFoodMenusApi.md#getGoogleBusinessFoodMenus) | **GET** /v1/accounts/{accountId}/gmb-food-menus | Get food menus |
| [**getGoogleBusinessFoodMenusWithHttpInfo**](GmbFoodMenusApi.md#getGoogleBusinessFoodMenusWithHttpInfo) | **GET** /v1/accounts/{accountId}/gmb-food-menus | Get food menus |
| [**updateGoogleBusinessFoodMenus**](GmbFoodMenusApi.md#updateGoogleBusinessFoodMenus) | **PUT** /v1/accounts/{accountId}/gmb-food-menus | Update food menus |
| [**updateGoogleBusinessFoodMenusWithHttpInfo**](GmbFoodMenusApi.md#updateGoogleBusinessFoodMenusWithHttpInfo) | **PUT** /v1/accounts/{accountId}/gmb-food-menus | Update food menus |



## getGoogleBusinessFoodMenus

> GetGoogleBusinessFoodMenus200Response getGoogleBusinessFoodMenus(accountId)

Get food menus

Fetches food menus for a connected Google Business Profile location.  Returns the full menu structure including: - Menu names and descriptions - Sections (e.g. Appetizers, Entrees, Drinks) - Items with labels, pricing, dietary info, and allergens - Item options/variants  Only available for locations with food menu support (restaurants, cafes, etc.). 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbFoodMenusApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbFoodMenusApi apiInstance = new GmbFoodMenusApi(defaultClient);
        String accountId = "accountId_example"; // String | The Late account ID (from /v1/accounts)
        try {
            GetGoogleBusinessFoodMenus200Response result = apiInstance.getGoogleBusinessFoodMenus(accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbFoodMenusApi#getGoogleBusinessFoodMenus");
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

### Return type

[**GetGoogleBusinessFoodMenus200Response**](GetGoogleBusinessFoodMenus200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Food menus fetched successfully |  -  |
| **400** | Invalid request - not a Google Business account or missing location |  -  |
| **401** | Unauthorized or token expired |  -  |
| **403** | Permission denied for this location |  -  |
| **404** | Resource not found |  -  |
| **500** | Failed to fetch food menus |  -  |

## getGoogleBusinessFoodMenusWithHttpInfo

> ApiResponse<GetGoogleBusinessFoodMenus200Response> getGoogleBusinessFoodMenus getGoogleBusinessFoodMenusWithHttpInfo(accountId)

Get food menus

Fetches food menus for a connected Google Business Profile location.  Returns the full menu structure including: - Menu names and descriptions - Sections (e.g. Appetizers, Entrees, Drinks) - Items with labels, pricing, dietary info, and allergens - Item options/variants  Only available for locations with food menu support (restaurants, cafes, etc.). 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbFoodMenusApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbFoodMenusApi apiInstance = new GmbFoodMenusApi(defaultClient);
        String accountId = "accountId_example"; // String | The Late account ID (from /v1/accounts)
        try {
            ApiResponse<GetGoogleBusinessFoodMenus200Response> response = apiInstance.getGoogleBusinessFoodMenusWithHttpInfo(accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbFoodMenusApi#getGoogleBusinessFoodMenus");
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

### Return type

ApiResponse<[**GetGoogleBusinessFoodMenus200Response**](GetGoogleBusinessFoodMenus200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Food menus fetched successfully |  -  |
| **400** | Invalid request - not a Google Business account or missing location |  -  |
| **401** | Unauthorized or token expired |  -  |
| **403** | Permission denied for this location |  -  |
| **404** | Resource not found |  -  |
| **500** | Failed to fetch food menus |  -  |


## updateGoogleBusinessFoodMenus

> UpdateGoogleBusinessFoodMenus200Response updateGoogleBusinessFoodMenus(accountId, updateGoogleBusinessFoodMenusRequest)

Update food menus

Updates the food menus for a connected Google Business Profile location.  Send the full menus array. Use &#x60;updateMask&#x60; for partial updates (e.g. &#x60;\&quot;menus\&quot;&#x60; to only update the menus field).  Each menu can contain sections, and each section can contain items with pricing, dietary restrictions, allergens, and more. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbFoodMenusApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbFoodMenusApi apiInstance = new GmbFoodMenusApi(defaultClient);
        String accountId = "accountId_example"; // String | The Late account ID (from /v1/accounts)
        UpdateGoogleBusinessFoodMenusRequest updateGoogleBusinessFoodMenusRequest = new UpdateGoogleBusinessFoodMenusRequest(); // UpdateGoogleBusinessFoodMenusRequest | 
        try {
            UpdateGoogleBusinessFoodMenus200Response result = apiInstance.updateGoogleBusinessFoodMenus(accountId, updateGoogleBusinessFoodMenusRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbFoodMenusApi#updateGoogleBusinessFoodMenus");
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
| **updateGoogleBusinessFoodMenusRequest** | [**UpdateGoogleBusinessFoodMenusRequest**](UpdateGoogleBusinessFoodMenusRequest.md)|  | |

### Return type

[**UpdateGoogleBusinessFoodMenus200Response**](UpdateGoogleBusinessFoodMenus200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Food menus updated successfully |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized or token expired |  -  |
| **403** | Permission denied for this location |  -  |
| **404** | Resource not found |  -  |
| **500** | Failed to update food menus |  -  |

## updateGoogleBusinessFoodMenusWithHttpInfo

> ApiResponse<UpdateGoogleBusinessFoodMenus200Response> updateGoogleBusinessFoodMenus updateGoogleBusinessFoodMenusWithHttpInfo(accountId, updateGoogleBusinessFoodMenusRequest)

Update food menus

Updates the food menus for a connected Google Business Profile location.  Send the full menus array. Use &#x60;updateMask&#x60; for partial updates (e.g. &#x60;\&quot;menus\&quot;&#x60; to only update the menus field).  Each menu can contain sections, and each section can contain items with pricing, dietary restrictions, allergens, and more. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbFoodMenusApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbFoodMenusApi apiInstance = new GmbFoodMenusApi(defaultClient);
        String accountId = "accountId_example"; // String | The Late account ID (from /v1/accounts)
        UpdateGoogleBusinessFoodMenusRequest updateGoogleBusinessFoodMenusRequest = new UpdateGoogleBusinessFoodMenusRequest(); // UpdateGoogleBusinessFoodMenusRequest | 
        try {
            ApiResponse<UpdateGoogleBusinessFoodMenus200Response> response = apiInstance.updateGoogleBusinessFoodMenusWithHttpInfo(accountId, updateGoogleBusinessFoodMenusRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbFoodMenusApi#updateGoogleBusinessFoodMenus");
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
| **updateGoogleBusinessFoodMenusRequest** | [**UpdateGoogleBusinessFoodMenusRequest**](UpdateGoogleBusinessFoodMenusRequest.md)|  | |

### Return type

ApiResponse<[**UpdateGoogleBusinessFoodMenus200Response**](UpdateGoogleBusinessFoodMenus200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Food menus updated successfully |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized or token expired |  -  |
| **403** | Permission denied for this location |  -  |
| **404** | Resource not found |  -  |
| **500** | Failed to update food menus |  -  |

