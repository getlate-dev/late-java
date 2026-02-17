# MessagesApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**editInboxMessage**](MessagesApi.md#editInboxMessage) | **PATCH** /v1/inbox/conversations/{conversationId}/messages/{messageId} | Edit message |
| [**editInboxMessageWithHttpInfo**](MessagesApi.md#editInboxMessageWithHttpInfo) | **PATCH** /v1/inbox/conversations/{conversationId}/messages/{messageId} | Edit message |
| [**getInboxConversation**](MessagesApi.md#getInboxConversation) | **GET** /v1/inbox/conversations/{conversationId} | Get conversation |
| [**getInboxConversationWithHttpInfo**](MessagesApi.md#getInboxConversationWithHttpInfo) | **GET** /v1/inbox/conversations/{conversationId} | Get conversation |
| [**getInboxConversationMessages**](MessagesApi.md#getInboxConversationMessages) | **GET** /v1/inbox/conversations/{conversationId}/messages | List messages |
| [**getInboxConversationMessagesWithHttpInfo**](MessagesApi.md#getInboxConversationMessagesWithHttpInfo) | **GET** /v1/inbox/conversations/{conversationId}/messages | List messages |
| [**listInboxConversations**](MessagesApi.md#listInboxConversations) | **GET** /v1/inbox/conversations | List conversations |
| [**listInboxConversationsWithHttpInfo**](MessagesApi.md#listInboxConversationsWithHttpInfo) | **GET** /v1/inbox/conversations | List conversations |
| [**sendInboxMessage**](MessagesApi.md#sendInboxMessage) | **POST** /v1/inbox/conversations/{conversationId}/messages | Send message |
| [**sendInboxMessageWithHttpInfo**](MessagesApi.md#sendInboxMessageWithHttpInfo) | **POST** /v1/inbox/conversations/{conversationId}/messages | Send message |
| [**updateInboxConversation**](MessagesApi.md#updateInboxConversation) | **PUT** /v1/inbox/conversations/{conversationId} | Update conversation status |
| [**updateInboxConversationWithHttpInfo**](MessagesApi.md#updateInboxConversationWithHttpInfo) | **PUT** /v1/inbox/conversations/{conversationId} | Update conversation status |



## editInboxMessage

> EditInboxMessage200Response editInboxMessage(conversationId, messageId, editInboxMessageRequest)

Edit message

Edit the text and/or reply markup of a previously sent Telegram message. Only supported for Telegram. Returns 400 for other platforms. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.MessagesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        MessagesApi apiInstance = new MessagesApi(defaultClient);
        String conversationId = "conversationId_example"; // String | The conversation ID
        String messageId = "messageId_example"; // String | The Telegram message ID to edit
        EditInboxMessageRequest editInboxMessageRequest = new EditInboxMessageRequest(); // EditInboxMessageRequest | 
        try {
            EditInboxMessage200Response result = apiInstance.editInboxMessage(conversationId, messageId, editInboxMessageRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling MessagesApi#editInboxMessage");
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
| **conversationId** | **String**| The conversation ID | |
| **messageId** | **String**| The Telegram message ID to edit | |
| **editInboxMessageRequest** | [**EditInboxMessageRequest**](EditInboxMessageRequest.md)|  | |

### Return type

[**EditInboxMessage200Response**](EditInboxMessage200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Message edited |  -  |
| **400** | Not supported or invalid request |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |

## editInboxMessageWithHttpInfo

> ApiResponse<EditInboxMessage200Response> editInboxMessage editInboxMessageWithHttpInfo(conversationId, messageId, editInboxMessageRequest)

Edit message

Edit the text and/or reply markup of a previously sent Telegram message. Only supported for Telegram. Returns 400 for other platforms. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.MessagesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        MessagesApi apiInstance = new MessagesApi(defaultClient);
        String conversationId = "conversationId_example"; // String | The conversation ID
        String messageId = "messageId_example"; // String | The Telegram message ID to edit
        EditInboxMessageRequest editInboxMessageRequest = new EditInboxMessageRequest(); // EditInboxMessageRequest | 
        try {
            ApiResponse<EditInboxMessage200Response> response = apiInstance.editInboxMessageWithHttpInfo(conversationId, messageId, editInboxMessageRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling MessagesApi#editInboxMessage");
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
| **conversationId** | **String**| The conversation ID | |
| **messageId** | **String**| The Telegram message ID to edit | |
| **editInboxMessageRequest** | [**EditInboxMessageRequest**](EditInboxMessageRequest.md)|  | |

### Return type

ApiResponse<[**EditInboxMessage200Response**](EditInboxMessage200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Message edited |  -  |
| **400** | Not supported or invalid request |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |


## getInboxConversation

> GetInboxConversation200Response getInboxConversation(conversationId, accountId)

Get conversation

Retrieve details and metadata for a specific conversation. Requires accountId query parameter.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.MessagesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        MessagesApi apiInstance = new MessagesApi(defaultClient);
        String conversationId = "conversationId_example"; // String | The conversation ID (id field from list conversations endpoint). This is the platform-specific conversation identifier, not an internal database ID.
        String accountId = "accountId_example"; // String | The social account ID
        try {
            GetInboxConversation200Response result = apiInstance.getInboxConversation(conversationId, accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling MessagesApi#getInboxConversation");
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
| **conversationId** | **String**| The conversation ID (id field from list conversations endpoint). This is the platform-specific conversation identifier, not an internal database ID. | |
| **accountId** | **String**| The social account ID | |

### Return type

[**GetInboxConversation200Response**](GetInboxConversation200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Conversation details |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |
| **404** | Conversation not found |  -  |

## getInboxConversationWithHttpInfo

> ApiResponse<GetInboxConversation200Response> getInboxConversation getInboxConversationWithHttpInfo(conversationId, accountId)

Get conversation

Retrieve details and metadata for a specific conversation. Requires accountId query parameter.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.MessagesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        MessagesApi apiInstance = new MessagesApi(defaultClient);
        String conversationId = "conversationId_example"; // String | The conversation ID (id field from list conversations endpoint). This is the platform-specific conversation identifier, not an internal database ID.
        String accountId = "accountId_example"; // String | The social account ID
        try {
            ApiResponse<GetInboxConversation200Response> response = apiInstance.getInboxConversationWithHttpInfo(conversationId, accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling MessagesApi#getInboxConversation");
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
| **conversationId** | **String**| The conversation ID (id field from list conversations endpoint). This is the platform-specific conversation identifier, not an internal database ID. | |
| **accountId** | **String**| The social account ID | |

### Return type

ApiResponse<[**GetInboxConversation200Response**](GetInboxConversation200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Conversation details |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |
| **404** | Conversation not found |  -  |


## getInboxConversationMessages

> GetInboxConversationMessages200Response getInboxConversationMessages(conversationId, accountId)

List messages

Fetch messages for a specific conversation. Requires accountId query parameter.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.MessagesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        MessagesApi apiInstance = new MessagesApi(defaultClient);
        String conversationId = "conversationId_example"; // String | The conversation ID (id field from list conversations endpoint). This is the platform-specific conversation identifier, not an internal database ID.
        String accountId = "accountId_example"; // String | Social account ID
        try {
            GetInboxConversationMessages200Response result = apiInstance.getInboxConversationMessages(conversationId, accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling MessagesApi#getInboxConversationMessages");
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
| **conversationId** | **String**| The conversation ID (id field from list conversations endpoint). This is the platform-specific conversation identifier, not an internal database ID. | |
| **accountId** | **String**| Social account ID | |

### Return type

[**GetInboxConversationMessages200Response**](GetInboxConversationMessages200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Messages in conversation |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |

## getInboxConversationMessagesWithHttpInfo

> ApiResponse<GetInboxConversationMessages200Response> getInboxConversationMessages getInboxConversationMessagesWithHttpInfo(conversationId, accountId)

List messages

Fetch messages for a specific conversation. Requires accountId query parameter.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.MessagesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        MessagesApi apiInstance = new MessagesApi(defaultClient);
        String conversationId = "conversationId_example"; // String | The conversation ID (id field from list conversations endpoint). This is the platform-specific conversation identifier, not an internal database ID.
        String accountId = "accountId_example"; // String | Social account ID
        try {
            ApiResponse<GetInboxConversationMessages200Response> response = apiInstance.getInboxConversationMessagesWithHttpInfo(conversationId, accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling MessagesApi#getInboxConversationMessages");
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
| **conversationId** | **String**| The conversation ID (id field from list conversations endpoint). This is the platform-specific conversation identifier, not an internal database ID. | |
| **accountId** | **String**| Social account ID | |

### Return type

ApiResponse<[**GetInboxConversationMessages200Response**](GetInboxConversationMessages200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Messages in conversation |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |


## listInboxConversations

> ListInboxConversations200Response listInboxConversations(profileId, platform, status, sortOrder, limit, cursor, accountId)

List conversations

Fetch conversations (DMs) from all connected messaging accounts in a single API call. Supports filtering by profile and platform. Results are aggregated and deduplicated. Supported platforms: Facebook, Instagram, Twitter/X, Bluesky, Reddit, Telegram. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.MessagesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        MessagesApi apiInstance = new MessagesApi(defaultClient);
        String profileId = "profileId_example"; // String | Filter by profile ID
        String platform = "facebook"; // String | Filter by platform
        String status = "active"; // String | Filter by conversation status
        String sortOrder = "asc"; // String | Sort order by updated time
        Integer limit = 50; // Integer | Maximum number of conversations to return
        String cursor = "cursor_example"; // String | Pagination cursor for next page
        String accountId = "accountId_example"; // String | Filter by specific social account ID
        try {
            ListInboxConversations200Response result = apiInstance.listInboxConversations(profileId, platform, status, sortOrder, limit, cursor, accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling MessagesApi#listInboxConversations");
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
| **profileId** | **String**| Filter by profile ID | [optional] |
| **platform** | **String**| Filter by platform | [optional] [enum: facebook, instagram, twitter, bluesky, reddit, telegram] |
| **status** | **String**| Filter by conversation status | [optional] [enum: active, archived] |
| **sortOrder** | **String**| Sort order by updated time | [optional] [default to desc] [enum: asc, desc] |
| **limit** | **Integer**| Maximum number of conversations to return | [optional] [default to 50] |
| **cursor** | **String**| Pagination cursor for next page | [optional] |
| **accountId** | **String**| Filter by specific social account ID | [optional] |

### Return type

[**ListInboxConversations200Response**](ListInboxConversations200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Aggregated conversations |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |

## listInboxConversationsWithHttpInfo

> ApiResponse<ListInboxConversations200Response> listInboxConversations listInboxConversationsWithHttpInfo(profileId, platform, status, sortOrder, limit, cursor, accountId)

List conversations

Fetch conversations (DMs) from all connected messaging accounts in a single API call. Supports filtering by profile and platform. Results are aggregated and deduplicated. Supported platforms: Facebook, Instagram, Twitter/X, Bluesky, Reddit, Telegram. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.MessagesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        MessagesApi apiInstance = new MessagesApi(defaultClient);
        String profileId = "profileId_example"; // String | Filter by profile ID
        String platform = "facebook"; // String | Filter by platform
        String status = "active"; // String | Filter by conversation status
        String sortOrder = "asc"; // String | Sort order by updated time
        Integer limit = 50; // Integer | Maximum number of conversations to return
        String cursor = "cursor_example"; // String | Pagination cursor for next page
        String accountId = "accountId_example"; // String | Filter by specific social account ID
        try {
            ApiResponse<ListInboxConversations200Response> response = apiInstance.listInboxConversationsWithHttpInfo(profileId, platform, status, sortOrder, limit, cursor, accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling MessagesApi#listInboxConversations");
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
| **profileId** | **String**| Filter by profile ID | [optional] |
| **platform** | **String**| Filter by platform | [optional] [enum: facebook, instagram, twitter, bluesky, reddit, telegram] |
| **status** | **String**| Filter by conversation status | [optional] [enum: active, archived] |
| **sortOrder** | **String**| Sort order by updated time | [optional] [default to desc] [enum: asc, desc] |
| **limit** | **Integer**| Maximum number of conversations to return | [optional] [default to 50] |
| **cursor** | **String**| Pagination cursor for next page | [optional] |
| **accountId** | **String**| Filter by specific social account ID | [optional] |

### Return type

ApiResponse<[**ListInboxConversations200Response**](ListInboxConversations200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Aggregated conversations |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |


## sendInboxMessage

> SendInboxMessage200Response sendInboxMessage(conversationId, sendInboxMessageRequest)

Send message

Send a message in a conversation. Supports text, attachments, quick replies, buttons, and message tags. Attachment and interactive message support varies by platform.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.MessagesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        MessagesApi apiInstance = new MessagesApi(defaultClient);
        String conversationId = "conversationId_example"; // String | The conversation ID (id field from list conversations endpoint). This is the platform-specific conversation identifier, not an internal database ID.
        SendInboxMessageRequest sendInboxMessageRequest = new SendInboxMessageRequest(); // SendInboxMessageRequest | 
        try {
            SendInboxMessage200Response result = apiInstance.sendInboxMessage(conversationId, sendInboxMessageRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling MessagesApi#sendInboxMessage");
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
| **conversationId** | **String**| The conversation ID (id field from list conversations endpoint). This is the platform-specific conversation identifier, not an internal database ID. | |
| **sendInboxMessageRequest** | [**SendInboxMessageRequest**](SendInboxMessageRequest.md)|  | |

### Return type

[**SendInboxMessage200Response**](SendInboxMessage200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json, multipart/form-data
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Message sent |  -  |
| **400** | Bad request (e.g., attachment not supported for platform, validation error) |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |

## sendInboxMessageWithHttpInfo

> ApiResponse<SendInboxMessage200Response> sendInboxMessage sendInboxMessageWithHttpInfo(conversationId, sendInboxMessageRequest)

Send message

Send a message in a conversation. Supports text, attachments, quick replies, buttons, and message tags. Attachment and interactive message support varies by platform.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.MessagesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        MessagesApi apiInstance = new MessagesApi(defaultClient);
        String conversationId = "conversationId_example"; // String | The conversation ID (id field from list conversations endpoint). This is the platform-specific conversation identifier, not an internal database ID.
        SendInboxMessageRequest sendInboxMessageRequest = new SendInboxMessageRequest(); // SendInboxMessageRequest | 
        try {
            ApiResponse<SendInboxMessage200Response> response = apiInstance.sendInboxMessageWithHttpInfo(conversationId, sendInboxMessageRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling MessagesApi#sendInboxMessage");
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
| **conversationId** | **String**| The conversation ID (id field from list conversations endpoint). This is the platform-specific conversation identifier, not an internal database ID. | |
| **sendInboxMessageRequest** | [**SendInboxMessageRequest**](SendInboxMessageRequest.md)|  | |

### Return type

ApiResponse<[**SendInboxMessage200Response**](SendInboxMessage200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json, multipart/form-data
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Message sent |  -  |
| **400** | Bad request (e.g., attachment not supported for platform, validation error) |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |


## updateInboxConversation

> UpdateInboxConversation200Response updateInboxConversation(conversationId, updateInboxConversationRequest)

Update conversation status

Archive or activate a conversation. Requires accountId in request body.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.MessagesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        MessagesApi apiInstance = new MessagesApi(defaultClient);
        String conversationId = "conversationId_example"; // String | The conversation ID (id field from list conversations endpoint). This is the platform-specific conversation identifier, not an internal database ID.
        UpdateInboxConversationRequest updateInboxConversationRequest = new UpdateInboxConversationRequest(); // UpdateInboxConversationRequest | 
        try {
            UpdateInboxConversation200Response result = apiInstance.updateInboxConversation(conversationId, updateInboxConversationRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling MessagesApi#updateInboxConversation");
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
| **conversationId** | **String**| The conversation ID (id field from list conversations endpoint). This is the platform-specific conversation identifier, not an internal database ID. | |
| **updateInboxConversationRequest** | [**UpdateInboxConversationRequest**](UpdateInboxConversationRequest.md)|  | |

### Return type

[**UpdateInboxConversation200Response**](UpdateInboxConversation200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Conversation updated |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |

## updateInboxConversationWithHttpInfo

> ApiResponse<UpdateInboxConversation200Response> updateInboxConversation updateInboxConversationWithHttpInfo(conversationId, updateInboxConversationRequest)

Update conversation status

Archive or activate a conversation. Requires accountId in request body.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.MessagesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        MessagesApi apiInstance = new MessagesApi(defaultClient);
        String conversationId = "conversationId_example"; // String | The conversation ID (id field from list conversations endpoint). This is the platform-specific conversation identifier, not an internal database ID.
        UpdateInboxConversationRequest updateInboxConversationRequest = new UpdateInboxConversationRequest(); // UpdateInboxConversationRequest | 
        try {
            ApiResponse<UpdateInboxConversation200Response> response = apiInstance.updateInboxConversationWithHttpInfo(conversationId, updateInboxConversationRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling MessagesApi#updateInboxConversation");
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
| **conversationId** | **String**| The conversation ID (id field from list conversations endpoint). This is the platform-specific conversation identifier, not an internal database ID. | |
| **updateInboxConversationRequest** | [**UpdateInboxConversationRequest**](UpdateInboxConversationRequest.md)|  | |

### Return type

ApiResponse<[**UpdateInboxConversation200Response**](UpdateInboxConversation200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Conversation updated |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |

