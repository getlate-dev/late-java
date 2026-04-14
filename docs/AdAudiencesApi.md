# AdAudiencesApi

All URIs are relative to *https://zernio.com/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addUsersToAdAudience**](AdAudiencesApi.md#addUsersToAdAudience) | **POST** /v1/ads/audiences/{audienceId}/users | Add users to audience |
| [**addUsersToAdAudienceWithHttpInfo**](AdAudiencesApi.md#addUsersToAdAudienceWithHttpInfo) | **POST** /v1/ads/audiences/{audienceId}/users | Add users to audience |
| [**createAdAudience**](AdAudiencesApi.md#createAdAudience) | **POST** /v1/ads/audiences | Create custom audience |
| [**createAdAudienceWithHttpInfo**](AdAudiencesApi.md#createAdAudienceWithHttpInfo) | **POST** /v1/ads/audiences | Create custom audience |
| [**deleteAdAudience**](AdAudiencesApi.md#deleteAdAudience) | **DELETE** /v1/ads/audiences/{audienceId} | Delete custom audience |
| [**deleteAdAudienceWithHttpInfo**](AdAudiencesApi.md#deleteAdAudienceWithHttpInfo) | **DELETE** /v1/ads/audiences/{audienceId} | Delete custom audience |
| [**getAdAudience**](AdAudiencesApi.md#getAdAudience) | **GET** /v1/ads/audiences/{audienceId} | Get audience details |
| [**getAdAudienceWithHttpInfo**](AdAudiencesApi.md#getAdAudienceWithHttpInfo) | **GET** /v1/ads/audiences/{audienceId} | Get audience details |
| [**listAdAudiences**](AdAudiencesApi.md#listAdAudiences) | **GET** /v1/ads/audiences | List custom audiences |
| [**listAdAudiencesWithHttpInfo**](AdAudiencesApi.md#listAdAudiencesWithHttpInfo) | **GET** /v1/ads/audiences | List custom audiences |



## addUsersToAdAudience

> AddUsersToAdAudience200Response addUsersToAdAudience(audienceId, addUsersToAdAudienceRequest)

Add users to audience

Upload user data (emails and/or phone numbers) to a customer_list audience. Data is SHA256-hashed server-side before sending to Meta. Max 10,000 users per request.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdAudiencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdAudiencesApi apiInstance = new AdAudiencesApi(defaultClient);
        String audienceId = "audienceId_example"; // String | 
        AddUsersToAdAudienceRequest addUsersToAdAudienceRequest = new AddUsersToAdAudienceRequest(); // AddUsersToAdAudienceRequest | 
        try {
            AddUsersToAdAudience200Response result = apiInstance.addUsersToAdAudience(audienceId, addUsersToAdAudienceRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdAudiencesApi#addUsersToAdAudience");
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
| **audienceId** | **String**|  | |
| **addUsersToAdAudienceRequest** | [**AddUsersToAdAudienceRequest**](AddUsersToAdAudienceRequest.md)|  | |

### Return type

[**AddUsersToAdAudience200Response**](AddUsersToAdAudience200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Users added |  -  |
| **400** | Invalid input (empty users array, missing email/phone) |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Resource not found |  -  |
| **422** | Audience is not a customer_list type or has no platform ID yet |  -  |

## addUsersToAdAudienceWithHttpInfo

> ApiResponse<AddUsersToAdAudience200Response> addUsersToAdAudience addUsersToAdAudienceWithHttpInfo(audienceId, addUsersToAdAudienceRequest)

Add users to audience

Upload user data (emails and/or phone numbers) to a customer_list audience. Data is SHA256-hashed server-side before sending to Meta. Max 10,000 users per request.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdAudiencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdAudiencesApi apiInstance = new AdAudiencesApi(defaultClient);
        String audienceId = "audienceId_example"; // String | 
        AddUsersToAdAudienceRequest addUsersToAdAudienceRequest = new AddUsersToAdAudienceRequest(); // AddUsersToAdAudienceRequest | 
        try {
            ApiResponse<AddUsersToAdAudience200Response> response = apiInstance.addUsersToAdAudienceWithHttpInfo(audienceId, addUsersToAdAudienceRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdAudiencesApi#addUsersToAdAudience");
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
| **audienceId** | **String**|  | |
| **addUsersToAdAudienceRequest** | [**AddUsersToAdAudienceRequest**](AddUsersToAdAudienceRequest.md)|  | |

### Return type

ApiResponse<[**AddUsersToAdAudience200Response**](AddUsersToAdAudience200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Users added |  -  |
| **400** | Invalid input (empty users array, missing email/phone) |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Resource not found |  -  |
| **422** | Audience is not a customer_list type or has no platform ID yet |  -  |


## createAdAudience

> CreateAdAudience201Response createAdAudience(createAdAudienceRequest)

Create custom audience

Create a customer list, website retargeting, or lookalike audience on Meta (Facebook/Instagram).

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdAudiencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdAudiencesApi apiInstance = new AdAudiencesApi(defaultClient);
        CreateAdAudienceRequest createAdAudienceRequest = new CreateAdAudienceRequest(); // CreateAdAudienceRequest | 
        try {
            CreateAdAudience201Response result = apiInstance.createAdAudience(createAdAudienceRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdAudiencesApi#createAdAudience");
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
| **createAdAudienceRequest** | [**CreateAdAudienceRequest**](CreateAdAudienceRequest.md)|  | |

### Return type

[**CreateAdAudience201Response**](CreateAdAudience201Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Audience created |  -  |
| **400** | Missing required fields |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |

## createAdAudienceWithHttpInfo

> ApiResponse<CreateAdAudience201Response> createAdAudience createAdAudienceWithHttpInfo(createAdAudienceRequest)

Create custom audience

Create a customer list, website retargeting, or lookalike audience on Meta (Facebook/Instagram).

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdAudiencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdAudiencesApi apiInstance = new AdAudiencesApi(defaultClient);
        CreateAdAudienceRequest createAdAudienceRequest = new CreateAdAudienceRequest(); // CreateAdAudienceRequest | 
        try {
            ApiResponse<CreateAdAudience201Response> response = apiInstance.createAdAudienceWithHttpInfo(createAdAudienceRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdAudiencesApi#createAdAudience");
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
| **createAdAudienceRequest** | [**CreateAdAudienceRequest**](CreateAdAudienceRequest.md)|  | |

### Return type

ApiResponse<[**CreateAdAudience201Response**](CreateAdAudience201Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Audience created |  -  |
| **400** | Missing required fields |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |


## deleteAdAudience

> DeleteAccountGroup200Response deleteAdAudience(audienceId)

Delete custom audience

Deletes the audience from both Meta and the local database.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdAudiencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdAudiencesApi apiInstance = new AdAudiencesApi(defaultClient);
        String audienceId = "audienceId_example"; // String | 
        try {
            DeleteAccountGroup200Response result = apiInstance.deleteAdAudience(audienceId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdAudiencesApi#deleteAdAudience");
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
| **audienceId** | **String**|  | |

### Return type

[**DeleteAccountGroup200Response**](DeleteAccountGroup200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Audience deleted |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Resource not found |  -  |

## deleteAdAudienceWithHttpInfo

> ApiResponse<DeleteAccountGroup200Response> deleteAdAudience deleteAdAudienceWithHttpInfo(audienceId)

Delete custom audience

Deletes the audience from both Meta and the local database.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdAudiencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdAudiencesApi apiInstance = new AdAudiencesApi(defaultClient);
        String audienceId = "audienceId_example"; // String | 
        try {
            ApiResponse<DeleteAccountGroup200Response> response = apiInstance.deleteAdAudienceWithHttpInfo(audienceId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdAudiencesApi#deleteAdAudience");
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
| **audienceId** | **String**|  | |

### Return type

ApiResponse<[**DeleteAccountGroup200Response**](DeleteAccountGroup200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Audience deleted |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Resource not found |  -  |


## getAdAudience

> GetAdAudience200Response getAdAudience(audienceId)

Get audience details

Returns the local audience record and fresh data from Meta (if available).

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdAudiencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdAudiencesApi apiInstance = new AdAudiencesApi(defaultClient);
        String audienceId = "audienceId_example"; // String | 
        try {
            GetAdAudience200Response result = apiInstance.getAdAudience(audienceId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdAudiencesApi#getAdAudience");
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
| **audienceId** | **String**|  | |

### Return type

[**GetAdAudience200Response**](GetAdAudience200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Audience details |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Resource not found |  -  |

## getAdAudienceWithHttpInfo

> ApiResponse<GetAdAudience200Response> getAdAudience getAdAudienceWithHttpInfo(audienceId)

Get audience details

Returns the local audience record and fresh data from Meta (if available).

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdAudiencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdAudiencesApi apiInstance = new AdAudiencesApi(defaultClient);
        String audienceId = "audienceId_example"; // String | 
        try {
            ApiResponse<GetAdAudience200Response> response = apiInstance.getAdAudienceWithHttpInfo(audienceId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdAudiencesApi#getAdAudience");
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
| **audienceId** | **String**|  | |

### Return type

ApiResponse<[**GetAdAudience200Response**](GetAdAudience200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Audience details |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Resource not found |  -  |


## listAdAudiences

> ListAdAudiences200Response listAdAudiences(accountId, adAccountId, platform)

List custom audiences

Returns custom audiences for the given ad account. Supports Meta, Google, TikTok, and Pinterest.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdAudiencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdAudiencesApi apiInstance = new AdAudiencesApi(defaultClient);
        String accountId = "accountId_example"; // String | Social account ID
        String adAccountId = "adAccountId_example"; // String | Platform ad account ID
        String platform = "facebook"; // String | 
        try {
            ListAdAudiences200Response result = apiInstance.listAdAudiences(accountId, adAccountId, platform);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AdAudiencesApi#listAdAudiences");
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
| **accountId** | **String**| Social account ID | |
| **adAccountId** | **String**| Platform ad account ID | |
| **platform** | **String**|  | [optional] [enum: facebook, instagram, googleads, tiktok, pinterest] |

### Return type

[**ListAdAudiences200Response**](ListAdAudiences200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Audiences |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |

## listAdAudiencesWithHttpInfo

> ApiResponse<ListAdAudiences200Response> listAdAudiences listAdAudiencesWithHttpInfo(accountId, adAccountId, platform)

List custom audiences

Returns custom audiences for the given ad account. Supports Meta, Google, TikTok, and Pinterest.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.AdAudiencesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AdAudiencesApi apiInstance = new AdAudiencesApi(defaultClient);
        String accountId = "accountId_example"; // String | Social account ID
        String adAccountId = "adAccountId_example"; // String | Platform ad account ID
        String platform = "facebook"; // String | 
        try {
            ApiResponse<ListAdAudiences200Response> response = apiInstance.listAdAudiencesWithHttpInfo(accountId, adAccountId, platform);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AdAudiencesApi#listAdAudiences");
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
| **accountId** | **String**| Social account ID | |
| **adAccountId** | **String**| Platform ad account ID | |
| **platform** | **String**|  | [optional] [enum: facebook, instagram, googleads, tiktok, pinterest] |

### Return type

ApiResponse<[**ListAdAudiences200Response**](ListAdAudiences200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Audiences |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |

