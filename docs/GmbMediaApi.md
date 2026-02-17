# GmbMediaApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createGoogleBusinessMedia**](GmbMediaApi.md#createGoogleBusinessMedia) | **POST** /v1/accounts/{accountId}/gmb-media | Upload photo |
| [**createGoogleBusinessMediaWithHttpInfo**](GmbMediaApi.md#createGoogleBusinessMediaWithHttpInfo) | **POST** /v1/accounts/{accountId}/gmb-media | Upload photo |
| [**deleteGoogleBusinessMedia**](GmbMediaApi.md#deleteGoogleBusinessMedia) | **DELETE** /v1/accounts/{accountId}/gmb-media | Delete photo |
| [**deleteGoogleBusinessMediaWithHttpInfo**](GmbMediaApi.md#deleteGoogleBusinessMediaWithHttpInfo) | **DELETE** /v1/accounts/{accountId}/gmb-media | Delete photo |
| [**listGoogleBusinessMedia**](GmbMediaApi.md#listGoogleBusinessMedia) | **GET** /v1/accounts/{accountId}/gmb-media | List media |
| [**listGoogleBusinessMediaWithHttpInfo**](GmbMediaApi.md#listGoogleBusinessMediaWithHttpInfo) | **GET** /v1/accounts/{accountId}/gmb-media | List media |



## createGoogleBusinessMedia

> CreateGoogleBusinessMedia200Response createGoogleBusinessMedia(accountId, createGoogleBusinessMediaRequest)

Upload photo

Creates a media item (photo) for a location from a publicly accessible URL.  Categories determine where the photo appears: COVER, PROFILE, LOGO, EXTERIOR, INTERIOR, FOOD_AND_DRINK, MENU, PRODUCT, TEAMS, ADDITIONAL. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbMediaApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbMediaApi apiInstance = new GmbMediaApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        CreateGoogleBusinessMediaRequest createGoogleBusinessMediaRequest = new CreateGoogleBusinessMediaRequest(); // CreateGoogleBusinessMediaRequest | 
        try {
            CreateGoogleBusinessMedia200Response result = apiInstance.createGoogleBusinessMedia(accountId, createGoogleBusinessMediaRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbMediaApi#createGoogleBusinessMedia");
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
| **createGoogleBusinessMediaRequest** | [**CreateGoogleBusinessMediaRequest**](CreateGoogleBusinessMediaRequest.md)|  | |

### Return type

[**CreateGoogleBusinessMedia200Response**](CreateGoogleBusinessMedia200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Media created successfully |  -  |
| **400** | Invalid request or unsupported media format |  -  |
| **401** | Unauthorized |  -  |

## createGoogleBusinessMediaWithHttpInfo

> ApiResponse<CreateGoogleBusinessMedia200Response> createGoogleBusinessMedia createGoogleBusinessMediaWithHttpInfo(accountId, createGoogleBusinessMediaRequest)

Upload photo

Creates a media item (photo) for a location from a publicly accessible URL.  Categories determine where the photo appears: COVER, PROFILE, LOGO, EXTERIOR, INTERIOR, FOOD_AND_DRINK, MENU, PRODUCT, TEAMS, ADDITIONAL. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbMediaApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbMediaApi apiInstance = new GmbMediaApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        CreateGoogleBusinessMediaRequest createGoogleBusinessMediaRequest = new CreateGoogleBusinessMediaRequest(); // CreateGoogleBusinessMediaRequest | 
        try {
            ApiResponse<CreateGoogleBusinessMedia200Response> response = apiInstance.createGoogleBusinessMediaWithHttpInfo(accountId, createGoogleBusinessMediaRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbMediaApi#createGoogleBusinessMedia");
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
| **createGoogleBusinessMediaRequest** | [**CreateGoogleBusinessMediaRequest**](CreateGoogleBusinessMediaRequest.md)|  | |

### Return type

ApiResponse<[**CreateGoogleBusinessMedia200Response**](CreateGoogleBusinessMedia200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Media created successfully |  -  |
| **400** | Invalid request or unsupported media format |  -  |
| **401** | Unauthorized |  -  |


## deleteGoogleBusinessMedia

> DeleteGoogleBusinessMedia200Response deleteGoogleBusinessMedia(accountId, mediaId)

Delete photo

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbMediaApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbMediaApi apiInstance = new GmbMediaApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        String mediaId = "mediaId_example"; // String | The media item ID to delete
        try {
            DeleteGoogleBusinessMedia200Response result = apiInstance.deleteGoogleBusinessMedia(accountId, mediaId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbMediaApi#deleteGoogleBusinessMedia");
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
| **mediaId** | **String**| The media item ID to delete | |

### Return type

[**DeleteGoogleBusinessMedia200Response**](DeleteGoogleBusinessMedia200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Media deleted successfully |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |

## deleteGoogleBusinessMediaWithHttpInfo

> ApiResponse<DeleteGoogleBusinessMedia200Response> deleteGoogleBusinessMedia deleteGoogleBusinessMediaWithHttpInfo(accountId, mediaId)

Delete photo

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbMediaApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbMediaApi apiInstance = new GmbMediaApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        String mediaId = "mediaId_example"; // String | The media item ID to delete
        try {
            ApiResponse<DeleteGoogleBusinessMedia200Response> response = apiInstance.deleteGoogleBusinessMediaWithHttpInfo(accountId, mediaId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbMediaApi#deleteGoogleBusinessMedia");
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
| **mediaId** | **String**| The media item ID to delete | |

### Return type

ApiResponse<[**DeleteGoogleBusinessMedia200Response**](DeleteGoogleBusinessMedia200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Media deleted successfully |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |


## listGoogleBusinessMedia

> ListGoogleBusinessMedia200Response listGoogleBusinessMedia(accountId, pageSize, pageToken)

List media

Lists media items (photos) for a Google Business Profile location. Returns photo URLs, descriptions, categories, and metadata. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbMediaApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbMediaApi apiInstance = new GmbMediaApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        Integer pageSize = 100; // Integer | Number of items to return (max 100)
        String pageToken = "pageToken_example"; // String | Pagination token from previous response
        try {
            ListGoogleBusinessMedia200Response result = apiInstance.listGoogleBusinessMedia(accountId, pageSize, pageToken);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbMediaApi#listGoogleBusinessMedia");
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
| **pageSize** | **Integer**| Number of items to return (max 100) | [optional] [default to 100] |
| **pageToken** | **String**| Pagination token from previous response | [optional] |

### Return type

[**ListGoogleBusinessMedia200Response**](ListGoogleBusinessMedia200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Media items fetched successfully |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |

## listGoogleBusinessMediaWithHttpInfo

> ApiResponse<ListGoogleBusinessMedia200Response> listGoogleBusinessMedia listGoogleBusinessMediaWithHttpInfo(accountId, pageSize, pageToken)

List media

Lists media items (photos) for a Google Business Profile location. Returns photo URLs, descriptions, categories, and metadata. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbMediaApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbMediaApi apiInstance = new GmbMediaApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        Integer pageSize = 100; // Integer | Number of items to return (max 100)
        String pageToken = "pageToken_example"; // String | Pagination token from previous response
        try {
            ApiResponse<ListGoogleBusinessMedia200Response> response = apiInstance.listGoogleBusinessMediaWithHttpInfo(accountId, pageSize, pageToken);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbMediaApi#listGoogleBusinessMedia");
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
| **pageSize** | **Integer**| Number of items to return (max 100) | [optional] [default to 100] |
| **pageToken** | **String**| Pagination token from previous response | [optional] |

### Return type

ApiResponse<[**ListGoogleBusinessMedia200Response**](ListGoogleBusinessMedia200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Media items fetched successfully |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |

