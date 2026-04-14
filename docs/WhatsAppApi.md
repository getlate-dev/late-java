# WhatsAppApi

All URIs are relative to *https://zernio.com/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addWhatsAppGroupParticipants**](WhatsAppApi.md#addWhatsAppGroupParticipants) | **POST** /v1/whatsapp/wa-groups/{groupId}/participants | Add participants |
| [**addWhatsAppGroupParticipantsWithHttpInfo**](WhatsAppApi.md#addWhatsAppGroupParticipantsWithHttpInfo) | **POST** /v1/whatsapp/wa-groups/{groupId}/participants | Add participants |
| [**approveWhatsAppGroupJoinRequests**](WhatsAppApi.md#approveWhatsAppGroupJoinRequests) | **POST** /v1/whatsapp/wa-groups/{groupId}/join-requests | Approve join requests |
| [**approveWhatsAppGroupJoinRequestsWithHttpInfo**](WhatsAppApi.md#approveWhatsAppGroupJoinRequestsWithHttpInfo) | **POST** /v1/whatsapp/wa-groups/{groupId}/join-requests | Approve join requests |
| [**createWhatsAppGroupChat**](WhatsAppApi.md#createWhatsAppGroupChat) | **POST** /v1/whatsapp/wa-groups | Create group |
| [**createWhatsAppGroupChatWithHttpInfo**](WhatsAppApi.md#createWhatsAppGroupChatWithHttpInfo) | **POST** /v1/whatsapp/wa-groups | Create group |
| [**createWhatsAppGroupInviteLink**](WhatsAppApi.md#createWhatsAppGroupInviteLink) | **POST** /v1/whatsapp/wa-groups/{groupId}/invite-link | Create invite link |
| [**createWhatsAppGroupInviteLinkWithHttpInfo**](WhatsAppApi.md#createWhatsAppGroupInviteLinkWithHttpInfo) | **POST** /v1/whatsapp/wa-groups/{groupId}/invite-link | Create invite link |
| [**createWhatsAppTemplate**](WhatsAppApi.md#createWhatsAppTemplate) | **POST** /v1/whatsapp/templates | Create template |
| [**createWhatsAppTemplateWithHttpInfo**](WhatsAppApi.md#createWhatsAppTemplateWithHttpInfo) | **POST** /v1/whatsapp/templates | Create template |
| [**deleteWhatsAppGroupChat**](WhatsAppApi.md#deleteWhatsAppGroupChat) | **DELETE** /v1/whatsapp/wa-groups/{groupId} | Delete group |
| [**deleteWhatsAppGroupChatWithHttpInfo**](WhatsAppApi.md#deleteWhatsAppGroupChatWithHttpInfo) | **DELETE** /v1/whatsapp/wa-groups/{groupId} | Delete group |
| [**deleteWhatsAppTemplate**](WhatsAppApi.md#deleteWhatsAppTemplate) | **DELETE** /v1/whatsapp/templates/{templateName} | Delete template |
| [**deleteWhatsAppTemplateWithHttpInfo**](WhatsAppApi.md#deleteWhatsAppTemplateWithHttpInfo) | **DELETE** /v1/whatsapp/templates/{templateName} | Delete template |
| [**getWhatsAppBusinessProfile**](WhatsAppApi.md#getWhatsAppBusinessProfile) | **GET** /v1/whatsapp/business-profile | Get business profile |
| [**getWhatsAppBusinessProfileWithHttpInfo**](WhatsAppApi.md#getWhatsAppBusinessProfileWithHttpInfo) | **GET** /v1/whatsapp/business-profile | Get business profile |
| [**getWhatsAppDisplayName**](WhatsAppApi.md#getWhatsAppDisplayName) | **GET** /v1/whatsapp/business-profile/display-name | Get display name and review status |
| [**getWhatsAppDisplayNameWithHttpInfo**](WhatsAppApi.md#getWhatsAppDisplayNameWithHttpInfo) | **GET** /v1/whatsapp/business-profile/display-name | Get display name and review status |
| [**getWhatsAppGroupChat**](WhatsAppApi.md#getWhatsAppGroupChat) | **GET** /v1/whatsapp/wa-groups/{groupId} | Get group info |
| [**getWhatsAppGroupChatWithHttpInfo**](WhatsAppApi.md#getWhatsAppGroupChatWithHttpInfo) | **GET** /v1/whatsapp/wa-groups/{groupId} | Get group info |
| [**getWhatsAppTemplate**](WhatsAppApi.md#getWhatsAppTemplate) | **GET** /v1/whatsapp/templates/{templateName} | Get template |
| [**getWhatsAppTemplateWithHttpInfo**](WhatsAppApi.md#getWhatsAppTemplateWithHttpInfo) | **GET** /v1/whatsapp/templates/{templateName} | Get template |
| [**getWhatsAppTemplates**](WhatsAppApi.md#getWhatsAppTemplates) | **GET** /v1/whatsapp/templates | List templates |
| [**getWhatsAppTemplatesWithHttpInfo**](WhatsAppApi.md#getWhatsAppTemplatesWithHttpInfo) | **GET** /v1/whatsapp/templates | List templates |
| [**listWhatsAppGroupChats**](WhatsAppApi.md#listWhatsAppGroupChats) | **GET** /v1/whatsapp/wa-groups | List active groups |
| [**listWhatsAppGroupChatsWithHttpInfo**](WhatsAppApi.md#listWhatsAppGroupChatsWithHttpInfo) | **GET** /v1/whatsapp/wa-groups | List active groups |
| [**listWhatsAppGroupJoinRequests**](WhatsAppApi.md#listWhatsAppGroupJoinRequests) | **GET** /v1/whatsapp/wa-groups/{groupId}/join-requests | List join requests |
| [**listWhatsAppGroupJoinRequestsWithHttpInfo**](WhatsAppApi.md#listWhatsAppGroupJoinRequestsWithHttpInfo) | **GET** /v1/whatsapp/wa-groups/{groupId}/join-requests | List join requests |
| [**rejectWhatsAppGroupJoinRequests**](WhatsAppApi.md#rejectWhatsAppGroupJoinRequests) | **DELETE** /v1/whatsapp/wa-groups/{groupId}/join-requests | Reject join requests |
| [**rejectWhatsAppGroupJoinRequestsWithHttpInfo**](WhatsAppApi.md#rejectWhatsAppGroupJoinRequestsWithHttpInfo) | **DELETE** /v1/whatsapp/wa-groups/{groupId}/join-requests | Reject join requests |
| [**removeWhatsAppGroupParticipants**](WhatsAppApi.md#removeWhatsAppGroupParticipants) | **DELETE** /v1/whatsapp/wa-groups/{groupId}/participants | Remove participants |
| [**removeWhatsAppGroupParticipantsWithHttpInfo**](WhatsAppApi.md#removeWhatsAppGroupParticipantsWithHttpInfo) | **DELETE** /v1/whatsapp/wa-groups/{groupId}/participants | Remove participants |
| [**updateWhatsAppBusinessProfile**](WhatsAppApi.md#updateWhatsAppBusinessProfile) | **POST** /v1/whatsapp/business-profile | Update business profile |
| [**updateWhatsAppBusinessProfileWithHttpInfo**](WhatsAppApi.md#updateWhatsAppBusinessProfileWithHttpInfo) | **POST** /v1/whatsapp/business-profile | Update business profile |
| [**updateWhatsAppDisplayName**](WhatsAppApi.md#updateWhatsAppDisplayName) | **POST** /v1/whatsapp/business-profile/display-name | Request display name change |
| [**updateWhatsAppDisplayNameWithHttpInfo**](WhatsAppApi.md#updateWhatsAppDisplayNameWithHttpInfo) | **POST** /v1/whatsapp/business-profile/display-name | Request display name change |
| [**updateWhatsAppGroupChat**](WhatsAppApi.md#updateWhatsAppGroupChat) | **POST** /v1/whatsapp/wa-groups/{groupId} | Update group settings |
| [**updateWhatsAppGroupChatWithHttpInfo**](WhatsAppApi.md#updateWhatsAppGroupChatWithHttpInfo) | **POST** /v1/whatsapp/wa-groups/{groupId} | Update group settings |
| [**updateWhatsAppTemplate**](WhatsAppApi.md#updateWhatsAppTemplate) | **PATCH** /v1/whatsapp/templates/{templateName} | Update template |
| [**updateWhatsAppTemplateWithHttpInfo**](WhatsAppApi.md#updateWhatsAppTemplateWithHttpInfo) | **PATCH** /v1/whatsapp/templates/{templateName} | Update template |
| [**uploadWhatsAppProfilePhoto**](WhatsAppApi.md#uploadWhatsAppProfilePhoto) | **POST** /v1/whatsapp/business-profile/photo | Upload profile picture |
| [**uploadWhatsAppProfilePhotoWithHttpInfo**](WhatsAppApi.md#uploadWhatsAppProfilePhotoWithHttpInfo) | **POST** /v1/whatsapp/business-profile/photo | Upload profile picture |



## addWhatsAppGroupParticipants

> UnpublishPost200Response addWhatsAppGroupParticipants(groupId, accountId, addWhatsAppGroupParticipantsRequest)

Add participants

Add participants to a WhatsApp group. Maximum 8 participants per request. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String groupId = "groupId_example"; // String | Group ID
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        AddWhatsAppGroupParticipantsRequest addWhatsAppGroupParticipantsRequest = new AddWhatsAppGroupParticipantsRequest(); // AddWhatsAppGroupParticipantsRequest | 
        try {
            UnpublishPost200Response result = apiInstance.addWhatsAppGroupParticipants(groupId, accountId, addWhatsAppGroupParticipantsRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#addWhatsAppGroupParticipants");
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
| **groupId** | **String**| Group ID | |
| **accountId** | **String**| WhatsApp social account ID | |
| **addWhatsAppGroupParticipantsRequest** | [**AddWhatsAppGroupParticipantsRequest**](AddWhatsAppGroupParticipantsRequest.md)|  | |

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
| **200** | Participants added |  -  |
| **401** | Unauthorized |  -  |

## addWhatsAppGroupParticipantsWithHttpInfo

> ApiResponse<UnpublishPost200Response> addWhatsAppGroupParticipants addWhatsAppGroupParticipantsWithHttpInfo(groupId, accountId, addWhatsAppGroupParticipantsRequest)

Add participants

Add participants to a WhatsApp group. Maximum 8 participants per request. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String groupId = "groupId_example"; // String | Group ID
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        AddWhatsAppGroupParticipantsRequest addWhatsAppGroupParticipantsRequest = new AddWhatsAppGroupParticipantsRequest(); // AddWhatsAppGroupParticipantsRequest | 
        try {
            ApiResponse<UnpublishPost200Response> response = apiInstance.addWhatsAppGroupParticipantsWithHttpInfo(groupId, accountId, addWhatsAppGroupParticipantsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#addWhatsAppGroupParticipants");
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
| **groupId** | **String**| Group ID | |
| **accountId** | **String**| WhatsApp social account ID | |
| **addWhatsAppGroupParticipantsRequest** | [**AddWhatsAppGroupParticipantsRequest**](AddWhatsAppGroupParticipantsRequest.md)|  | |

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
| **200** | Participants added |  -  |
| **401** | Unauthorized |  -  |


## approveWhatsAppGroupJoinRequests

> UnpublishPost200Response approveWhatsAppGroupJoinRequests(groupId, accountId, approveWhatsAppGroupJoinRequestsRequest)

Approve join requests

Approve pending join requests for a WhatsApp group. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String groupId = "groupId_example"; // String | Group ID
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        ApproveWhatsAppGroupJoinRequestsRequest approveWhatsAppGroupJoinRequestsRequest = new ApproveWhatsAppGroupJoinRequestsRequest(); // ApproveWhatsAppGroupJoinRequestsRequest | 
        try {
            UnpublishPost200Response result = apiInstance.approveWhatsAppGroupJoinRequests(groupId, accountId, approveWhatsAppGroupJoinRequestsRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#approveWhatsAppGroupJoinRequests");
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
| **groupId** | **String**| Group ID | |
| **accountId** | **String**| WhatsApp social account ID | |
| **approveWhatsAppGroupJoinRequestsRequest** | [**ApproveWhatsAppGroupJoinRequestsRequest**](ApproveWhatsAppGroupJoinRequestsRequest.md)|  | |

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
| **200** | Requests approved |  -  |
| **401** | Unauthorized |  -  |

## approveWhatsAppGroupJoinRequestsWithHttpInfo

> ApiResponse<UnpublishPost200Response> approveWhatsAppGroupJoinRequests approveWhatsAppGroupJoinRequestsWithHttpInfo(groupId, accountId, approveWhatsAppGroupJoinRequestsRequest)

Approve join requests

Approve pending join requests for a WhatsApp group. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String groupId = "groupId_example"; // String | Group ID
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        ApproveWhatsAppGroupJoinRequestsRequest approveWhatsAppGroupJoinRequestsRequest = new ApproveWhatsAppGroupJoinRequestsRequest(); // ApproveWhatsAppGroupJoinRequestsRequest | 
        try {
            ApiResponse<UnpublishPost200Response> response = apiInstance.approveWhatsAppGroupJoinRequestsWithHttpInfo(groupId, accountId, approveWhatsAppGroupJoinRequestsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#approveWhatsAppGroupJoinRequests");
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
| **groupId** | **String**| Group ID | |
| **accountId** | **String**| WhatsApp social account ID | |
| **approveWhatsAppGroupJoinRequestsRequest** | [**ApproveWhatsAppGroupJoinRequestsRequest**](ApproveWhatsAppGroupJoinRequestsRequest.md)|  | |

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
| **200** | Requests approved |  -  |
| **401** | Unauthorized |  -  |


## createWhatsAppGroupChat

> CreateWhatsAppGroupChat201Response createWhatsAppGroupChat(createWhatsAppGroupChatRequest)

Create group

Create a new WhatsApp group chat. Returns the group ID and optionally an invite link. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        CreateWhatsAppGroupChatRequest createWhatsAppGroupChatRequest = new CreateWhatsAppGroupChatRequest(); // CreateWhatsAppGroupChatRequest | 
        try {
            CreateWhatsAppGroupChat201Response result = apiInstance.createWhatsAppGroupChat(createWhatsAppGroupChatRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#createWhatsAppGroupChat");
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
| **createWhatsAppGroupChatRequest** | [**CreateWhatsAppGroupChatRequest**](CreateWhatsAppGroupChatRequest.md)|  | |

### Return type

[**CreateWhatsAppGroupChat201Response**](CreateWhatsAppGroupChat201Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Group created |  -  |
| **401** | Unauthorized |  -  |

## createWhatsAppGroupChatWithHttpInfo

> ApiResponse<CreateWhatsAppGroupChat201Response> createWhatsAppGroupChat createWhatsAppGroupChatWithHttpInfo(createWhatsAppGroupChatRequest)

Create group

Create a new WhatsApp group chat. Returns the group ID and optionally an invite link. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        CreateWhatsAppGroupChatRequest createWhatsAppGroupChatRequest = new CreateWhatsAppGroupChatRequest(); // CreateWhatsAppGroupChatRequest | 
        try {
            ApiResponse<CreateWhatsAppGroupChat201Response> response = apiInstance.createWhatsAppGroupChatWithHttpInfo(createWhatsAppGroupChatRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#createWhatsAppGroupChat");
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
| **createWhatsAppGroupChatRequest** | [**CreateWhatsAppGroupChatRequest**](CreateWhatsAppGroupChatRequest.md)|  | |

### Return type

ApiResponse<[**CreateWhatsAppGroupChat201Response**](CreateWhatsAppGroupChat201Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Group created |  -  |
| **401** | Unauthorized |  -  |


## createWhatsAppGroupInviteLink

> CreateWhatsAppGroupInviteLink200Response createWhatsAppGroupInviteLink(groupId, accountId)

Create invite link

Create a new invite link for a WhatsApp group. The previous link is revoked. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String groupId = "groupId_example"; // String | Group ID
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        try {
            CreateWhatsAppGroupInviteLink200Response result = apiInstance.createWhatsAppGroupInviteLink(groupId, accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#createWhatsAppGroupInviteLink");
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
| **groupId** | **String**| Group ID | |
| **accountId** | **String**| WhatsApp social account ID | |

### Return type

[**CreateWhatsAppGroupInviteLink200Response**](CreateWhatsAppGroupInviteLink200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Invite link created |  -  |
| **401** | Unauthorized |  -  |

## createWhatsAppGroupInviteLinkWithHttpInfo

> ApiResponse<CreateWhatsAppGroupInviteLink200Response> createWhatsAppGroupInviteLink createWhatsAppGroupInviteLinkWithHttpInfo(groupId, accountId)

Create invite link

Create a new invite link for a WhatsApp group. The previous link is revoked. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String groupId = "groupId_example"; // String | Group ID
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        try {
            ApiResponse<CreateWhatsAppGroupInviteLink200Response> response = apiInstance.createWhatsAppGroupInviteLinkWithHttpInfo(groupId, accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#createWhatsAppGroupInviteLink");
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
| **groupId** | **String**| Group ID | |
| **accountId** | **String**| WhatsApp social account ID | |

### Return type

ApiResponse<[**CreateWhatsAppGroupInviteLink200Response**](CreateWhatsAppGroupInviteLink200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Invite link created |  -  |
| **401** | Unauthorized |  -  |


## createWhatsAppTemplate

> CreateWhatsAppTemplate200Response createWhatsAppTemplate(createWhatsAppTemplateRequest)

Create template

Create a new message template. Supports two modes:  **Custom template:** Provide &#x60;components&#x60; with your own content. Submitted to Meta for review (can take up to 24h).  **Library template:** Provide &#x60;library_template_name&#x60; instead of &#x60;components&#x60; to use a pre-built template from Meta&#39;s template library. Library templates are **pre-approved** (no review wait). You can optionally customize parameters and buttons via &#x60;library_template_body_inputs&#x60; and &#x60;library_template_button_inputs&#x60;.  Browse available library templates at: https://business.facebook.com/wa/manage/message-templates/ 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        CreateWhatsAppTemplateRequest createWhatsAppTemplateRequest = new CreateWhatsAppTemplateRequest(); // CreateWhatsAppTemplateRequest | 
        try {
            CreateWhatsAppTemplate200Response result = apiInstance.createWhatsAppTemplate(createWhatsAppTemplateRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#createWhatsAppTemplate");
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
| **createWhatsAppTemplateRequest** | [**CreateWhatsAppTemplateRequest**](CreateWhatsAppTemplateRequest.md)|  | |

### Return type

[**CreateWhatsAppTemplate200Response**](CreateWhatsAppTemplate200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Template created (pre-approved for library templates, pending review for custom) |  -  |
| **400** | Validation error (invalid name format |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |

## createWhatsAppTemplateWithHttpInfo

> ApiResponse<CreateWhatsAppTemplate200Response> createWhatsAppTemplate createWhatsAppTemplateWithHttpInfo(createWhatsAppTemplateRequest)

Create template

Create a new message template. Supports two modes:  **Custom template:** Provide &#x60;components&#x60; with your own content. Submitted to Meta for review (can take up to 24h).  **Library template:** Provide &#x60;library_template_name&#x60; instead of &#x60;components&#x60; to use a pre-built template from Meta&#39;s template library. Library templates are **pre-approved** (no review wait). You can optionally customize parameters and buttons via &#x60;library_template_body_inputs&#x60; and &#x60;library_template_button_inputs&#x60;.  Browse available library templates at: https://business.facebook.com/wa/manage/message-templates/ 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        CreateWhatsAppTemplateRequest createWhatsAppTemplateRequest = new CreateWhatsAppTemplateRequest(); // CreateWhatsAppTemplateRequest | 
        try {
            ApiResponse<CreateWhatsAppTemplate200Response> response = apiInstance.createWhatsAppTemplateWithHttpInfo(createWhatsAppTemplateRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#createWhatsAppTemplate");
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
| **createWhatsAppTemplateRequest** | [**CreateWhatsAppTemplateRequest**](CreateWhatsAppTemplateRequest.md)|  | |

### Return type

ApiResponse<[**CreateWhatsAppTemplate200Response**](CreateWhatsAppTemplate200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Template created (pre-approved for library templates, pending review for custom) |  -  |
| **400** | Validation error (invalid name format |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |


## deleteWhatsAppGroupChat

> UnpublishPost200Response deleteWhatsAppGroupChat(groupId, accountId)

Delete group

Delete a WhatsApp group and remove all participants. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String groupId = "groupId_example"; // String | Group ID
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        try {
            UnpublishPost200Response result = apiInstance.deleteWhatsAppGroupChat(groupId, accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#deleteWhatsAppGroupChat");
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
| **groupId** | **String**| Group ID | |
| **accountId** | **String**| WhatsApp social account ID | |

### Return type

[**UnpublishPost200Response**](UnpublishPost200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Group deleted |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## deleteWhatsAppGroupChatWithHttpInfo

> ApiResponse<UnpublishPost200Response> deleteWhatsAppGroupChat deleteWhatsAppGroupChatWithHttpInfo(groupId, accountId)

Delete group

Delete a WhatsApp group and remove all participants. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String groupId = "groupId_example"; // String | Group ID
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        try {
            ApiResponse<UnpublishPost200Response> response = apiInstance.deleteWhatsAppGroupChatWithHttpInfo(groupId, accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#deleteWhatsAppGroupChat");
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
| **groupId** | **String**| Group ID | |
| **accountId** | **String**| WhatsApp social account ID | |

### Return type

ApiResponse<[**UnpublishPost200Response**](UnpublishPost200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Group deleted |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## deleteWhatsAppTemplate

> UnpublishPost200Response deleteWhatsAppTemplate(templateName, accountId)

Delete template

Permanently delete a message template by name. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String templateName = "templateName_example"; // String | Template name
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        try {
            UnpublishPost200Response result = apiInstance.deleteWhatsAppTemplate(templateName, accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#deleteWhatsAppTemplate");
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
| **templateName** | **String**| Template name | |
| **accountId** | **String**| WhatsApp social account ID | |

### Return type

[**UnpublishPost200Response**](UnpublishPost200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Template deleted successfully |  -  |
| **400** | accountId or template name is required |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## deleteWhatsAppTemplateWithHttpInfo

> ApiResponse<UnpublishPost200Response> deleteWhatsAppTemplate deleteWhatsAppTemplateWithHttpInfo(templateName, accountId)

Delete template

Permanently delete a message template by name. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String templateName = "templateName_example"; // String | Template name
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        try {
            ApiResponse<UnpublishPost200Response> response = apiInstance.deleteWhatsAppTemplateWithHttpInfo(templateName, accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#deleteWhatsAppTemplate");
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
| **templateName** | **String**| Template name | |
| **accountId** | **String**| WhatsApp social account ID | |

### Return type

ApiResponse<[**UnpublishPost200Response**](UnpublishPost200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Template deleted successfully |  -  |
| **400** | accountId or template name is required |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## getWhatsAppBusinessProfile

> GetWhatsAppBusinessProfile200Response getWhatsAppBusinessProfile(accountId)

Get business profile

Retrieve the WhatsApp Business profile for the account (about, address, description, email, websites, etc.). 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        try {
            GetWhatsAppBusinessProfile200Response result = apiInstance.getWhatsAppBusinessProfile(accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppBusinessProfile");
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
| **accountId** | **String**| WhatsApp social account ID | |

### Return type

[**GetWhatsAppBusinessProfile200Response**](GetWhatsAppBusinessProfile200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Business profile retrieved successfully |  -  |
| **400** | accountId is required or phone number ID not found |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |

## getWhatsAppBusinessProfileWithHttpInfo

> ApiResponse<GetWhatsAppBusinessProfile200Response> getWhatsAppBusinessProfile getWhatsAppBusinessProfileWithHttpInfo(accountId)

Get business profile

Retrieve the WhatsApp Business profile for the account (about, address, description, email, websites, etc.). 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        try {
            ApiResponse<GetWhatsAppBusinessProfile200Response> response = apiInstance.getWhatsAppBusinessProfileWithHttpInfo(accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppBusinessProfile");
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
| **accountId** | **String**| WhatsApp social account ID | |

### Return type

ApiResponse<[**GetWhatsAppBusinessProfile200Response**](GetWhatsAppBusinessProfile200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Business profile retrieved successfully |  -  |
| **400** | accountId is required or phone number ID not found |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |


## getWhatsAppDisplayName

> GetWhatsAppDisplayName200Response getWhatsAppDisplayName(accountId)

Get display name and review status

Fetch the current display name and its Meta review status for a WhatsApp Business account. Display name changes require Meta approval and can take 1-3 business days. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        try {
            GetWhatsAppDisplayName200Response result = apiInstance.getWhatsAppDisplayName(accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppDisplayName");
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
| **accountId** | **String**| WhatsApp social account ID | |

### Return type

[**GetWhatsAppDisplayName200Response**](GetWhatsAppDisplayName200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Display name info retrieved |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |

## getWhatsAppDisplayNameWithHttpInfo

> ApiResponse<GetWhatsAppDisplayName200Response> getWhatsAppDisplayName getWhatsAppDisplayNameWithHttpInfo(accountId)

Get display name and review status

Fetch the current display name and its Meta review status for a WhatsApp Business account. Display name changes require Meta approval and can take 1-3 business days. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        try {
            ApiResponse<GetWhatsAppDisplayName200Response> response = apiInstance.getWhatsAppDisplayNameWithHttpInfo(accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppDisplayName");
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
| **accountId** | **String**| WhatsApp social account ID | |

### Return type

ApiResponse<[**GetWhatsAppDisplayName200Response**](GetWhatsAppDisplayName200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Display name info retrieved |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |


## getWhatsAppGroupChat

> GetWhatsAppGroupChat200Response getWhatsAppGroupChat(groupId, accountId)

Get group info

Retrieve metadata about a WhatsApp group including subject, description, participants, and settings. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String groupId = "groupId_example"; // String | Group ID
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        try {
            GetWhatsAppGroupChat200Response result = apiInstance.getWhatsAppGroupChat(groupId, accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppGroupChat");
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
| **groupId** | **String**| Group ID | |
| **accountId** | **String**| WhatsApp social account ID | |

### Return type

[**GetWhatsAppGroupChat200Response**](GetWhatsAppGroupChat200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Group info |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## getWhatsAppGroupChatWithHttpInfo

> ApiResponse<GetWhatsAppGroupChat200Response> getWhatsAppGroupChat getWhatsAppGroupChatWithHttpInfo(groupId, accountId)

Get group info

Retrieve metadata about a WhatsApp group including subject, description, participants, and settings. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String groupId = "groupId_example"; // String | Group ID
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        try {
            ApiResponse<GetWhatsAppGroupChat200Response> response = apiInstance.getWhatsAppGroupChatWithHttpInfo(groupId, accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppGroupChat");
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
| **groupId** | **String**| Group ID | |
| **accountId** | **String**| WhatsApp social account ID | |

### Return type

ApiResponse<[**GetWhatsAppGroupChat200Response**](GetWhatsAppGroupChat200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Group info |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## getWhatsAppTemplate

> GetWhatsAppTemplate200Response getWhatsAppTemplate(templateName, accountId)

Get template

Retrieve a single message template by name. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String templateName = "templateName_example"; // String | Template name
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        try {
            GetWhatsAppTemplate200Response result = apiInstance.getWhatsAppTemplate(templateName, accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppTemplate");
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
| **templateName** | **String**| Template name | |
| **accountId** | **String**| WhatsApp social account ID | |

### Return type

[**GetWhatsAppTemplate200Response**](GetWhatsAppTemplate200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Template retrieved successfully |  -  |
| **400** | accountId is required |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## getWhatsAppTemplateWithHttpInfo

> ApiResponse<GetWhatsAppTemplate200Response> getWhatsAppTemplate getWhatsAppTemplateWithHttpInfo(templateName, accountId)

Get template

Retrieve a single message template by name. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String templateName = "templateName_example"; // String | Template name
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        try {
            ApiResponse<GetWhatsAppTemplate200Response> response = apiInstance.getWhatsAppTemplateWithHttpInfo(templateName, accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppTemplate");
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
| **templateName** | **String**| Template name | |
| **accountId** | **String**| WhatsApp social account ID | |

### Return type

ApiResponse<[**GetWhatsAppTemplate200Response**](GetWhatsAppTemplate200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Template retrieved successfully |  -  |
| **400** | accountId is required |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## getWhatsAppTemplates

> GetWhatsAppTemplates200Response getWhatsAppTemplates(accountId)

List templates

List all message templates for the WhatsApp Business Account (WABA) associated with the given account. Templates are fetched directly from the WhatsApp Cloud API. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        try {
            GetWhatsAppTemplates200Response result = apiInstance.getWhatsAppTemplates(accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppTemplates");
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
| **accountId** | **String**| WhatsApp social account ID | |

### Return type

[**GetWhatsAppTemplates200Response**](GetWhatsAppTemplates200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Templates retrieved successfully |  -  |
| **400** | accountId is required or WABA ID not found |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |

## getWhatsAppTemplatesWithHttpInfo

> ApiResponse<GetWhatsAppTemplates200Response> getWhatsAppTemplates getWhatsAppTemplatesWithHttpInfo(accountId)

List templates

List all message templates for the WhatsApp Business Account (WABA) associated with the given account. Templates are fetched directly from the WhatsApp Cloud API. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        try {
            ApiResponse<GetWhatsAppTemplates200Response> response = apiInstance.getWhatsAppTemplatesWithHttpInfo(accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppTemplates");
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
| **accountId** | **String**| WhatsApp social account ID | |

### Return type

ApiResponse<[**GetWhatsAppTemplates200Response**](GetWhatsAppTemplates200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Templates retrieved successfully |  -  |
| **400** | accountId is required or WABA ID not found |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |


## listWhatsAppGroupChats

> ListWhatsAppGroupChats200Response listWhatsAppGroupChats(accountId, limit, after)

List active groups

List active WhatsApp group chats for a business phone number. These are actual WhatsApp group conversations on the platform. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        Integer limit = 25; // Integer | Max groups to return
        String after = "after_example"; // String | Pagination cursor
        try {
            ListWhatsAppGroupChats200Response result = apiInstance.listWhatsAppGroupChats(accountId, limit, after);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#listWhatsAppGroupChats");
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
| **accountId** | **String**| WhatsApp social account ID | |
| **limit** | **Integer**| Max groups to return | [optional] [default to 25] |
| **after** | **String**| Pagination cursor | [optional] |

### Return type

[**ListWhatsAppGroupChats200Response**](ListWhatsAppGroupChats200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of active groups |  -  |
| **401** | Unauthorized |  -  |

## listWhatsAppGroupChatsWithHttpInfo

> ApiResponse<ListWhatsAppGroupChats200Response> listWhatsAppGroupChats listWhatsAppGroupChatsWithHttpInfo(accountId, limit, after)

List active groups

List active WhatsApp group chats for a business phone number. These are actual WhatsApp group conversations on the platform. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        Integer limit = 25; // Integer | Max groups to return
        String after = "after_example"; // String | Pagination cursor
        try {
            ApiResponse<ListWhatsAppGroupChats200Response> response = apiInstance.listWhatsAppGroupChatsWithHttpInfo(accountId, limit, after);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#listWhatsAppGroupChats");
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
| **accountId** | **String**| WhatsApp social account ID | |
| **limit** | **Integer**| Max groups to return | [optional] [default to 25] |
| **after** | **String**| Pagination cursor | [optional] |

### Return type

ApiResponse<[**ListWhatsAppGroupChats200Response**](ListWhatsAppGroupChats200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of active groups |  -  |
| **401** | Unauthorized |  -  |


## listWhatsAppGroupJoinRequests

> ListWhatsAppGroupJoinRequests200Response listWhatsAppGroupJoinRequests(groupId, accountId)

List join requests

List pending join requests for a WhatsApp group (only for groups with approval_required mode). 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String groupId = "groupId_example"; // String | Group ID
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        try {
            ListWhatsAppGroupJoinRequests200Response result = apiInstance.listWhatsAppGroupJoinRequests(groupId, accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#listWhatsAppGroupJoinRequests");
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
| **groupId** | **String**| Group ID | |
| **accountId** | **String**| WhatsApp social account ID | |

### Return type

[**ListWhatsAppGroupJoinRequests200Response**](ListWhatsAppGroupJoinRequests200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Join requests |  -  |
| **401** | Unauthorized |  -  |

## listWhatsAppGroupJoinRequestsWithHttpInfo

> ApiResponse<ListWhatsAppGroupJoinRequests200Response> listWhatsAppGroupJoinRequests listWhatsAppGroupJoinRequestsWithHttpInfo(groupId, accountId)

List join requests

List pending join requests for a WhatsApp group (only for groups with approval_required mode). 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String groupId = "groupId_example"; // String | Group ID
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        try {
            ApiResponse<ListWhatsAppGroupJoinRequests200Response> response = apiInstance.listWhatsAppGroupJoinRequestsWithHttpInfo(groupId, accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#listWhatsAppGroupJoinRequests");
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
| **groupId** | **String**| Group ID | |
| **accountId** | **String**| WhatsApp social account ID | |

### Return type

ApiResponse<[**ListWhatsAppGroupJoinRequests200Response**](ListWhatsAppGroupJoinRequests200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Join requests |  -  |
| **401** | Unauthorized |  -  |


## rejectWhatsAppGroupJoinRequests

> UnpublishPost200Response rejectWhatsAppGroupJoinRequests(groupId, accountId, rejectWhatsAppGroupJoinRequestsRequest)

Reject join requests

Reject pending join requests for a WhatsApp group. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String groupId = "groupId_example"; // String | Group ID
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        RejectWhatsAppGroupJoinRequestsRequest rejectWhatsAppGroupJoinRequestsRequest = new RejectWhatsAppGroupJoinRequestsRequest(); // RejectWhatsAppGroupJoinRequestsRequest | 
        try {
            UnpublishPost200Response result = apiInstance.rejectWhatsAppGroupJoinRequests(groupId, accountId, rejectWhatsAppGroupJoinRequestsRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#rejectWhatsAppGroupJoinRequests");
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
| **groupId** | **String**| Group ID | |
| **accountId** | **String**| WhatsApp social account ID | |
| **rejectWhatsAppGroupJoinRequestsRequest** | [**RejectWhatsAppGroupJoinRequestsRequest**](RejectWhatsAppGroupJoinRequestsRequest.md)|  | |

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
| **200** | Requests rejected |  -  |
| **401** | Unauthorized |  -  |

## rejectWhatsAppGroupJoinRequestsWithHttpInfo

> ApiResponse<UnpublishPost200Response> rejectWhatsAppGroupJoinRequests rejectWhatsAppGroupJoinRequestsWithHttpInfo(groupId, accountId, rejectWhatsAppGroupJoinRequestsRequest)

Reject join requests

Reject pending join requests for a WhatsApp group. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String groupId = "groupId_example"; // String | Group ID
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        RejectWhatsAppGroupJoinRequestsRequest rejectWhatsAppGroupJoinRequestsRequest = new RejectWhatsAppGroupJoinRequestsRequest(); // RejectWhatsAppGroupJoinRequestsRequest | 
        try {
            ApiResponse<UnpublishPost200Response> response = apiInstance.rejectWhatsAppGroupJoinRequestsWithHttpInfo(groupId, accountId, rejectWhatsAppGroupJoinRequestsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#rejectWhatsAppGroupJoinRequests");
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
| **groupId** | **String**| Group ID | |
| **accountId** | **String**| WhatsApp social account ID | |
| **rejectWhatsAppGroupJoinRequestsRequest** | [**RejectWhatsAppGroupJoinRequestsRequest**](RejectWhatsAppGroupJoinRequestsRequest.md)|  | |

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
| **200** | Requests rejected |  -  |
| **401** | Unauthorized |  -  |


## removeWhatsAppGroupParticipants

> UnpublishPost200Response removeWhatsAppGroupParticipants(groupId, accountId, removeWhatsAppGroupParticipantsRequest)

Remove participants

Remove participants from a WhatsApp group. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String groupId = "groupId_example"; // String | Group ID
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        RemoveWhatsAppGroupParticipantsRequest removeWhatsAppGroupParticipantsRequest = new RemoveWhatsAppGroupParticipantsRequest(); // RemoveWhatsAppGroupParticipantsRequest | 
        try {
            UnpublishPost200Response result = apiInstance.removeWhatsAppGroupParticipants(groupId, accountId, removeWhatsAppGroupParticipantsRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#removeWhatsAppGroupParticipants");
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
| **groupId** | **String**| Group ID | |
| **accountId** | **String**| WhatsApp social account ID | |
| **removeWhatsAppGroupParticipantsRequest** | [**RemoveWhatsAppGroupParticipantsRequest**](RemoveWhatsAppGroupParticipantsRequest.md)|  | |

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
| **200** | Participants removed |  -  |
| **401** | Unauthorized |  -  |

## removeWhatsAppGroupParticipantsWithHttpInfo

> ApiResponse<UnpublishPost200Response> removeWhatsAppGroupParticipants removeWhatsAppGroupParticipantsWithHttpInfo(groupId, accountId, removeWhatsAppGroupParticipantsRequest)

Remove participants

Remove participants from a WhatsApp group. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String groupId = "groupId_example"; // String | Group ID
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        RemoveWhatsAppGroupParticipantsRequest removeWhatsAppGroupParticipantsRequest = new RemoveWhatsAppGroupParticipantsRequest(); // RemoveWhatsAppGroupParticipantsRequest | 
        try {
            ApiResponse<UnpublishPost200Response> response = apiInstance.removeWhatsAppGroupParticipantsWithHttpInfo(groupId, accountId, removeWhatsAppGroupParticipantsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#removeWhatsAppGroupParticipants");
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
| **groupId** | **String**| Group ID | |
| **accountId** | **String**| WhatsApp social account ID | |
| **removeWhatsAppGroupParticipantsRequest** | [**RemoveWhatsAppGroupParticipantsRequest**](RemoveWhatsAppGroupParticipantsRequest.md)|  | |

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
| **200** | Participants removed |  -  |
| **401** | Unauthorized |  -  |


## updateWhatsAppBusinessProfile

> UnpublishPost200Response updateWhatsAppBusinessProfile(updateWhatsAppBusinessProfileRequest)

Update business profile

Update the WhatsApp Business profile. All fields are optional; only provided fields will be updated. Constraints: about max 139 chars, description max 512 chars, max 2 websites. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        UpdateWhatsAppBusinessProfileRequest updateWhatsAppBusinessProfileRequest = new UpdateWhatsAppBusinessProfileRequest(); // UpdateWhatsAppBusinessProfileRequest | 
        try {
            UnpublishPost200Response result = apiInstance.updateWhatsAppBusinessProfile(updateWhatsAppBusinessProfileRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#updateWhatsAppBusinessProfile");
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
| **updateWhatsAppBusinessProfileRequest** | [**UpdateWhatsAppBusinessProfileRequest**](UpdateWhatsAppBusinessProfileRequest.md)|  | |

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
| **200** | Business profile updated successfully |  -  |
| **400** | Validation error (field too long |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |

## updateWhatsAppBusinessProfileWithHttpInfo

> ApiResponse<UnpublishPost200Response> updateWhatsAppBusinessProfile updateWhatsAppBusinessProfileWithHttpInfo(updateWhatsAppBusinessProfileRequest)

Update business profile

Update the WhatsApp Business profile. All fields are optional; only provided fields will be updated. Constraints: about max 139 chars, description max 512 chars, max 2 websites. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        UpdateWhatsAppBusinessProfileRequest updateWhatsAppBusinessProfileRequest = new UpdateWhatsAppBusinessProfileRequest(); // UpdateWhatsAppBusinessProfileRequest | 
        try {
            ApiResponse<UnpublishPost200Response> response = apiInstance.updateWhatsAppBusinessProfileWithHttpInfo(updateWhatsAppBusinessProfileRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#updateWhatsAppBusinessProfile");
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
| **updateWhatsAppBusinessProfileRequest** | [**UpdateWhatsAppBusinessProfileRequest**](UpdateWhatsAppBusinessProfileRequest.md)|  | |

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
| **200** | Business profile updated successfully |  -  |
| **400** | Validation error (field too long |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |


## updateWhatsAppDisplayName

> UpdateWhatsAppDisplayName200Response updateWhatsAppDisplayName(updateWhatsAppDisplayNameRequest)

Request display name change

Submit a display name change request for the WhatsApp Business account. The new name must follow WhatsApp naming guidelines (3-512 characters, must represent your business). Changes require Meta review and approval, which typically takes 1-3 business days. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        UpdateWhatsAppDisplayNameRequest updateWhatsAppDisplayNameRequest = new UpdateWhatsAppDisplayNameRequest(); // UpdateWhatsAppDisplayNameRequest | 
        try {
            UpdateWhatsAppDisplayName200Response result = apiInstance.updateWhatsAppDisplayName(updateWhatsAppDisplayNameRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#updateWhatsAppDisplayName");
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
| **updateWhatsAppDisplayNameRequest** | [**UpdateWhatsAppDisplayNameRequest**](UpdateWhatsAppDisplayNameRequest.md)|  | |

### Return type

[**UpdateWhatsAppDisplayName200Response**](UpdateWhatsAppDisplayName200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Display name change submitted for review |  -  |
| **400** | Invalid display name (too short |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |

## updateWhatsAppDisplayNameWithHttpInfo

> ApiResponse<UpdateWhatsAppDisplayName200Response> updateWhatsAppDisplayName updateWhatsAppDisplayNameWithHttpInfo(updateWhatsAppDisplayNameRequest)

Request display name change

Submit a display name change request for the WhatsApp Business account. The new name must follow WhatsApp naming guidelines (3-512 characters, must represent your business). Changes require Meta review and approval, which typically takes 1-3 business days. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        UpdateWhatsAppDisplayNameRequest updateWhatsAppDisplayNameRequest = new UpdateWhatsAppDisplayNameRequest(); // UpdateWhatsAppDisplayNameRequest | 
        try {
            ApiResponse<UpdateWhatsAppDisplayName200Response> response = apiInstance.updateWhatsAppDisplayNameWithHttpInfo(updateWhatsAppDisplayNameRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#updateWhatsAppDisplayName");
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
| **updateWhatsAppDisplayNameRequest** | [**UpdateWhatsAppDisplayNameRequest**](UpdateWhatsAppDisplayNameRequest.md)|  | |

### Return type

ApiResponse<[**UpdateWhatsAppDisplayName200Response**](UpdateWhatsAppDisplayName200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Display name change submitted for review |  -  |
| **400** | Invalid display name (too short |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |


## updateWhatsAppGroupChat

> UnpublishPost200Response updateWhatsAppGroupChat(groupId, accountId, updateWhatsAppGroupChatRequest)

Update group settings

Update the subject, description, or join approval mode of a WhatsApp group. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String groupId = "groupId_example"; // String | Group ID
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        UpdateWhatsAppGroupChatRequest updateWhatsAppGroupChatRequest = new UpdateWhatsAppGroupChatRequest(); // UpdateWhatsAppGroupChatRequest | 
        try {
            UnpublishPost200Response result = apiInstance.updateWhatsAppGroupChat(groupId, accountId, updateWhatsAppGroupChatRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#updateWhatsAppGroupChat");
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
| **groupId** | **String**| Group ID | |
| **accountId** | **String**| WhatsApp social account ID | |
| **updateWhatsAppGroupChatRequest** | [**UpdateWhatsAppGroupChatRequest**](UpdateWhatsAppGroupChatRequest.md)|  | |

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
| **200** | Group updated |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## updateWhatsAppGroupChatWithHttpInfo

> ApiResponse<UnpublishPost200Response> updateWhatsAppGroupChat updateWhatsAppGroupChatWithHttpInfo(groupId, accountId, updateWhatsAppGroupChatRequest)

Update group settings

Update the subject, description, or join approval mode of a WhatsApp group. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String groupId = "groupId_example"; // String | Group ID
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        UpdateWhatsAppGroupChatRequest updateWhatsAppGroupChatRequest = new UpdateWhatsAppGroupChatRequest(); // UpdateWhatsAppGroupChatRequest | 
        try {
            ApiResponse<UnpublishPost200Response> response = apiInstance.updateWhatsAppGroupChatWithHttpInfo(groupId, accountId, updateWhatsAppGroupChatRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#updateWhatsAppGroupChat");
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
| **groupId** | **String**| Group ID | |
| **accountId** | **String**| WhatsApp social account ID | |
| **updateWhatsAppGroupChatRequest** | [**UpdateWhatsAppGroupChatRequest**](UpdateWhatsAppGroupChatRequest.md)|  | |

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
| **200** | Group updated |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## updateWhatsAppTemplate

> UpdateWhatsAppTemplate200Response updateWhatsAppTemplate(templateName, updateWhatsAppTemplateRequest)

Update template

Update a message template&#39;s components. Only certain fields can be updated depending on the template&#39;s current approval state. Approved templates can only have components updated. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String templateName = "templateName_example"; // String | Template name
        UpdateWhatsAppTemplateRequest updateWhatsAppTemplateRequest = new UpdateWhatsAppTemplateRequest(); // UpdateWhatsAppTemplateRequest | 
        try {
            UpdateWhatsAppTemplate200Response result = apiInstance.updateWhatsAppTemplate(templateName, updateWhatsAppTemplateRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#updateWhatsAppTemplate");
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
| **templateName** | **String**| Template name | |
| **updateWhatsAppTemplateRequest** | [**UpdateWhatsAppTemplateRequest**](UpdateWhatsAppTemplateRequest.md)|  | |

### Return type

[**UpdateWhatsAppTemplate200Response**](UpdateWhatsAppTemplate200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Template updated successfully |  -  |
| **400** | Validation error (missing fields) |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## updateWhatsAppTemplateWithHttpInfo

> ApiResponse<UpdateWhatsAppTemplate200Response> updateWhatsAppTemplate updateWhatsAppTemplateWithHttpInfo(templateName, updateWhatsAppTemplateRequest)

Update template

Update a message template&#39;s components. Only certain fields can be updated depending on the template&#39;s current approval state. Approved templates can only have components updated. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String templateName = "templateName_example"; // String | Template name
        UpdateWhatsAppTemplateRequest updateWhatsAppTemplateRequest = new UpdateWhatsAppTemplateRequest(); // UpdateWhatsAppTemplateRequest | 
        try {
            ApiResponse<UpdateWhatsAppTemplate200Response> response = apiInstance.updateWhatsAppTemplateWithHttpInfo(templateName, updateWhatsAppTemplateRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#updateWhatsAppTemplate");
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
| **templateName** | **String**| Template name | |
| **updateWhatsAppTemplateRequest** | [**UpdateWhatsAppTemplateRequest**](UpdateWhatsAppTemplateRequest.md)|  | |

### Return type

ApiResponse<[**UpdateWhatsAppTemplate200Response**](UpdateWhatsAppTemplate200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Template updated successfully |  -  |
| **400** | Validation error (missing fields) |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## uploadWhatsAppProfilePhoto

> UnpublishPost200Response uploadWhatsAppProfilePhoto(accountId, _file)

Upload profile picture

Upload a new profile picture for the WhatsApp Business Profile. Uses Meta&#39;s resumable upload API under the hood: creates an upload session, uploads the image bytes, then updates the business profile with the resulting handle. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        File _file = new File("/path/to/file"); // File | Image file (JPEG or PNG, max 5MB, recommended 640x640)
        try {
            UnpublishPost200Response result = apiInstance.uploadWhatsAppProfilePhoto(accountId, _file);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#uploadWhatsAppProfilePhoto");
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
| **accountId** | **String**| WhatsApp social account ID | |
| **_file** | **File**| Image file (JPEG or PNG, max 5MB, recommended 640x640) | |

### Return type

[**UnpublishPost200Response**](UnpublishPost200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Profile picture updated successfully |  -  |
| **400** | Invalid file type |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |

## uploadWhatsAppProfilePhotoWithHttpInfo

> ApiResponse<UnpublishPost200Response> uploadWhatsAppProfilePhoto uploadWhatsAppProfilePhotoWithHttpInfo(accountId, _file)

Upload profile picture

Upload a new profile picture for the WhatsApp Business Profile. Uses Meta&#39;s resumable upload API under the hood: creates an upload session, uploads the image bytes, then updates the business profile with the resulting handle. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.WhatsAppApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppApi apiInstance = new WhatsAppApi(defaultClient);
        String accountId = "accountId_example"; // String | WhatsApp social account ID
        File _file = new File("/path/to/file"); // File | Image file (JPEG or PNG, max 5MB, recommended 640x640)
        try {
            ApiResponse<UnpublishPost200Response> response = apiInstance.uploadWhatsAppProfilePhotoWithHttpInfo(accountId, _file);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#uploadWhatsAppProfilePhoto");
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
| **accountId** | **String**| WhatsApp social account ID | |
| **_file** | **File**| Image file (JPEG or PNG, max 5MB, recommended 640x640) | |

### Return type

ApiResponse<[**UnpublishPost200Response**](UnpublishPost200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Profile picture updated successfully |  -  |
| **400** | Invalid file type |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |

