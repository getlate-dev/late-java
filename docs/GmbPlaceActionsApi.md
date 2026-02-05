# GmbPlaceActionsApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createGoogleBusinessPlaceAction**](GmbPlaceActionsApi.md#createGoogleBusinessPlaceAction) | **POST** /v1/accounts/{accountId}/gmb-place-actions | Create a place action link (booking, ordering, reservation) |
| [**createGoogleBusinessPlaceActionWithHttpInfo**](GmbPlaceActionsApi.md#createGoogleBusinessPlaceActionWithHttpInfo) | **POST** /v1/accounts/{accountId}/gmb-place-actions | Create a place action link (booking, ordering, reservation) |
| [**deleteGoogleBusinessPlaceAction**](GmbPlaceActionsApi.md#deleteGoogleBusinessPlaceAction) | **DELETE** /v1/accounts/{accountId}/gmb-place-actions | Delete a place action link |
| [**deleteGoogleBusinessPlaceActionWithHttpInfo**](GmbPlaceActionsApi.md#deleteGoogleBusinessPlaceActionWithHttpInfo) | **DELETE** /v1/accounts/{accountId}/gmb-place-actions | Delete a place action link |
| [**listGoogleBusinessPlaceActions**](GmbPlaceActionsApi.md#listGoogleBusinessPlaceActions) | **GET** /v1/accounts/{accountId}/gmb-place-actions | List place action links (booking, ordering, reservations) |
| [**listGoogleBusinessPlaceActionsWithHttpInfo**](GmbPlaceActionsApi.md#listGoogleBusinessPlaceActionsWithHttpInfo) | **GET** /v1/accounts/{accountId}/gmb-place-actions | List place action links (booking, ordering, reservations) |



## createGoogleBusinessPlaceAction

> CreateGoogleBusinessPlaceAction200Response createGoogleBusinessPlaceAction(accountId, createGoogleBusinessPlaceActionRequest)

Create a place action link (booking, ordering, reservation)

Creates a place action link for a location.  Available action types: - &#x60;APPOINTMENT&#x60; - Booking an appointment - &#x60;ONLINE_APPOINTMENT&#x60; - Booking an online appointment - &#x60;DINING_RESERVATION&#x60; - Making a dining reservation (OpenTable, Resy, etc.) - &#x60;FOOD_ORDERING&#x60; - Ordering food for delivery and/or takeout (DoorDash, Uber Eats, etc.) - &#x60;FOOD_DELIVERY&#x60; - Ordering food for delivery only - &#x60;FOOD_TAKEOUT&#x60; - Ordering food for takeout only - &#x60;SHOP_ONLINE&#x60; - Shopping with delivery and/or pickup 

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

Create a place action link (booking, ordering, reservation)

Creates a place action link for a location.  Available action types: - &#x60;APPOINTMENT&#x60; - Booking an appointment - &#x60;ONLINE_APPOINTMENT&#x60; - Booking an online appointment - &#x60;DINING_RESERVATION&#x60; - Making a dining reservation (OpenTable, Resy, etc.) - &#x60;FOOD_ORDERING&#x60; - Ordering food for delivery and/or takeout (DoorDash, Uber Eats, etc.) - &#x60;FOOD_DELIVERY&#x60; - Ordering food for delivery only - &#x60;FOOD_TAKEOUT&#x60; - Ordering food for takeout only - &#x60;SHOP_ONLINE&#x60; - Shopping with delivery and/or pickup 

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

Delete a place action link

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

Delete a place action link

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

List place action links (booking, ordering, reservations)

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

List place action links (booking, ordering, reservations)

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

