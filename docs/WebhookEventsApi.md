# WebhookEventsApi

All URIs are relative to *https://zernio.com/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**onAccountConnected**](WebhookEventsApi.md#onAccountConnected) | **POST** /account.connected | Account connected event |
| [**onAccountConnectedWithHttpInfo**](WebhookEventsApi.md#onAccountConnectedWithHttpInfo) | **POST** /account.connected | Account connected event |
| [**onAccountDisconnected**](WebhookEventsApi.md#onAccountDisconnected) | **POST** /account.disconnected | Account disconnected event |
| [**onAccountDisconnectedWithHttpInfo**](WebhookEventsApi.md#onAccountDisconnectedWithHttpInfo) | **POST** /account.disconnected | Account disconnected event |
| [**onCommentReceived**](WebhookEventsApi.md#onCommentReceived) | **POST** /comment.received | Comment received event |
| [**onCommentReceivedWithHttpInfo**](WebhookEventsApi.md#onCommentReceivedWithHttpInfo) | **POST** /comment.received | Comment received event |
| [**onMessageReceived**](WebhookEventsApi.md#onMessageReceived) | **POST** /message.received | Message received event |
| [**onMessageReceivedWithHttpInfo**](WebhookEventsApi.md#onMessageReceivedWithHttpInfo) | **POST** /message.received | Message received event |
| [**onMessageSent**](WebhookEventsApi.md#onMessageSent) | **POST** /message.sent | Message sent event |
| [**onMessageSentWithHttpInfo**](WebhookEventsApi.md#onMessageSentWithHttpInfo) | **POST** /message.sent | Message sent event |
| [**onPostCancelled**](WebhookEventsApi.md#onPostCancelled) | **POST** /post.cancelled | Post cancelled event |
| [**onPostCancelledWithHttpInfo**](WebhookEventsApi.md#onPostCancelledWithHttpInfo) | **POST** /post.cancelled | Post cancelled event |
| [**onPostFailed**](WebhookEventsApi.md#onPostFailed) | **POST** /post.failed | Post failed event |
| [**onPostFailedWithHttpInfo**](WebhookEventsApi.md#onPostFailedWithHttpInfo) | **POST** /post.failed | Post failed event |
| [**onPostPartial**](WebhookEventsApi.md#onPostPartial) | **POST** /post.partial | Post partial event |
| [**onPostPartialWithHttpInfo**](WebhookEventsApi.md#onPostPartialWithHttpInfo) | **POST** /post.partial | Post partial event |
| [**onPostPublished**](WebhookEventsApi.md#onPostPublished) | **POST** /post.published | Post published event |
| [**onPostPublishedWithHttpInfo**](WebhookEventsApi.md#onPostPublishedWithHttpInfo) | **POST** /post.published | Post published event |
| [**onPostRecycled**](WebhookEventsApi.md#onPostRecycled) | **POST** /post.recycled | Post recycled event |
| [**onPostRecycledWithHttpInfo**](WebhookEventsApi.md#onPostRecycledWithHttpInfo) | **POST** /post.recycled | Post recycled event |
| [**onPostScheduled**](WebhookEventsApi.md#onPostScheduled) | **POST** /post.scheduled | Post scheduled event |
| [**onPostScheduledWithHttpInfo**](WebhookEventsApi.md#onPostScheduledWithHttpInfo) | **POST** /post.scheduled | Post scheduled event |
| [**onWebhookTest**](WebhookEventsApi.md#onWebhookTest) | **POST** /webhook.test | Webhook test event |
| [**onWebhookTestWithHttpInfo**](WebhookEventsApi.md#onWebhookTestWithHttpInfo) | **POST** /webhook.test | Webhook test event |



## onAccountConnected

> void onAccountConnected(webhookPayloadAccountConnected)

Account connected event

Fired when a social account is successfully connected.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadAccountConnected webhookPayloadAccountConnected = new WebhookPayloadAccountConnected(); // WebhookPayloadAccountConnected | 
        try {
            apiInstance.onAccountConnected(webhookPayloadAccountConnected);
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onAccountConnected");
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
| **webhookPayloadAccountConnected** | [**WebhookPayloadAccountConnected**](WebhookPayloadAccountConnected.md)|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |

## onAccountConnectedWithHttpInfo

> ApiResponse<Void> onAccountConnected onAccountConnectedWithHttpInfo(webhookPayloadAccountConnected)

Account connected event

Fired when a social account is successfully connected.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadAccountConnected webhookPayloadAccountConnected = new WebhookPayloadAccountConnected(); // WebhookPayloadAccountConnected | 
        try {
            ApiResponse<Void> response = apiInstance.onAccountConnectedWithHttpInfo(webhookPayloadAccountConnected);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onAccountConnected");
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
| **webhookPayloadAccountConnected** | [**WebhookPayloadAccountConnected**](WebhookPayloadAccountConnected.md)|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |


## onAccountDisconnected

> void onAccountDisconnected(webhookPayloadAccountDisconnected)

Account disconnected event

Fired when a connected social account becomes disconnected.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadAccountDisconnected webhookPayloadAccountDisconnected = new WebhookPayloadAccountDisconnected(); // WebhookPayloadAccountDisconnected | 
        try {
            apiInstance.onAccountDisconnected(webhookPayloadAccountDisconnected);
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onAccountDisconnected");
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
| **webhookPayloadAccountDisconnected** | [**WebhookPayloadAccountDisconnected**](WebhookPayloadAccountDisconnected.md)|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |

## onAccountDisconnectedWithHttpInfo

> ApiResponse<Void> onAccountDisconnected onAccountDisconnectedWithHttpInfo(webhookPayloadAccountDisconnected)

Account disconnected event

Fired when a connected social account becomes disconnected.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadAccountDisconnected webhookPayloadAccountDisconnected = new WebhookPayloadAccountDisconnected(); // WebhookPayloadAccountDisconnected | 
        try {
            ApiResponse<Void> response = apiInstance.onAccountDisconnectedWithHttpInfo(webhookPayloadAccountDisconnected);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onAccountDisconnected");
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
| **webhookPayloadAccountDisconnected** | [**WebhookPayloadAccountDisconnected**](WebhookPayloadAccountDisconnected.md)|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |


## onCommentReceived

> void onCommentReceived(webhookPayloadComment)

Comment received event

Fired when a new comment is received on a tracked post.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadComment webhookPayloadComment = new WebhookPayloadComment(); // WebhookPayloadComment | 
        try {
            apiInstance.onCommentReceived(webhookPayloadComment);
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onCommentReceived");
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
| **webhookPayloadComment** | [**WebhookPayloadComment**](WebhookPayloadComment.md)|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |

## onCommentReceivedWithHttpInfo

> ApiResponse<Void> onCommentReceived onCommentReceivedWithHttpInfo(webhookPayloadComment)

Comment received event

Fired when a new comment is received on a tracked post.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadComment webhookPayloadComment = new WebhookPayloadComment(); // WebhookPayloadComment | 
        try {
            ApiResponse<Void> response = apiInstance.onCommentReceivedWithHttpInfo(webhookPayloadComment);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onCommentReceived");
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
| **webhookPayloadComment** | [**WebhookPayloadComment**](WebhookPayloadComment.md)|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |


## onMessageReceived

> void onMessageReceived(webhookPayloadMessage)

Message received event

Fired when a new inbox message is received.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadMessage webhookPayloadMessage = new WebhookPayloadMessage(); // WebhookPayloadMessage | 
        try {
            apiInstance.onMessageReceived(webhookPayloadMessage);
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onMessageReceived");
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
| **webhookPayloadMessage** | [**WebhookPayloadMessage**](WebhookPayloadMessage.md)|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |

## onMessageReceivedWithHttpInfo

> ApiResponse<Void> onMessageReceived onMessageReceivedWithHttpInfo(webhookPayloadMessage)

Message received event

Fired when a new inbox message is received.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadMessage webhookPayloadMessage = new WebhookPayloadMessage(); // WebhookPayloadMessage | 
        try {
            ApiResponse<Void> response = apiInstance.onMessageReceivedWithHttpInfo(webhookPayloadMessage);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onMessageReceived");
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
| **webhookPayloadMessage** | [**WebhookPayloadMessage**](WebhookPayloadMessage.md)|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |


## onMessageSent

> void onMessageSent(webhookPayloadMessageSent)

Message sent event

Fired when a message is sent via the API.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadMessageSent webhookPayloadMessageSent = new WebhookPayloadMessageSent(); // WebhookPayloadMessageSent | 
        try {
            apiInstance.onMessageSent(webhookPayloadMessageSent);
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onMessageSent");
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
| **webhookPayloadMessageSent** | [**WebhookPayloadMessageSent**](WebhookPayloadMessageSent.md)|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |

## onMessageSentWithHttpInfo

> ApiResponse<Void> onMessageSent onMessageSentWithHttpInfo(webhookPayloadMessageSent)

Message sent event

Fired when a message is sent via the API.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadMessageSent webhookPayloadMessageSent = new WebhookPayloadMessageSent(); // WebhookPayloadMessageSent | 
        try {
            ApiResponse<Void> response = apiInstance.onMessageSentWithHttpInfo(webhookPayloadMessageSent);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onMessageSent");
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
| **webhookPayloadMessageSent** | [**WebhookPayloadMessageSent**](WebhookPayloadMessageSent.md)|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |


## onPostCancelled

> void onPostCancelled(webhookPayloadPost)

Post cancelled event

Fired when a post publishing job is cancelled.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadPost webhookPayloadPost = new WebhookPayloadPost(); // WebhookPayloadPost | 
        try {
            apiInstance.onPostCancelled(webhookPayloadPost);
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onPostCancelled");
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
| **webhookPayloadPost** | [**WebhookPayloadPost**](WebhookPayloadPost.md)|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |

## onPostCancelledWithHttpInfo

> ApiResponse<Void> onPostCancelled onPostCancelledWithHttpInfo(webhookPayloadPost)

Post cancelled event

Fired when a post publishing job is cancelled.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadPost webhookPayloadPost = new WebhookPayloadPost(); // WebhookPayloadPost | 
        try {
            ApiResponse<Void> response = apiInstance.onPostCancelledWithHttpInfo(webhookPayloadPost);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onPostCancelled");
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
| **webhookPayloadPost** | [**WebhookPayloadPost**](WebhookPayloadPost.md)|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |


## onPostFailed

> void onPostFailed(webhookPayloadPost)

Post failed event

Fired when a post fails to publish on all target platforms.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadPost webhookPayloadPost = new WebhookPayloadPost(); // WebhookPayloadPost | 
        try {
            apiInstance.onPostFailed(webhookPayloadPost);
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onPostFailed");
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
| **webhookPayloadPost** | [**WebhookPayloadPost**](WebhookPayloadPost.md)|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |

## onPostFailedWithHttpInfo

> ApiResponse<Void> onPostFailed onPostFailedWithHttpInfo(webhookPayloadPost)

Post failed event

Fired when a post fails to publish on all target platforms.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadPost webhookPayloadPost = new WebhookPayloadPost(); // WebhookPayloadPost | 
        try {
            ApiResponse<Void> response = apiInstance.onPostFailedWithHttpInfo(webhookPayloadPost);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onPostFailed");
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
| **webhookPayloadPost** | [**WebhookPayloadPost**](WebhookPayloadPost.md)|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |


## onPostPartial

> void onPostPartial(webhookPayloadPost)

Post partial event

Fired when a post publishes on some platforms and fails on others.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadPost webhookPayloadPost = new WebhookPayloadPost(); // WebhookPayloadPost | 
        try {
            apiInstance.onPostPartial(webhookPayloadPost);
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onPostPartial");
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
| **webhookPayloadPost** | [**WebhookPayloadPost**](WebhookPayloadPost.md)|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |

## onPostPartialWithHttpInfo

> ApiResponse<Void> onPostPartial onPostPartialWithHttpInfo(webhookPayloadPost)

Post partial event

Fired when a post publishes on some platforms and fails on others.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadPost webhookPayloadPost = new WebhookPayloadPost(); // WebhookPayloadPost | 
        try {
            ApiResponse<Void> response = apiInstance.onPostPartialWithHttpInfo(webhookPayloadPost);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onPostPartial");
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
| **webhookPayloadPost** | [**WebhookPayloadPost**](WebhookPayloadPost.md)|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |


## onPostPublished

> void onPostPublished(webhookPayloadPost)

Post published event

Fired when a post is successfully published.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadPost webhookPayloadPost = new WebhookPayloadPost(); // WebhookPayloadPost | 
        try {
            apiInstance.onPostPublished(webhookPayloadPost);
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onPostPublished");
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
| **webhookPayloadPost** | [**WebhookPayloadPost**](WebhookPayloadPost.md)|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |

## onPostPublishedWithHttpInfo

> ApiResponse<Void> onPostPublished onPostPublishedWithHttpInfo(webhookPayloadPost)

Post published event

Fired when a post is successfully published.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadPost webhookPayloadPost = new WebhookPayloadPost(); // WebhookPayloadPost | 
        try {
            ApiResponse<Void> response = apiInstance.onPostPublishedWithHttpInfo(webhookPayloadPost);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onPostPublished");
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
| **webhookPayloadPost** | [**WebhookPayloadPost**](WebhookPayloadPost.md)|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |


## onPostRecycled

> void onPostRecycled(webhookPayloadPost)

Post recycled event

Fired when a post is recycled (cloned and re-scheduled for publishing).

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadPost webhookPayloadPost = new WebhookPayloadPost(); // WebhookPayloadPost | 
        try {
            apiInstance.onPostRecycled(webhookPayloadPost);
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onPostRecycled");
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
| **webhookPayloadPost** | [**WebhookPayloadPost**](WebhookPayloadPost.md)|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |

## onPostRecycledWithHttpInfo

> ApiResponse<Void> onPostRecycled onPostRecycledWithHttpInfo(webhookPayloadPost)

Post recycled event

Fired when a post is recycled (cloned and re-scheduled for publishing).

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadPost webhookPayloadPost = new WebhookPayloadPost(); // WebhookPayloadPost | 
        try {
            ApiResponse<Void> response = apiInstance.onPostRecycledWithHttpInfo(webhookPayloadPost);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onPostRecycled");
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
| **webhookPayloadPost** | [**WebhookPayloadPost**](WebhookPayloadPost.md)|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |


## onPostScheduled

> void onPostScheduled(webhookPayloadPost)

Post scheduled event

Fired when a post is created and scheduled for publishing.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadPost webhookPayloadPost = new WebhookPayloadPost(); // WebhookPayloadPost | 
        try {
            apiInstance.onPostScheduled(webhookPayloadPost);
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onPostScheduled");
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
| **webhookPayloadPost** | [**WebhookPayloadPost**](WebhookPayloadPost.md)|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |

## onPostScheduledWithHttpInfo

> ApiResponse<Void> onPostScheduled onPostScheduledWithHttpInfo(webhookPayloadPost)

Post scheduled event

Fired when a post is created and scheduled for publishing.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadPost webhookPayloadPost = new WebhookPayloadPost(); // WebhookPayloadPost | 
        try {
            ApiResponse<Void> response = apiInstance.onPostScheduledWithHttpInfo(webhookPayloadPost);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onPostScheduled");
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
| **webhookPayloadPost** | [**WebhookPayloadPost**](WebhookPayloadPost.md)|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |


## onWebhookTest

> void onWebhookTest(webhookPayloadTest)

Webhook test event

Fired when sending a test webhook to verify the endpoint configuration.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadTest webhookPayloadTest = new WebhookPayloadTest(); // WebhookPayloadTest | 
        try {
            apiInstance.onWebhookTest(webhookPayloadTest);
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onWebhookTest");
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
| **webhookPayloadTest** | [**WebhookPayloadTest**](WebhookPayloadTest.md)|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |

## onWebhookTestWithHttpInfo

> ApiResponse<Void> onWebhookTest onWebhookTestWithHttpInfo(webhookPayloadTest)

Webhook test event

Fired when sending a test webhook to verify the endpoint configuration.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WebhookEventsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WebhookEventsApi apiInstance = new WebhookEventsApi(defaultClient);
        WebhookPayloadTest webhookPayloadTest = new WebhookPayloadTest(); // WebhookPayloadTest | 
        try {
            ApiResponse<Void> response = apiInstance.onWebhookTestWithHttpInfo(webhookPayloadTest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling WebhookEventsApi#onWebhookTest");
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
| **webhookPayloadTest** | [**WebhookPayloadTest**](WebhookPayloadTest.md)|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |

