# GmbPlaceActionsApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createGoogleBusinessPlaceAction**](GmbPlaceActionsApi.md#createGoogleBusinessPlaceAction) | **POST** /v1/accounts/{accountId}/gmb-place-actions | Create action link |
| [**createGoogleBusinessPlaceActionWithHttpInfo**](GmbPlaceActionsApi.md#createGoogleBusinessPlaceActionWithHttpInfo) | **POST** /v1/accounts/{accountId}/gmb-place-actions | Create action link |
| [**deleteGoogleBusinessPlaceAction**](GmbPlaceActionsApi.md#deleteGoogleBusinessPlaceAction) | **DELETE** /v1/accounts/{accountId}/gmb-place-actions | Delete action link |
| [**deleteGoogleBusinessPlaceActionWithHttpInfo**](GmbPlaceActionsApi.md#deleteGoogleBusinessPlaceActionWithHttpInfo) | **DELETE** /v1/accounts/{accountId}/gmb-place-actions | Delete action link |
| [**listGoogleBusinessPlaceActions**](GmbPlaceActionsApi.md#listGoogleBusinessPlaceActions) | **GET** /v1/accounts/{accountId}/gmb-place-actions | List action links |
| [**listGoogleBusinessPlaceActionsWithHttpInfo**](GmbPlaceActionsApi.md#listGoogleBusinessPlaceActionsWithHttpInfo) | **GET** /v1/accounts/{accountId}/gmb-place-actions | List action links |



## createGoogleBusinessPlaceAction

> CreateGoogleBusinessPlaceAction200Response createGoogleBusinessPlaceAction(accountId, createGoogleBusinessPlaceActionRequest)

Create action link

Creates a place action link for a location.  Available action types: APPOINTMENT, ONLINE_APPOINTMENT, DINING_RESERVATION, FOOD_ORDERING, FOOD_DELIVERY, FOOD_TAKEOUT, SHOP_ONLINE. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbPlaceActionsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbPlaceActionsApi apiInstance = new GmbPlaceActionsApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        CreateGoogleBusinessPlaceActionRequest createGoogleBusinessPlaceActionRequest = new CreateGoogleBusinessPlaceActionRequest(); // CreateGoogleBusinessPlaceActionRequest | 
        try {
            CreateGoogleBusinessPlaceAction200Response result = apiInstance.createGoogleBusinessPlaceAction(accountId, createGoogleBusinessPlaceActionRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbPlaceActionsApi#createGoogleBusinessPlaceAction");
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
| **createGoogleBusinessPlaceActionRequest** | [**CreateGoogleBusinessPlaceActionRequest**](CreateGoogleBusinessPlaceActionRequest.md)|  | |

### Return type

[**CreateGoogleBusinessPlaceAction200Response**](CreateGoogleBusinessPlaceAction200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Place action created successfully |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |

## createGoogleBusinessPlaceActionWithHttpInfo

> ApiResponse<CreateGoogleBusinessPlaceAction200Response> createGoogleBusinessPlaceAction createGoogleBusinessPlaceActionWithHttpInfo(accountId, createGoogleBusinessPlaceActionRequest)

Create action link

Creates a place action link for a location.  Available action types: APPOINTMENT, ONLINE_APPOINTMENT, DINING_RESERVATION, FOOD_ORDERING, FOOD_DELIVERY, FOOD_TAKEOUT, SHOP_ONLINE. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbPlaceActionsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbPlaceActionsApi apiInstance = new GmbPlaceActionsApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        CreateGoogleBusinessPlaceActionRequest createGoogleBusinessPlaceActionRequest = new CreateGoogleBusinessPlaceActionRequest(); // CreateGoogleBusinessPlaceActionRequest | 
        try {
            ApiResponse<CreateGoogleBusinessPlaceAction200Response> response = apiInstance.createGoogleBusinessPlaceActionWithHttpInfo(accountId, createGoogleBusinessPlaceActionRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbPlaceActionsApi#createGoogleBusinessPlaceAction");
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
| **createGoogleBusinessPlaceActionRequest** | [**CreateGoogleBusinessPlaceActionRequest**](CreateGoogleBusinessPlaceActionRequest.md)|  | |

### Return type

ApiResponse<[**CreateGoogleBusinessPlaceAction200Response**](CreateGoogleBusinessPlaceAction200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Place action created successfully |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |


## deleteGoogleBusinessPlaceAction

> DeleteGoogleBusinessPlaceAction200Response deleteGoogleBusinessPlaceAction(accountId, name)

Delete action link

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbPlaceActionsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbPlaceActionsApi apiInstance = new GmbPlaceActionsApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        String name = "name_example"; // String | The resource name of the place action link (e.g. locations/123/placeActionLinks/456)
        try {
            DeleteGoogleBusinessPlaceAction200Response result = apiInstance.deleteGoogleBusinessPlaceAction(accountId, name);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbPlaceActionsApi#deleteGoogleBusinessPlaceAction");
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
| **name** | **String**| The resource name of the place action link (e.g. locations/123/placeActionLinks/456) | |

### Return type

[**DeleteGoogleBusinessPlaceAction200Response**](DeleteGoogleBusinessPlaceAction200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Place action deleted successfully |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |

## deleteGoogleBusinessPlaceActionWithHttpInfo

> ApiResponse<DeleteGoogleBusinessPlaceAction200Response> deleteGoogleBusinessPlaceAction deleteGoogleBusinessPlaceActionWithHttpInfo(accountId, name)

Delete action link

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbPlaceActionsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbPlaceActionsApi apiInstance = new GmbPlaceActionsApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        String name = "name_example"; // String | The resource name of the place action link (e.g. locations/123/placeActionLinks/456)
        try {
            ApiResponse<DeleteGoogleBusinessPlaceAction200Response> response = apiInstance.deleteGoogleBusinessPlaceActionWithHttpInfo(accountId, name);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbPlaceActionsApi#deleteGoogleBusinessPlaceAction");
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
| **name** | **String**| The resource name of the place action link (e.g. locations/123/placeActionLinks/456) | |

### Return type

ApiResponse<[**DeleteGoogleBusinessPlaceAction200Response**](DeleteGoogleBusinessPlaceAction200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Place action deleted successfully |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |


## listGoogleBusinessPlaceActions

> ListGoogleBusinessPlaceActions200Response listGoogleBusinessPlaceActions(accountId, pageSize, pageToken)

List action links

Lists place action links for a Google Business Profile location.  Place actions are the booking, ordering, and reservation buttons that appear on your listing. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbPlaceActionsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbPlaceActionsApi apiInstance = new GmbPlaceActionsApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        Integer pageSize = 100; // Integer | 
        String pageToken = "pageToken_example"; // String | 
        try {
            ListGoogleBusinessPlaceActions200Response result = apiInstance.listGoogleBusinessPlaceActions(accountId, pageSize, pageToken);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbPlaceActionsApi#listGoogleBusinessPlaceActions");
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
| **pageSize** | **Integer**|  | [optional] [default to 100] |
| **pageToken** | **String**|  | [optional] |

### Return type

[**ListGoogleBusinessPlaceActions200Response**](ListGoogleBusinessPlaceActions200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Place actions fetched successfully |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |

## listGoogleBusinessPlaceActionsWithHttpInfo

> ApiResponse<ListGoogleBusinessPlaceActions200Response> listGoogleBusinessPlaceActions listGoogleBusinessPlaceActionsWithHttpInfo(accountId, pageSize, pageToken)

List action links

Lists place action links for a Google Business Profile location.  Place actions are the booking, ordering, and reservation buttons that appear on your listing. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbPlaceActionsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbPlaceActionsApi apiInstance = new GmbPlaceActionsApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        Integer pageSize = 100; // Integer | 
        String pageToken = "pageToken_example"; // String | 
        try {
            ApiResponse<ListGoogleBusinessPlaceActions200Response> response = apiInstance.listGoogleBusinessPlaceActionsWithHttpInfo(accountId, pageSize, pageToken);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbPlaceActionsApi#listGoogleBusinessPlaceActions");
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
| **pageSize** | **Integer**|  | [optional] [default to 100] |
| **pageToken** | **String**|  | [optional] |

### Return type

ApiResponse<[**ListGoogleBusinessPlaceActions200Response**](ListGoogleBusinessPlaceActions200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Place actions fetched successfully |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |

