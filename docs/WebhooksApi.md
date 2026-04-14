# WebhooksApi

All URIs are relative to *https://zernio.com/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createWebhookSettings**](WebhooksApi.md#createWebhookSettings) | **POST** /v1/webhooks/settings | Create webhook |
| [**createWebhookSettingsWithHttpInfo**](WebhooksApi.md#createWebhookSettingsWithHttpInfo) | **POST** /v1/webhooks/settings | Create webhook |
| [**deleteWebhookSettings**](WebhooksApi.md#deleteWebhookSettings) | **DELETE** /v1/webhooks/settings | Delete webhook |
| [**deleteWebhookSettingsWithHttpInfo**](WebhooksApi.md#deleteWebhookSettingsWithHttpInfo) | **DELETE** /v1/webhooks/settings | Delete webhook |
| [**getWebhookSettings**](WebhooksApi.md#getWebhookSettings) | **GET** /v1/webhooks/settings | List webhooks |
| [**getWebhookSettingsWithHttpInfo**](WebhooksApi.md#getWebhookSettingsWithHttpInfo) | **GET** /v1/webhooks/settings | List webhooks |
| [**testWebhook**](WebhooksApi.md#testWebhook) | **POST** /v1/webhooks/test | Send test webhook |
| [**testWebhookWithHttpInfo**](WebhooksApi.md#testWebhookWithHttpInfo) | **POST** /v1/webhooks/test | Send test webhook |
| [**updateWebhookSettings**](WebhooksApi.md#updateWebhookSettings) | **PUT** /v1/webhooks/settings | Update webhook |
| [**updateWebhookSettingsWithHttpInfo**](WebhooksApi.md#updateWebhookSettingsWithHttpInfo) | **PUT** /v1/webhooks/settings | Update webhook |



## createWebhookSettings

> UpdateWebhookSettings200Response createWebhookSettings(createWebhookSettingsRequest)

Create webhook

Create a new webhook configuration. Maximum 10 webhooks per user.  Webhooks are automatically disabled after 10 consecutive delivery failures. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhooksApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhooksApi apiInstance = new WebhooksApi(defaultClient);
        CreateWebhookSettingsRequest createWebhookSettingsRequest = new CreateWebhookSettingsRequest(); // CreateWebhookSettingsRequest | 
        try {
            UpdateWebhookSettings200Response result = apiInstance.createWebhookSettings(createWebhookSettingsRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhooksApi#createWebhookSettings");
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
| **createWebhookSettingsRequest** | [**CreateWebhookSettingsRequest**](CreateWebhookSettingsRequest.md)|  | |

### Return type

[**UpdateWebhookSettings200Response**](UpdateWebhookSettings200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook created successfully |  -  |
| **400** | Validation error or maximum webhooks reached |  -  |
| **401** | Unauthorized |  -  |

## createWebhookSettingsWithHttpInfo

> ApiResponse<UpdateWebhookSettings200Response> createWebhookSettings createWebhookSettingsWithHttpInfo(createWebhookSettingsRequest)

Create webhook

Create a new webhook configuration. Maximum 10 webhooks per user.  Webhooks are automatically disabled after 10 consecutive delivery failures. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhooksApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhooksApi apiInstance = new WebhooksApi(defaultClient);
        CreateWebhookSettingsRequest createWebhookSettingsRequest = new CreateWebhookSettingsRequest(); // CreateWebhookSettingsRequest | 
        try {
            ApiResponse<UpdateWebhookSettings200Response> response = apiInstance.createWebhookSettingsWithHttpInfo(createWebhookSettingsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhooksApi#createWebhookSettings");
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
| **createWebhookSettingsRequest** | [**CreateWebhookSettingsRequest**](CreateWebhookSettingsRequest.md)|  | |

### Return type

ApiResponse<[**UpdateWebhookSettings200Response**](UpdateWebhookSettings200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook created successfully |  -  |
| **400** | Validation error or maximum webhooks reached |  -  |
| **401** | Unauthorized |  -  |


## deleteWebhookSettings

> UpdateYoutubeDefaultPlaylist200Response deleteWebhookSettings(id)

Delete webhook

Permanently delete a webhook configuration.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhooksApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhooksApi apiInstance = new WebhooksApi(defaultClient);
        String id = "id_example"; // String | Webhook ID to delete
        try {
            UpdateYoutubeDefaultPlaylist200Response result = apiInstance.deleteWebhookSettings(id);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhooksApi#deleteWebhookSettings");
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
| **id** | **String**| Webhook ID to delete | |

### Return type

[**UpdateYoutubeDefaultPlaylist200Response**](UpdateYoutubeDefaultPlaylist200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook deleted successfully |  -  |
| **400** | Webhook ID required |  -  |
| **401** | Unauthorized |  -  |

## deleteWebhookSettingsWithHttpInfo

> ApiResponse<UpdateYoutubeDefaultPlaylist200Response> deleteWebhookSettings deleteWebhookSettingsWithHttpInfo(id)

Delete webhook

Permanently delete a webhook configuration.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhooksApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhooksApi apiInstance = new WebhooksApi(defaultClient);
        String id = "id_example"; // String | Webhook ID to delete
        try {
            ApiResponse<UpdateYoutubeDefaultPlaylist200Response> response = apiInstance.deleteWebhookSettingsWithHttpInfo(id);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhooksApi#deleteWebhookSettings");
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
| **id** | **String**| Webhook ID to delete | |

### Return type

ApiResponse<[**UpdateYoutubeDefaultPlaylist200Response**](UpdateYoutubeDefaultPlaylist200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook deleted successfully |  -  |
| **400** | Webhook ID required |  -  |
| **401** | Unauthorized |  -  |


## getWebhookSettings

> GetWebhookSettings200Response getWebhookSettings()

List webhooks

Retrieve all configured webhooks for the authenticated user. Supports up to 10 webhooks per user.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhooksApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhooksApi apiInstance = new WebhooksApi(defaultClient);
        try {
            GetWebhookSettings200Response result = apiInstance.getWebhookSettings();
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhooksApi#getWebhookSettings");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**GetWebhookSettings200Response**](GetWebhookSettings200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhooks retrieved successfully |  -  |
| **401** | Unauthorized |  -  |

## getWebhookSettingsWithHttpInfo

> ApiResponse<GetWebhookSettings200Response> getWebhookSettings getWebhookSettingsWithHttpInfo()

List webhooks

Retrieve all configured webhooks for the authenticated user. Supports up to 10 webhooks per user.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhooksApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhooksApi apiInstance = new WebhooksApi(defaultClient);
        try {
            ApiResponse<GetWebhookSettings200Response> response = apiInstance.getWebhookSettingsWithHttpInfo();
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhooksApi#getWebhookSettings");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Response headers: " + e.getResponseHeaders());
            System.err.println("Reason: " + e.getResponseBody());
            e.printStackTrace();
        }
    }
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

ApiResponse<[**GetWebhookSettings200Response**](GetWebhookSettings200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhooks retrieved successfully |  -  |
| **401** | Unauthorized |  -  |


## testWebhook

> UnpublishPost200Response testWebhook(testWebhookRequest)

Send test webhook

Send a test webhook to verify your endpoint is configured correctly. The test payload includes event: \&quot;webhook.test\&quot; to distinguish it from real events. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhooksApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhooksApi apiInstance = new WebhooksApi(defaultClient);
        TestWebhookRequest testWebhookRequest = new TestWebhookRequest(); // TestWebhookRequest | 
        try {
            UnpublishPost200Response result = apiInstance.testWebhook(testWebhookRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhooksApi#testWebhook");
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
| **testWebhookRequest** | [**TestWebhookRequest**](TestWebhookRequest.md)|  | |

### Return type

[**UnpublishPost200Response**](UnpublishPost200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Test webhook sent successfully |  -  |
| **400** | Webhook ID required |  -  |
| **401** | Unauthorized |  -  |
| **500** | Test webhook failed to deliver |  -  |

## testWebhookWithHttpInfo

> ApiResponse<UnpublishPost200Response> testWebhook testWebhookWithHttpInfo(testWebhookRequest)

Send test webhook

Send a test webhook to verify your endpoint is configured correctly. The test payload includes event: \&quot;webhook.test\&quot; to distinguish it from real events. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhooksApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhooksApi apiInstance = new WebhooksApi(defaultClient);
        TestWebhookRequest testWebhookRequest = new TestWebhookRequest(); // TestWebhookRequest | 
        try {
            ApiResponse<UnpublishPost200Response> response = apiInstance.testWebhookWithHttpInfo(testWebhookRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhooksApi#testWebhook");
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
| **testWebhookRequest** | [**TestWebhookRequest**](TestWebhookRequest.md)|  | |

### Return type

ApiResponse<[**UnpublishPost200Response**](UnpublishPost200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Test webhook sent successfully |  -  |
| **400** | Webhook ID required |  -  |
| **401** | Unauthorized |  -  |
| **500** | Test webhook failed to deliver |  -  |


## updateWebhookSettings

> UpdateWebhookSettings200Response updateWebhookSettings(updateWebhookSettingsRequest)

Update webhook

Update an existing webhook configuration. All fields except _id are optional; only provided fields will be updated.  Webhooks are automatically disabled after 10 consecutive delivery failures. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhooksApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhooksApi apiInstance = new WebhooksApi(defaultClient);
        UpdateWebhookSettingsRequest updateWebhookSettingsRequest = new UpdateWebhookSettingsRequest(); // UpdateWebhookSettingsRequest | 
        try {
            UpdateWebhookSettings200Response result = apiInstance.updateWebhookSettings(updateWebhookSettingsRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhooksApi#updateWebhookSettings");
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
| **updateWebhookSettingsRequest** | [**UpdateWebhookSettingsRequest**](UpdateWebhookSettingsRequest.md)|  | |

### Return type

[**UpdateWebhookSettings200Response**](UpdateWebhookSettings200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook updated successfully |  -  |
| **400** | Validation error or missing webhook ID |  -  |
| **401** | Unauthorized |  -  |
| **404** | Webhook not found |  -  |

## updateWebhookSettingsWithHttpInfo

> ApiResponse<UpdateWebhookSettings200Response> updateWebhookSettings updateWebhookSettingsWithHttpInfo(updateWebhookSettingsRequest)

Update webhook

Update an existing webhook configuration. All fields except _id are optional; only provided fields will be updated.  Webhooks are automatically disabled after 10 consecutive delivery failures. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhooksApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhooksApi apiInstance = new WebhooksApi(defaultClient);
        UpdateWebhookSettingsRequest updateWebhookSettingsRequest = new UpdateWebhookSettingsRequest(); // UpdateWebhookSettingsRequest | 
        try {
            ApiResponse<UpdateWebhookSettings200Response> response = apiInstance.updateWebhookSettingsWithHttpInfo(updateWebhookSettingsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhooksApi#updateWebhookSettings");
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
| **updateWebhookSettingsRequest** | [**UpdateWebhookSettingsRequest**](UpdateWebhookSettingsRequest.md)|  | |

### Return type

ApiResponse<[**UpdateWebhookSettings200Response**](UpdateWebhookSettings200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook updated successfully |  -  |
| **400** | Validation error or missing webhook ID |  -  |
| **401** | Unauthorized |  -  |
| **404** | Webhook not found |  -  |

