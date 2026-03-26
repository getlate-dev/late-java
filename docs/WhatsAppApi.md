# WhatsAppApi

All URIs are relative to *https://zernio.com/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addWhatsAppBroadcastRecipients**](WhatsAppApi.md#addWhatsAppBroadcastRecipients) | **PATCH** /v1/whatsapp/broadcasts/{broadcastId}/recipients | Add recipients |
| [**addWhatsAppBroadcastRecipientsWithHttpInfo**](WhatsAppApi.md#addWhatsAppBroadcastRecipientsWithHttpInfo) | **PATCH** /v1/whatsapp/broadcasts/{broadcastId}/recipients | Add recipients |
| [**addWhatsAppGroupParticipants**](WhatsAppApi.md#addWhatsAppGroupParticipants) | **POST** /v1/whatsapp/wa-groups/{groupId}/participants | Add participants |
| [**addWhatsAppGroupParticipantsWithHttpInfo**](WhatsAppApi.md#addWhatsAppGroupParticipantsWithHttpInfo) | **POST** /v1/whatsapp/wa-groups/{groupId}/participants | Add participants |
| [**approveWhatsAppGroupJoinRequests**](WhatsAppApi.md#approveWhatsAppGroupJoinRequests) | **POST** /v1/whatsapp/wa-groups/{groupId}/join-requests | Approve join requests |
| [**approveWhatsAppGroupJoinRequestsWithHttpInfo**](WhatsAppApi.md#approveWhatsAppGroupJoinRequestsWithHttpInfo) | **POST** /v1/whatsapp/wa-groups/{groupId}/join-requests | Approve join requests |
| [**bulkDeleteWhatsAppContacts**](WhatsAppApi.md#bulkDeleteWhatsAppContacts) | **DELETE** /v1/whatsapp/contacts/bulk | Bulk delete contacts |
| [**bulkDeleteWhatsAppContactsWithHttpInfo**](WhatsAppApi.md#bulkDeleteWhatsAppContactsWithHttpInfo) | **DELETE** /v1/whatsapp/contacts/bulk | Bulk delete contacts |
| [**bulkUpdateWhatsAppContacts**](WhatsAppApi.md#bulkUpdateWhatsAppContacts) | **POST** /v1/whatsapp/contacts/bulk | Bulk update contacts |
| [**bulkUpdateWhatsAppContactsWithHttpInfo**](WhatsAppApi.md#bulkUpdateWhatsAppContactsWithHttpInfo) | **POST** /v1/whatsapp/contacts/bulk | Bulk update contacts |
| [**cancelWhatsAppBroadcastSchedule**](WhatsAppApi.md#cancelWhatsAppBroadcastSchedule) | **DELETE** /v1/whatsapp/broadcasts/{broadcastId}/schedule | Cancel scheduled broadcast |
| [**cancelWhatsAppBroadcastScheduleWithHttpInfo**](WhatsAppApi.md#cancelWhatsAppBroadcastScheduleWithHttpInfo) | **DELETE** /v1/whatsapp/broadcasts/{broadcastId}/schedule | Cancel scheduled broadcast |
| [**createWhatsAppBroadcast**](WhatsAppApi.md#createWhatsAppBroadcast) | **POST** /v1/whatsapp/broadcasts | Create broadcast |
| [**createWhatsAppBroadcastWithHttpInfo**](WhatsAppApi.md#createWhatsAppBroadcastWithHttpInfo) | **POST** /v1/whatsapp/broadcasts | Create broadcast |
| [**createWhatsAppContact**](WhatsAppApi.md#createWhatsAppContact) | **POST** /v1/whatsapp/contacts | Create contact |
| [**createWhatsAppContactWithHttpInfo**](WhatsAppApi.md#createWhatsAppContactWithHttpInfo) | **POST** /v1/whatsapp/contacts | Create contact |
| [**createWhatsAppGroupChat**](WhatsAppApi.md#createWhatsAppGroupChat) | **POST** /v1/whatsapp/wa-groups | Create group |
| [**createWhatsAppGroupChatWithHttpInfo**](WhatsAppApi.md#createWhatsAppGroupChatWithHttpInfo) | **POST** /v1/whatsapp/wa-groups | Create group |
| [**createWhatsAppGroupInviteLink**](WhatsAppApi.md#createWhatsAppGroupInviteLink) | **POST** /v1/whatsapp/wa-groups/{groupId}/invite-link | Create invite link |
| [**createWhatsAppGroupInviteLinkWithHttpInfo**](WhatsAppApi.md#createWhatsAppGroupInviteLinkWithHttpInfo) | **POST** /v1/whatsapp/wa-groups/{groupId}/invite-link | Create invite link |
| [**createWhatsAppTemplate**](WhatsAppApi.md#createWhatsAppTemplate) | **POST** /v1/whatsapp/templates | Create template |
| [**createWhatsAppTemplateWithHttpInfo**](WhatsAppApi.md#createWhatsAppTemplateWithHttpInfo) | **POST** /v1/whatsapp/templates | Create template |
| [**deleteWhatsAppBroadcast**](WhatsAppApi.md#deleteWhatsAppBroadcast) | **DELETE** /v1/whatsapp/broadcasts/{broadcastId} | Delete broadcast |
| [**deleteWhatsAppBroadcastWithHttpInfo**](WhatsAppApi.md#deleteWhatsAppBroadcastWithHttpInfo) | **DELETE** /v1/whatsapp/broadcasts/{broadcastId} | Delete broadcast |
| [**deleteWhatsAppContact**](WhatsAppApi.md#deleteWhatsAppContact) | **DELETE** /v1/whatsapp/contacts/{contactId} | Delete contact |
| [**deleteWhatsAppContactWithHttpInfo**](WhatsAppApi.md#deleteWhatsAppContactWithHttpInfo) | **DELETE** /v1/whatsapp/contacts/{contactId} | Delete contact |
| [**deleteWhatsAppGroup**](WhatsAppApi.md#deleteWhatsAppGroup) | **DELETE** /v1/whatsapp/groups | Delete group |
| [**deleteWhatsAppGroupWithHttpInfo**](WhatsAppApi.md#deleteWhatsAppGroupWithHttpInfo) | **DELETE** /v1/whatsapp/groups | Delete group |
| [**deleteWhatsAppGroupChat**](WhatsAppApi.md#deleteWhatsAppGroupChat) | **DELETE** /v1/whatsapp/wa-groups/{groupId} | Delete group |
| [**deleteWhatsAppGroupChatWithHttpInfo**](WhatsAppApi.md#deleteWhatsAppGroupChatWithHttpInfo) | **DELETE** /v1/whatsapp/wa-groups/{groupId} | Delete group |
| [**deleteWhatsAppTemplate**](WhatsAppApi.md#deleteWhatsAppTemplate) | **DELETE** /v1/whatsapp/templates/{templateName} | Delete template |
| [**deleteWhatsAppTemplateWithHttpInfo**](WhatsAppApi.md#deleteWhatsAppTemplateWithHttpInfo) | **DELETE** /v1/whatsapp/templates/{templateName} | Delete template |
| [**getWhatsAppBroadcast**](WhatsAppApi.md#getWhatsAppBroadcast) | **GET** /v1/whatsapp/broadcasts/{broadcastId} | Get broadcast |
| [**getWhatsAppBroadcastWithHttpInfo**](WhatsAppApi.md#getWhatsAppBroadcastWithHttpInfo) | **GET** /v1/whatsapp/broadcasts/{broadcastId} | Get broadcast |
| [**getWhatsAppBroadcastRecipients**](WhatsAppApi.md#getWhatsAppBroadcastRecipients) | **GET** /v1/whatsapp/broadcasts/{broadcastId}/recipients | List recipients |
| [**getWhatsAppBroadcastRecipientsWithHttpInfo**](WhatsAppApi.md#getWhatsAppBroadcastRecipientsWithHttpInfo) | **GET** /v1/whatsapp/broadcasts/{broadcastId}/recipients | List recipients |
| [**getWhatsAppBroadcasts**](WhatsAppApi.md#getWhatsAppBroadcasts) | **GET** /v1/whatsapp/broadcasts | List broadcasts |
| [**getWhatsAppBroadcastsWithHttpInfo**](WhatsAppApi.md#getWhatsAppBroadcastsWithHttpInfo) | **GET** /v1/whatsapp/broadcasts | List broadcasts |
| [**getWhatsAppBusinessProfile**](WhatsAppApi.md#getWhatsAppBusinessProfile) | **GET** /v1/whatsapp/business-profile | Get business profile |
| [**getWhatsAppBusinessProfileWithHttpInfo**](WhatsAppApi.md#getWhatsAppBusinessProfileWithHttpInfo) | **GET** /v1/whatsapp/business-profile | Get business profile |
| [**getWhatsAppContact**](WhatsAppApi.md#getWhatsAppContact) | **GET** /v1/whatsapp/contacts/{contactId} | Get contact |
| [**getWhatsAppContactWithHttpInfo**](WhatsAppApi.md#getWhatsAppContactWithHttpInfo) | **GET** /v1/whatsapp/contacts/{contactId} | Get contact |
| [**getWhatsAppContacts**](WhatsAppApi.md#getWhatsAppContacts) | **GET** /v1/whatsapp/contacts | List contacts |
| [**getWhatsAppContactsWithHttpInfo**](WhatsAppApi.md#getWhatsAppContactsWithHttpInfo) | **GET** /v1/whatsapp/contacts | List contacts |
| [**getWhatsAppDisplayName**](WhatsAppApi.md#getWhatsAppDisplayName) | **GET** /v1/whatsapp/business-profile/display-name | Get display name and review status |
| [**getWhatsAppDisplayNameWithHttpInfo**](WhatsAppApi.md#getWhatsAppDisplayNameWithHttpInfo) | **GET** /v1/whatsapp/business-profile/display-name | Get display name and review status |
| [**getWhatsAppGroupChat**](WhatsAppApi.md#getWhatsAppGroupChat) | **GET** /v1/whatsapp/wa-groups/{groupId} | Get group info |
| [**getWhatsAppGroupChatWithHttpInfo**](WhatsAppApi.md#getWhatsAppGroupChatWithHttpInfo) | **GET** /v1/whatsapp/wa-groups/{groupId} | Get group info |
| [**getWhatsAppGroups**](WhatsAppApi.md#getWhatsAppGroups) | **GET** /v1/whatsapp/groups | List contact groups |
| [**getWhatsAppGroupsWithHttpInfo**](WhatsAppApi.md#getWhatsAppGroupsWithHttpInfo) | **GET** /v1/whatsapp/groups | List contact groups |
| [**getWhatsAppTemplate**](WhatsAppApi.md#getWhatsAppTemplate) | **GET** /v1/whatsapp/templates/{templateName} | Get template |
| [**getWhatsAppTemplateWithHttpInfo**](WhatsAppApi.md#getWhatsAppTemplateWithHttpInfo) | **GET** /v1/whatsapp/templates/{templateName} | Get template |
| [**getWhatsAppTemplates**](WhatsAppApi.md#getWhatsAppTemplates) | **GET** /v1/whatsapp/templates | List templates |
| [**getWhatsAppTemplatesWithHttpInfo**](WhatsAppApi.md#getWhatsAppTemplatesWithHttpInfo) | **GET** /v1/whatsapp/templates | List templates |
| [**importWhatsAppContacts**](WhatsAppApi.md#importWhatsAppContacts) | **POST** /v1/whatsapp/contacts/import | Bulk import contacts |
| [**importWhatsAppContactsWithHttpInfo**](WhatsAppApi.md#importWhatsAppContactsWithHttpInfo) | **POST** /v1/whatsapp/contacts/import | Bulk import contacts |
| [**listWhatsAppGroupChats**](WhatsAppApi.md#listWhatsAppGroupChats) | **GET** /v1/whatsapp/wa-groups | List active groups |
| [**listWhatsAppGroupChatsWithHttpInfo**](WhatsAppApi.md#listWhatsAppGroupChatsWithHttpInfo) | **GET** /v1/whatsapp/wa-groups | List active groups |
| [**listWhatsAppGroupJoinRequests**](WhatsAppApi.md#listWhatsAppGroupJoinRequests) | **GET** /v1/whatsapp/wa-groups/{groupId}/join-requests | List join requests |
| [**listWhatsAppGroupJoinRequestsWithHttpInfo**](WhatsAppApi.md#listWhatsAppGroupJoinRequestsWithHttpInfo) | **GET** /v1/whatsapp/wa-groups/{groupId}/join-requests | List join requests |
| [**rejectWhatsAppGroupJoinRequests**](WhatsAppApi.md#rejectWhatsAppGroupJoinRequests) | **DELETE** /v1/whatsapp/wa-groups/{groupId}/join-requests | Reject join requests |
| [**rejectWhatsAppGroupJoinRequestsWithHttpInfo**](WhatsAppApi.md#rejectWhatsAppGroupJoinRequestsWithHttpInfo) | **DELETE** /v1/whatsapp/wa-groups/{groupId}/join-requests | Reject join requests |
| [**removeWhatsAppBroadcastRecipients**](WhatsAppApi.md#removeWhatsAppBroadcastRecipients) | **DELETE** /v1/whatsapp/broadcasts/{broadcastId}/recipients | Remove recipients |
| [**removeWhatsAppBroadcastRecipientsWithHttpInfo**](WhatsAppApi.md#removeWhatsAppBroadcastRecipientsWithHttpInfo) | **DELETE** /v1/whatsapp/broadcasts/{broadcastId}/recipients | Remove recipients |
| [**removeWhatsAppGroupParticipants**](WhatsAppApi.md#removeWhatsAppGroupParticipants) | **DELETE** /v1/whatsapp/wa-groups/{groupId}/participants | Remove participants |
| [**removeWhatsAppGroupParticipantsWithHttpInfo**](WhatsAppApi.md#removeWhatsAppGroupParticipantsWithHttpInfo) | **DELETE** /v1/whatsapp/wa-groups/{groupId}/participants | Remove participants |
| [**renameWhatsAppGroup**](WhatsAppApi.md#renameWhatsAppGroup) | **POST** /v1/whatsapp/groups | Rename group |
| [**renameWhatsAppGroupWithHttpInfo**](WhatsAppApi.md#renameWhatsAppGroupWithHttpInfo) | **POST** /v1/whatsapp/groups | Rename group |
| [**scheduleWhatsAppBroadcast**](WhatsAppApi.md#scheduleWhatsAppBroadcast) | **POST** /v1/whatsapp/broadcasts/{broadcastId}/schedule | Schedule broadcast |
| [**scheduleWhatsAppBroadcastWithHttpInfo**](WhatsAppApi.md#scheduleWhatsAppBroadcastWithHttpInfo) | **POST** /v1/whatsapp/broadcasts/{broadcastId}/schedule | Schedule broadcast |
| [**sendWhatsAppBroadcast**](WhatsAppApi.md#sendWhatsAppBroadcast) | **POST** /v1/whatsapp/broadcasts/{broadcastId}/send | Send broadcast |
| [**sendWhatsAppBroadcastWithHttpInfo**](WhatsAppApi.md#sendWhatsAppBroadcastWithHttpInfo) | **POST** /v1/whatsapp/broadcasts/{broadcastId}/send | Send broadcast |
| [**sendWhatsAppBulk**](WhatsAppApi.md#sendWhatsAppBulk) | **POST** /v1/whatsapp/bulk | Bulk send template messages |
| [**sendWhatsAppBulkWithHttpInfo**](WhatsAppApi.md#sendWhatsAppBulkWithHttpInfo) | **POST** /v1/whatsapp/bulk | Bulk send template messages |
| [**updateWhatsAppBusinessProfile**](WhatsAppApi.md#updateWhatsAppBusinessProfile) | **POST** /v1/whatsapp/business-profile | Update business profile |
| [**updateWhatsAppBusinessProfileWithHttpInfo**](WhatsAppApi.md#updateWhatsAppBusinessProfileWithHttpInfo) | **POST** /v1/whatsapp/business-profile | Update business profile |
| [**updateWhatsAppContact**](WhatsAppApi.md#updateWhatsAppContact) | **PUT** /v1/whatsapp/contacts/{contactId} | Update contact |
| [**updateWhatsAppContactWithHttpInfo**](WhatsAppApi.md#updateWhatsAppContactWithHttpInfo) | **PUT** /v1/whatsapp/contacts/{contactId} | Update contact |
| [**updateWhatsAppDisplayName**](WhatsAppApi.md#updateWhatsAppDisplayName) | **POST** /v1/whatsapp/business-profile/display-name | Request display name change |
| [**updateWhatsAppDisplayNameWithHttpInfo**](WhatsAppApi.md#updateWhatsAppDisplayNameWithHttpInfo) | **POST** /v1/whatsapp/business-profile/display-name | Request display name change |
| [**updateWhatsAppGroupChat**](WhatsAppApi.md#updateWhatsAppGroupChat) | **POST** /v1/whatsapp/wa-groups/{groupId} | Update group settings |
| [**updateWhatsAppGroupChatWithHttpInfo**](WhatsAppApi.md#updateWhatsAppGroupChatWithHttpInfo) | **POST** /v1/whatsapp/wa-groups/{groupId} | Update group settings |
| [**updateWhatsAppTemplate**](WhatsAppApi.md#updateWhatsAppTemplate) | **PATCH** /v1/whatsapp/templates/{templateName} | Update template |
| [**updateWhatsAppTemplateWithHttpInfo**](WhatsAppApi.md#updateWhatsAppTemplateWithHttpInfo) | **PATCH** /v1/whatsapp/templates/{templateName} | Update template |
| [**uploadWhatsAppProfilePhoto**](WhatsAppApi.md#uploadWhatsAppProfilePhoto) | **POST** /v1/whatsapp/business-profile/photo | Upload profile picture |
| [**uploadWhatsAppProfilePhotoWithHttpInfo**](WhatsAppApi.md#uploadWhatsAppProfilePhotoWithHttpInfo) | **POST** /v1/whatsapp/business-profile/photo | Upload profile picture |



## addWhatsAppBroadcastRecipients

> AddWhatsAppBroadcastRecipients200Response addWhatsAppBroadcastRecipients(broadcastId, addWhatsAppBroadcastRecipientsRequest)

Add recipients

**Deprecated.** Use &#x60;POST /v1/broadcasts/{id}/recipients&#x60; instead. Add recipients to a draft broadcast. Maximum 1000 recipients per request. Duplicate phone numbers are automatically skipped. 

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
        String broadcastId = "broadcastId_example"; // String | Broadcast ID
        AddWhatsAppBroadcastRecipientsRequest addWhatsAppBroadcastRecipientsRequest = new AddWhatsAppBroadcastRecipientsRequest(); // AddWhatsAppBroadcastRecipientsRequest | 
        try {
            AddWhatsAppBroadcastRecipients200Response result = apiInstance.addWhatsAppBroadcastRecipients(broadcastId, addWhatsAppBroadcastRecipientsRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#addWhatsAppBroadcastRecipients");
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
| **broadcastId** | **String**| Broadcast ID | |
| **addWhatsAppBroadcastRecipientsRequest** | [**AddWhatsAppBroadcastRecipientsRequest**](AddWhatsAppBroadcastRecipientsRequest.md)|  | |

### Return type

[**AddWhatsAppBroadcastRecipients200Response**](AddWhatsAppBroadcastRecipients200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Recipients added successfully |  -  |
| **400** | Validation error or broadcast not in draft status |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## addWhatsAppBroadcastRecipientsWithHttpInfo

> ApiResponse<AddWhatsAppBroadcastRecipients200Response> addWhatsAppBroadcastRecipients addWhatsAppBroadcastRecipientsWithHttpInfo(broadcastId, addWhatsAppBroadcastRecipientsRequest)

Add recipients

**Deprecated.** Use &#x60;POST /v1/broadcasts/{id}/recipients&#x60; instead. Add recipients to a draft broadcast. Maximum 1000 recipients per request. Duplicate phone numbers are automatically skipped. 

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
        String broadcastId = "broadcastId_example"; // String | Broadcast ID
        AddWhatsAppBroadcastRecipientsRequest addWhatsAppBroadcastRecipientsRequest = new AddWhatsAppBroadcastRecipientsRequest(); // AddWhatsAppBroadcastRecipientsRequest | 
        try {
            ApiResponse<AddWhatsAppBroadcastRecipients200Response> response = apiInstance.addWhatsAppBroadcastRecipientsWithHttpInfo(broadcastId, addWhatsAppBroadcastRecipientsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#addWhatsAppBroadcastRecipients");
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
| **broadcastId** | **String**| Broadcast ID | |
| **addWhatsAppBroadcastRecipientsRequest** | [**AddWhatsAppBroadcastRecipientsRequest**](AddWhatsAppBroadcastRecipientsRequest.md)|  | |

### Return type

ApiResponse<[**AddWhatsAppBroadcastRecipients200Response**](AddWhatsAppBroadcastRecipients200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Recipients added successfully |  -  |
| **400** | Validation error or broadcast not in draft status |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


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


## bulkDeleteWhatsAppContacts

> BulkDeleteWhatsAppContacts200Response bulkDeleteWhatsAppContacts(bulkDeleteWhatsAppContactsRequest)

Bulk delete contacts

**Deprecated.** Use &#x60;DELETE /v1/contacts/{id}&#x60; for individual deletes instead. Permanently delete multiple contacts at once (max 500 per request). 

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
        BulkDeleteWhatsAppContactsRequest bulkDeleteWhatsAppContactsRequest = new BulkDeleteWhatsAppContactsRequest(); // BulkDeleteWhatsAppContactsRequest | 
        try {
            BulkDeleteWhatsAppContacts200Response result = apiInstance.bulkDeleteWhatsAppContacts(bulkDeleteWhatsAppContactsRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#bulkDeleteWhatsAppContacts");
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
| **bulkDeleteWhatsAppContactsRequest** | [**BulkDeleteWhatsAppContactsRequest**](BulkDeleteWhatsAppContactsRequest.md)|  | |

### Return type

[**BulkDeleteWhatsAppContacts200Response**](BulkDeleteWhatsAppContacts200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Bulk delete completed |  -  |
| **400** | contactIds array is required |  -  |
| **401** | Unauthorized |  -  |

## bulkDeleteWhatsAppContactsWithHttpInfo

> ApiResponse<BulkDeleteWhatsAppContacts200Response> bulkDeleteWhatsAppContacts bulkDeleteWhatsAppContactsWithHttpInfo(bulkDeleteWhatsAppContactsRequest)

Bulk delete contacts

**Deprecated.** Use &#x60;DELETE /v1/contacts/{id}&#x60; for individual deletes instead. Permanently delete multiple contacts at once (max 500 per request). 

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
        BulkDeleteWhatsAppContactsRequest bulkDeleteWhatsAppContactsRequest = new BulkDeleteWhatsAppContactsRequest(); // BulkDeleteWhatsAppContactsRequest | 
        try {
            ApiResponse<BulkDeleteWhatsAppContacts200Response> response = apiInstance.bulkDeleteWhatsAppContactsWithHttpInfo(bulkDeleteWhatsAppContactsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#bulkDeleteWhatsAppContacts");
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
| **bulkDeleteWhatsAppContactsRequest** | [**BulkDeleteWhatsAppContactsRequest**](BulkDeleteWhatsAppContactsRequest.md)|  | |

### Return type

ApiResponse<[**BulkDeleteWhatsAppContacts200Response**](BulkDeleteWhatsAppContacts200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Bulk delete completed |  -  |
| **400** | contactIds array is required |  -  |
| **401** | Unauthorized |  -  |


## bulkUpdateWhatsAppContacts

> BulkUpdateWhatsAppContacts200Response bulkUpdateWhatsAppContacts(bulkUpdateWhatsAppContactsRequest)

Bulk update contacts

**Deprecated.** Use &#x60;PATCH /v1/contacts/{id}&#x60; for individual updates instead. Perform bulk operations on multiple contacts (max 500 per request). Supported actions: addTags, removeTags, addGroups, removeGroups, optIn, optOut, block, unblock. 

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
        BulkUpdateWhatsAppContactsRequest bulkUpdateWhatsAppContactsRequest = new BulkUpdateWhatsAppContactsRequest(); // BulkUpdateWhatsAppContactsRequest | 
        try {
            BulkUpdateWhatsAppContacts200Response result = apiInstance.bulkUpdateWhatsAppContacts(bulkUpdateWhatsAppContactsRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#bulkUpdateWhatsAppContacts");
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
| **bulkUpdateWhatsAppContactsRequest** | [**BulkUpdateWhatsAppContactsRequest**](BulkUpdateWhatsAppContactsRequest.md)|  | |

### Return type

[**BulkUpdateWhatsAppContacts200Response**](BulkUpdateWhatsAppContacts200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Bulk update completed |  -  |
| **400** | Validation error (invalid action |  -  |
| **401** | Unauthorized |  -  |

## bulkUpdateWhatsAppContactsWithHttpInfo

> ApiResponse<BulkUpdateWhatsAppContacts200Response> bulkUpdateWhatsAppContacts bulkUpdateWhatsAppContactsWithHttpInfo(bulkUpdateWhatsAppContactsRequest)

Bulk update contacts

**Deprecated.** Use &#x60;PATCH /v1/contacts/{id}&#x60; for individual updates instead. Perform bulk operations on multiple contacts (max 500 per request). Supported actions: addTags, removeTags, addGroups, removeGroups, optIn, optOut, block, unblock. 

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
        BulkUpdateWhatsAppContactsRequest bulkUpdateWhatsAppContactsRequest = new BulkUpdateWhatsAppContactsRequest(); // BulkUpdateWhatsAppContactsRequest | 
        try {
            ApiResponse<BulkUpdateWhatsAppContacts200Response> response = apiInstance.bulkUpdateWhatsAppContactsWithHttpInfo(bulkUpdateWhatsAppContactsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#bulkUpdateWhatsAppContacts");
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
| **bulkUpdateWhatsAppContactsRequest** | [**BulkUpdateWhatsAppContactsRequest**](BulkUpdateWhatsAppContactsRequest.md)|  | |

### Return type

ApiResponse<[**BulkUpdateWhatsAppContacts200Response**](BulkUpdateWhatsAppContacts200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Bulk update completed |  -  |
| **400** | Validation error (invalid action |  -  |
| **401** | Unauthorized |  -  |


## cancelWhatsAppBroadcastSchedule

> CancelWhatsAppBroadcastSchedule200Response cancelWhatsAppBroadcastSchedule(broadcastId)

Cancel scheduled broadcast

**Deprecated.** Use &#x60;POST /v1/broadcasts/{id}/cancel&#x60; instead. Cancel a scheduled broadcast and return it to draft status. Only broadcasts in scheduled status can be cancelled. 

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
        String broadcastId = "broadcastId_example"; // String | Broadcast ID
        try {
            CancelWhatsAppBroadcastSchedule200Response result = apiInstance.cancelWhatsAppBroadcastSchedule(broadcastId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#cancelWhatsAppBroadcastSchedule");
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
| **broadcastId** | **String**| Broadcast ID | |

### Return type

[**CancelWhatsAppBroadcastSchedule200Response**](CancelWhatsAppBroadcastSchedule200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Schedule cancelled, broadcast returned to draft |  -  |
| **400** | Broadcast is not scheduled |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## cancelWhatsAppBroadcastScheduleWithHttpInfo

> ApiResponse<CancelWhatsAppBroadcastSchedule200Response> cancelWhatsAppBroadcastSchedule cancelWhatsAppBroadcastScheduleWithHttpInfo(broadcastId)

Cancel scheduled broadcast

**Deprecated.** Use &#x60;POST /v1/broadcasts/{id}/cancel&#x60; instead. Cancel a scheduled broadcast and return it to draft status. Only broadcasts in scheduled status can be cancelled. 

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
        String broadcastId = "broadcastId_example"; // String | Broadcast ID
        try {
            ApiResponse<CancelWhatsAppBroadcastSchedule200Response> response = apiInstance.cancelWhatsAppBroadcastScheduleWithHttpInfo(broadcastId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#cancelWhatsAppBroadcastSchedule");
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
| **broadcastId** | **String**| Broadcast ID | |

### Return type

ApiResponse<[**CancelWhatsAppBroadcastSchedule200Response**](CancelWhatsAppBroadcastSchedule200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Schedule cancelled, broadcast returned to draft |  -  |
| **400** | Broadcast is not scheduled |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## createWhatsAppBroadcast

> CreateWhatsAppBroadcast200Response createWhatsAppBroadcast(createWhatsAppBroadcastRequest)

Create broadcast

**Deprecated.** Use &#x60;POST /v1/broadcasts&#x60; instead. Create a new draft broadcast. Optionally include initial recipients. After creation, add recipients and then send or schedule the broadcast. 

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
        CreateWhatsAppBroadcastRequest createWhatsAppBroadcastRequest = new CreateWhatsAppBroadcastRequest(); // CreateWhatsAppBroadcastRequest | 
        try {
            CreateWhatsAppBroadcast200Response result = apiInstance.createWhatsAppBroadcast(createWhatsAppBroadcastRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#createWhatsAppBroadcast");
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
| **createWhatsAppBroadcastRequest** | [**CreateWhatsAppBroadcastRequest**](CreateWhatsAppBroadcastRequest.md)|  | |

### Return type

[**CreateWhatsAppBroadcast200Response**](CreateWhatsAppBroadcast200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Broadcast created as draft |  -  |
| **400** | Validation error (missing name |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |

## createWhatsAppBroadcastWithHttpInfo

> ApiResponse<CreateWhatsAppBroadcast200Response> createWhatsAppBroadcast createWhatsAppBroadcastWithHttpInfo(createWhatsAppBroadcastRequest)

Create broadcast

**Deprecated.** Use &#x60;POST /v1/broadcasts&#x60; instead. Create a new draft broadcast. Optionally include initial recipients. After creation, add recipients and then send or schedule the broadcast. 

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
        CreateWhatsAppBroadcastRequest createWhatsAppBroadcastRequest = new CreateWhatsAppBroadcastRequest(); // CreateWhatsAppBroadcastRequest | 
        try {
            ApiResponse<CreateWhatsAppBroadcast200Response> response = apiInstance.createWhatsAppBroadcastWithHttpInfo(createWhatsAppBroadcastRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#createWhatsAppBroadcast");
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
| **createWhatsAppBroadcastRequest** | [**CreateWhatsAppBroadcastRequest**](CreateWhatsAppBroadcastRequest.md)|  | |

### Return type

ApiResponse<[**CreateWhatsAppBroadcast200Response**](CreateWhatsAppBroadcast200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Broadcast created as draft |  -  |
| **400** | Validation error (missing name |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |


## createWhatsAppContact

> CreateWhatsAppContact200Response createWhatsAppContact(createWhatsAppContactRequest)

Create contact

**Deprecated.** Use &#x60;POST /v1/contacts&#x60; instead. Create a new WhatsApp contact. Phone number must be unique per account and in E.164 format (e.g., +1234567890). 

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
        CreateWhatsAppContactRequest createWhatsAppContactRequest = new CreateWhatsAppContactRequest(); // CreateWhatsAppContactRequest | 
        try {
            CreateWhatsAppContact200Response result = apiInstance.createWhatsAppContact(createWhatsAppContactRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#createWhatsAppContact");
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
| **createWhatsAppContactRequest** | [**CreateWhatsAppContactRequest**](CreateWhatsAppContactRequest.md)|  | |

### Return type

[**CreateWhatsAppContact200Response**](CreateWhatsAppContact200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Contact created successfully |  -  |
| **400** | Validation error (missing fields |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |
| **409** | Contact with this phone number already exists |  -  |

## createWhatsAppContactWithHttpInfo

> ApiResponse<CreateWhatsAppContact200Response> createWhatsAppContact createWhatsAppContactWithHttpInfo(createWhatsAppContactRequest)

Create contact

**Deprecated.** Use &#x60;POST /v1/contacts&#x60; instead. Create a new WhatsApp contact. Phone number must be unique per account and in E.164 format (e.g., +1234567890). 

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
        CreateWhatsAppContactRequest createWhatsAppContactRequest = new CreateWhatsAppContactRequest(); // CreateWhatsAppContactRequest | 
        try {
            ApiResponse<CreateWhatsAppContact200Response> response = apiInstance.createWhatsAppContactWithHttpInfo(createWhatsAppContactRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#createWhatsAppContact");
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
| **createWhatsAppContactRequest** | [**CreateWhatsAppContactRequest**](CreateWhatsAppContactRequest.md)|  | |

### Return type

ApiResponse<[**CreateWhatsAppContact200Response**](CreateWhatsAppContact200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Contact created successfully |  -  |
| **400** | Validation error (missing fields |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |
| **409** | Contact with this phone number already exists |  -  |


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


## deleteWhatsAppBroadcast

> UnpublishPost200Response deleteWhatsAppBroadcast(broadcastId)

Delete broadcast

**Deprecated.** Use &#x60;DELETE /v1/broadcasts/{id}&#x60; instead. Delete a broadcast. Only draft or cancelled broadcasts can be deleted. 

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
        String broadcastId = "broadcastId_example"; // String | Broadcast ID
        try {
            UnpublishPost200Response result = apiInstance.deleteWhatsAppBroadcast(broadcastId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#deleteWhatsAppBroadcast");
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
| **broadcastId** | **String**| Broadcast ID | |

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
| **200** | Broadcast deleted successfully |  -  |
| **400** | Can only delete draft or cancelled broadcasts |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## deleteWhatsAppBroadcastWithHttpInfo

> ApiResponse<UnpublishPost200Response> deleteWhatsAppBroadcast deleteWhatsAppBroadcastWithHttpInfo(broadcastId)

Delete broadcast

**Deprecated.** Use &#x60;DELETE /v1/broadcasts/{id}&#x60; instead. Delete a broadcast. Only draft or cancelled broadcasts can be deleted. 

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
        String broadcastId = "broadcastId_example"; // String | Broadcast ID
        try {
            ApiResponse<UnpublishPost200Response> response = apiInstance.deleteWhatsAppBroadcastWithHttpInfo(broadcastId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#deleteWhatsAppBroadcast");
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
| **broadcastId** | **String**| Broadcast ID | |

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
| **200** | Broadcast deleted successfully |  -  |
| **400** | Can only delete draft or cancelled broadcasts |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## deleteWhatsAppContact

> UnpublishPost200Response deleteWhatsAppContact(contactId)

Delete contact

**Deprecated.** Use &#x60;DELETE /v1/contacts/{id}&#x60; instead. Permanently delete a WhatsApp contact. 

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
        String contactId = "contactId_example"; // String | Contact ID
        try {
            UnpublishPost200Response result = apiInstance.deleteWhatsAppContact(contactId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#deleteWhatsAppContact");
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
| **contactId** | **String**| Contact ID | |

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
| **200** | Contact deleted successfully |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## deleteWhatsAppContactWithHttpInfo

> ApiResponse<UnpublishPost200Response> deleteWhatsAppContact deleteWhatsAppContactWithHttpInfo(contactId)

Delete contact

**Deprecated.** Use &#x60;DELETE /v1/contacts/{id}&#x60; instead. Permanently delete a WhatsApp contact. 

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
        String contactId = "contactId_example"; // String | Contact ID
        try {
            ApiResponse<UnpublishPost200Response> response = apiInstance.deleteWhatsAppContactWithHttpInfo(contactId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#deleteWhatsAppContact");
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
| **contactId** | **String**| Contact ID | |

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
| **200** | Contact deleted successfully |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## deleteWhatsAppGroup

> RenameWhatsAppGroup200Response deleteWhatsAppGroup(deleteWhatsAppGroupRequest)

Delete group

**Deprecated.** Use contact tags via &#x60;PATCH /v1/contacts/{id}&#x60; instead. Delete a contact group. This removes the group from all contacts but does not delete the contacts themselves. 

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
        DeleteWhatsAppGroupRequest deleteWhatsAppGroupRequest = new DeleteWhatsAppGroupRequest(); // DeleteWhatsAppGroupRequest | 
        try {
            RenameWhatsAppGroup200Response result = apiInstance.deleteWhatsAppGroup(deleteWhatsAppGroupRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#deleteWhatsAppGroup");
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
| **deleteWhatsAppGroupRequest** | [**DeleteWhatsAppGroupRequest**](DeleteWhatsAppGroupRequest.md)|  | |

### Return type

[**RenameWhatsAppGroup200Response**](RenameWhatsAppGroup200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Group deleted successfully |  -  |
| **400** | Validation error (missing fields) |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |

## deleteWhatsAppGroupWithHttpInfo

> ApiResponse<RenameWhatsAppGroup200Response> deleteWhatsAppGroup deleteWhatsAppGroupWithHttpInfo(deleteWhatsAppGroupRequest)

Delete group

**Deprecated.** Use contact tags via &#x60;PATCH /v1/contacts/{id}&#x60; instead. Delete a contact group. This removes the group from all contacts but does not delete the contacts themselves. 

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
        DeleteWhatsAppGroupRequest deleteWhatsAppGroupRequest = new DeleteWhatsAppGroupRequest(); // DeleteWhatsAppGroupRequest | 
        try {
            ApiResponse<RenameWhatsAppGroup200Response> response = apiInstance.deleteWhatsAppGroupWithHttpInfo(deleteWhatsAppGroupRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#deleteWhatsAppGroup");
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
| **deleteWhatsAppGroupRequest** | [**DeleteWhatsAppGroupRequest**](DeleteWhatsAppGroupRequest.md)|  | |

### Return type

ApiResponse<[**RenameWhatsAppGroup200Response**](RenameWhatsAppGroup200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Group deleted successfully |  -  |
| **400** | Validation error (missing fields) |  -  |
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


## getWhatsAppBroadcast

> GetWhatsAppBroadcast200Response getWhatsAppBroadcast(broadcastId)

Get broadcast

**Deprecated.** Use &#x60;GET /v1/broadcasts/{id}&#x60; instead. Retrieve detailed information about a single broadcast including delivery statistics. 

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
        String broadcastId = "broadcastId_example"; // String | Broadcast ID
        try {
            GetWhatsAppBroadcast200Response result = apiInstance.getWhatsAppBroadcast(broadcastId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppBroadcast");
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
| **broadcastId** | **String**| Broadcast ID | |

### Return type

[**GetWhatsAppBroadcast200Response**](GetWhatsAppBroadcast200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Broadcast retrieved successfully |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## getWhatsAppBroadcastWithHttpInfo

> ApiResponse<GetWhatsAppBroadcast200Response> getWhatsAppBroadcast getWhatsAppBroadcastWithHttpInfo(broadcastId)

Get broadcast

**Deprecated.** Use &#x60;GET /v1/broadcasts/{id}&#x60; instead. Retrieve detailed information about a single broadcast including delivery statistics. 

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
        String broadcastId = "broadcastId_example"; // String | Broadcast ID
        try {
            ApiResponse<GetWhatsAppBroadcast200Response> response = apiInstance.getWhatsAppBroadcastWithHttpInfo(broadcastId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppBroadcast");
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
| **broadcastId** | **String**| Broadcast ID | |

### Return type

ApiResponse<[**GetWhatsAppBroadcast200Response**](GetWhatsAppBroadcast200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Broadcast retrieved successfully |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## getWhatsAppBroadcastRecipients

> GetWhatsAppBroadcastRecipients200Response getWhatsAppBroadcastRecipients(broadcastId, status, limit, skip)

List recipients

**Deprecated.** Use &#x60;GET /v1/broadcasts/{id}/recipients&#x60; instead. List recipients of a broadcast with their delivery status. Supports filtering by delivery status and pagination. 

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
        String broadcastId = "broadcastId_example"; // String | Broadcast ID
        String status = "pending"; // String | Filter by recipient delivery status
        Integer limit = 100; // Integer | Maximum results (default 100)
        Integer skip = 0; // Integer | Offset for pagination
        try {
            GetWhatsAppBroadcastRecipients200Response result = apiInstance.getWhatsAppBroadcastRecipients(broadcastId, status, limit, skip);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppBroadcastRecipients");
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
| **broadcastId** | **String**| Broadcast ID | |
| **status** | **String**| Filter by recipient delivery status | [optional] [enum: pending, sent, delivered, read, failed] |
| **limit** | **Integer**| Maximum results (default 100) | [optional] [default to 100] |
| **skip** | **Integer**| Offset for pagination | [optional] [default to 0] |

### Return type

[**GetWhatsAppBroadcastRecipients200Response**](GetWhatsAppBroadcastRecipients200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Recipients retrieved successfully |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## getWhatsAppBroadcastRecipientsWithHttpInfo

> ApiResponse<GetWhatsAppBroadcastRecipients200Response> getWhatsAppBroadcastRecipients getWhatsAppBroadcastRecipientsWithHttpInfo(broadcastId, status, limit, skip)

List recipients

**Deprecated.** Use &#x60;GET /v1/broadcasts/{id}/recipients&#x60; instead. List recipients of a broadcast with their delivery status. Supports filtering by delivery status and pagination. 

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
        String broadcastId = "broadcastId_example"; // String | Broadcast ID
        String status = "pending"; // String | Filter by recipient delivery status
        Integer limit = 100; // Integer | Maximum results (default 100)
        Integer skip = 0; // Integer | Offset for pagination
        try {
            ApiResponse<GetWhatsAppBroadcastRecipients200Response> response = apiInstance.getWhatsAppBroadcastRecipientsWithHttpInfo(broadcastId, status, limit, skip);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppBroadcastRecipients");
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
| **broadcastId** | **String**| Broadcast ID | |
| **status** | **String**| Filter by recipient delivery status | [optional] [enum: pending, sent, delivered, read, failed] |
| **limit** | **Integer**| Maximum results (default 100) | [optional] [default to 100] |
| **skip** | **Integer**| Offset for pagination | [optional] [default to 0] |

### Return type

ApiResponse<[**GetWhatsAppBroadcastRecipients200Response**](GetWhatsAppBroadcastRecipients200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Recipients retrieved successfully |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## getWhatsAppBroadcasts

> GetWhatsAppBroadcasts200Response getWhatsAppBroadcasts(accountId, status, limit, skip)

List broadcasts

**Deprecated.** Use &#x60;GET /v1/broadcasts?profileId&#x3D;{profileId}&#x60; instead. List all WhatsApp broadcasts for an account. Returns broadcasts sorted by creation date (newest first) without the full recipients list for performance. 

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
        String status = "draft"; // String | Filter by broadcast status
        Integer limit = 50; // Integer | Maximum results (default 50)
        Integer skip = 0; // Integer | Offset for pagination
        try {
            GetWhatsAppBroadcasts200Response result = apiInstance.getWhatsAppBroadcasts(accountId, status, limit, skip);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppBroadcasts");
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
| **status** | **String**| Filter by broadcast status | [optional] [enum: draft, scheduled, sending, completed, failed, cancelled] |
| **limit** | **Integer**| Maximum results (default 50) | [optional] [default to 50] |
| **skip** | **Integer**| Offset for pagination | [optional] [default to 0] |

### Return type

[**GetWhatsAppBroadcasts200Response**](GetWhatsAppBroadcasts200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Broadcasts retrieved successfully |  -  |
| **400** | accountId is required |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |

## getWhatsAppBroadcastsWithHttpInfo

> ApiResponse<GetWhatsAppBroadcasts200Response> getWhatsAppBroadcasts getWhatsAppBroadcastsWithHttpInfo(accountId, status, limit, skip)

List broadcasts

**Deprecated.** Use &#x60;GET /v1/broadcasts?profileId&#x3D;{profileId}&#x60; instead. List all WhatsApp broadcasts for an account. Returns broadcasts sorted by creation date (newest first) without the full recipients list for performance. 

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
        String status = "draft"; // String | Filter by broadcast status
        Integer limit = 50; // Integer | Maximum results (default 50)
        Integer skip = 0; // Integer | Offset for pagination
        try {
            ApiResponse<GetWhatsAppBroadcasts200Response> response = apiInstance.getWhatsAppBroadcastsWithHttpInfo(accountId, status, limit, skip);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppBroadcasts");
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
| **status** | **String**| Filter by broadcast status | [optional] [enum: draft, scheduled, sending, completed, failed, cancelled] |
| **limit** | **Integer**| Maximum results (default 50) | [optional] [default to 50] |
| **skip** | **Integer**| Offset for pagination | [optional] [default to 0] |

### Return type

ApiResponse<[**GetWhatsAppBroadcasts200Response**](GetWhatsAppBroadcasts200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Broadcasts retrieved successfully |  -  |
| **400** | accountId is required |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |


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


## getWhatsAppContact

> GetWhatsAppContact200Response getWhatsAppContact(contactId)

Get contact

**Deprecated.** Use &#x60;GET /v1/contacts/{id}&#x60; instead. Retrieve a single WhatsApp contact by ID with full details. 

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
        String contactId = "contactId_example"; // String | Contact ID
        try {
            GetWhatsAppContact200Response result = apiInstance.getWhatsAppContact(contactId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppContact");
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
| **contactId** | **String**| Contact ID | |

### Return type

[**GetWhatsAppContact200Response**](GetWhatsAppContact200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Contact retrieved successfully |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## getWhatsAppContactWithHttpInfo

> ApiResponse<GetWhatsAppContact200Response> getWhatsAppContact getWhatsAppContactWithHttpInfo(contactId)

Get contact

**Deprecated.** Use &#x60;GET /v1/contacts/{id}&#x60; instead. Retrieve a single WhatsApp contact by ID with full details. 

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
        String contactId = "contactId_example"; // String | Contact ID
        try {
            ApiResponse<GetWhatsAppContact200Response> response = apiInstance.getWhatsAppContactWithHttpInfo(contactId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppContact");
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
| **contactId** | **String**| Contact ID | |

### Return type

ApiResponse<[**GetWhatsAppContact200Response**](GetWhatsAppContact200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Contact retrieved successfully |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## getWhatsAppContacts

> GetWhatsAppContacts200Response getWhatsAppContacts(accountId, search, tag, group, optedIn, limit, skip)

List contacts

**Deprecated.** Use &#x60;GET /v1/contacts?profileId&#x3D;{profileId}&#x60; instead. List WhatsApp contacts for an account. Supports filtering by tags, groups, opt-in status, and text search. Returns contacts sorted by name with available filter options. 

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
        String search = "search_example"; // String | Search contacts by name, phone, email, or company
        String tag = "tag_example"; // String | Filter by tag
        String group = "group_example"; // String | Filter by group
        String optedIn = "true"; // String | Filter by opt-in status
        Integer limit = 50; // Integer | Maximum results (default 50)
        Integer skip = 0; // Integer | Offset for pagination
        try {
            GetWhatsAppContacts200Response result = apiInstance.getWhatsAppContacts(accountId, search, tag, group, optedIn, limit, skip);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppContacts");
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
| **search** | **String**| Search contacts by name, phone, email, or company | [optional] |
| **tag** | **String**| Filter by tag | [optional] |
| **group** | **String**| Filter by group | [optional] |
| **optedIn** | **String**| Filter by opt-in status | [optional] [enum: true, false] |
| **limit** | **Integer**| Maximum results (default 50) | [optional] [default to 50] |
| **skip** | **Integer**| Offset for pagination | [optional] [default to 0] |

### Return type

[**GetWhatsAppContacts200Response**](GetWhatsAppContacts200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Contacts retrieved successfully |  -  |
| **400** | accountId is required |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |

## getWhatsAppContactsWithHttpInfo

> ApiResponse<GetWhatsAppContacts200Response> getWhatsAppContacts getWhatsAppContactsWithHttpInfo(accountId, search, tag, group, optedIn, limit, skip)

List contacts

**Deprecated.** Use &#x60;GET /v1/contacts?profileId&#x3D;{profileId}&#x60; instead. List WhatsApp contacts for an account. Supports filtering by tags, groups, opt-in status, and text search. Returns contacts sorted by name with available filter options. 

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
        String search = "search_example"; // String | Search contacts by name, phone, email, or company
        String tag = "tag_example"; // String | Filter by tag
        String group = "group_example"; // String | Filter by group
        String optedIn = "true"; // String | Filter by opt-in status
        Integer limit = 50; // Integer | Maximum results (default 50)
        Integer skip = 0; // Integer | Offset for pagination
        try {
            ApiResponse<GetWhatsAppContacts200Response> response = apiInstance.getWhatsAppContactsWithHttpInfo(accountId, search, tag, group, optedIn, limit, skip);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppContacts");
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
| **search** | **String**| Search contacts by name, phone, email, or company | [optional] |
| **tag** | **String**| Filter by tag | [optional] |
| **group** | **String**| Filter by group | [optional] |
| **optedIn** | **String**| Filter by opt-in status | [optional] [enum: true, false] |
| **limit** | **Integer**| Maximum results (default 50) | [optional] [default to 50] |
| **skip** | **Integer**| Offset for pagination | [optional] [default to 0] |

### Return type

ApiResponse<[**GetWhatsAppContacts200Response**](GetWhatsAppContacts200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Contacts retrieved successfully |  -  |
| **400** | accountId is required |  -  |
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


## getWhatsAppGroups

> GetWhatsAppGroups200Response getWhatsAppGroups(accountId)

List contact groups

**Deprecated.** Use contact tags via &#x60;GET /v1/contacts&#x60; for grouping instead. WhatsApp groups have no cross-platform equivalent. List all contact groups for a WhatsApp account with contact counts. Groups are derived from the groups field on contacts, not stored as separate documents. 

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
            GetWhatsAppGroups200Response result = apiInstance.getWhatsAppGroups(accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppGroups");
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

[**GetWhatsAppGroups200Response**](GetWhatsAppGroups200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Groups retrieved successfully |  -  |
| **400** | accountId is required |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |

## getWhatsAppGroupsWithHttpInfo

> ApiResponse<GetWhatsAppGroups200Response> getWhatsAppGroups getWhatsAppGroupsWithHttpInfo(accountId)

List contact groups

**Deprecated.** Use contact tags via &#x60;GET /v1/contacts&#x60; for grouping instead. WhatsApp groups have no cross-platform equivalent. List all contact groups for a WhatsApp account with contact counts. Groups are derived from the groups field on contacts, not stored as separate documents. 

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
            ApiResponse<GetWhatsAppGroups200Response> response = apiInstance.getWhatsAppGroupsWithHttpInfo(accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#getWhatsAppGroups");
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

ApiResponse<[**GetWhatsAppGroups200Response**](GetWhatsAppGroups200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Groups retrieved successfully |  -  |
| **400** | accountId is required |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |


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


## importWhatsAppContacts

> ImportWhatsAppContacts200Response importWhatsAppContacts(importWhatsAppContactsRequest)

Bulk import contacts

**Deprecated.** Use &#x60;POST /v1/contacts/bulk&#x60; instead. Import up to 1000 contacts at once. Each contact requires a phone number and name. Duplicates are skipped by default. Supports default tags and groups applied to all imported contacts. 

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
        ImportWhatsAppContactsRequest importWhatsAppContactsRequest = new ImportWhatsAppContactsRequest(); // ImportWhatsAppContactsRequest | 
        try {
            ImportWhatsAppContacts200Response result = apiInstance.importWhatsAppContacts(importWhatsAppContactsRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#importWhatsAppContacts");
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
| **importWhatsAppContactsRequest** | [**ImportWhatsAppContactsRequest**](ImportWhatsAppContactsRequest.md)|  | |

### Return type

[**ImportWhatsAppContacts200Response**](ImportWhatsAppContacts200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Import completed |  -  |
| **400** | Validation error (missing fields |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |

## importWhatsAppContactsWithHttpInfo

> ApiResponse<ImportWhatsAppContacts200Response> importWhatsAppContacts importWhatsAppContactsWithHttpInfo(importWhatsAppContactsRequest)

Bulk import contacts

**Deprecated.** Use &#x60;POST /v1/contacts/bulk&#x60; instead. Import up to 1000 contacts at once. Each contact requires a phone number and name. Duplicates are skipped by default. Supports default tags and groups applied to all imported contacts. 

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
        ImportWhatsAppContactsRequest importWhatsAppContactsRequest = new ImportWhatsAppContactsRequest(); // ImportWhatsAppContactsRequest | 
        try {
            ApiResponse<ImportWhatsAppContacts200Response> response = apiInstance.importWhatsAppContactsWithHttpInfo(importWhatsAppContactsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#importWhatsAppContacts");
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
| **importWhatsAppContactsRequest** | [**ImportWhatsAppContactsRequest**](ImportWhatsAppContactsRequest.md)|  | |

### Return type

ApiResponse<[**ImportWhatsAppContacts200Response**](ImportWhatsAppContacts200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Import completed |  -  |
| **400** | Validation error (missing fields |  -  |
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


## removeWhatsAppBroadcastRecipients

> RemoveWhatsAppBroadcastRecipients200Response removeWhatsAppBroadcastRecipients(broadcastId, removeWhatsAppBroadcastRecipientsRequest)

Remove recipients

**Deprecated.** Use &#x60;POST /v1/broadcasts/{id}/recipients&#x60; with removal flag instead. Remove recipients from a draft broadcast by phone number. 

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
        String broadcastId = "broadcastId_example"; // String | Broadcast ID
        RemoveWhatsAppBroadcastRecipientsRequest removeWhatsAppBroadcastRecipientsRequest = new RemoveWhatsAppBroadcastRecipientsRequest(); // RemoveWhatsAppBroadcastRecipientsRequest | 
        try {
            RemoveWhatsAppBroadcastRecipients200Response result = apiInstance.removeWhatsAppBroadcastRecipients(broadcastId, removeWhatsAppBroadcastRecipientsRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#removeWhatsAppBroadcastRecipients");
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
| **broadcastId** | **String**| Broadcast ID | |
| **removeWhatsAppBroadcastRecipientsRequest** | [**RemoveWhatsAppBroadcastRecipientsRequest**](RemoveWhatsAppBroadcastRecipientsRequest.md)|  | |

### Return type

[**RemoveWhatsAppBroadcastRecipients200Response**](RemoveWhatsAppBroadcastRecipients200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Recipients removed successfully |  -  |
| **400** | Validation error or broadcast not in draft status |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## removeWhatsAppBroadcastRecipientsWithHttpInfo

> ApiResponse<RemoveWhatsAppBroadcastRecipients200Response> removeWhatsAppBroadcastRecipients removeWhatsAppBroadcastRecipientsWithHttpInfo(broadcastId, removeWhatsAppBroadcastRecipientsRequest)

Remove recipients

**Deprecated.** Use &#x60;POST /v1/broadcasts/{id}/recipients&#x60; with removal flag instead. Remove recipients from a draft broadcast by phone number. 

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
        String broadcastId = "broadcastId_example"; // String | Broadcast ID
        RemoveWhatsAppBroadcastRecipientsRequest removeWhatsAppBroadcastRecipientsRequest = new RemoveWhatsAppBroadcastRecipientsRequest(); // RemoveWhatsAppBroadcastRecipientsRequest | 
        try {
            ApiResponse<RemoveWhatsAppBroadcastRecipients200Response> response = apiInstance.removeWhatsAppBroadcastRecipientsWithHttpInfo(broadcastId, removeWhatsAppBroadcastRecipientsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#removeWhatsAppBroadcastRecipients");
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
| **broadcastId** | **String**| Broadcast ID | |
| **removeWhatsAppBroadcastRecipientsRequest** | [**RemoveWhatsAppBroadcastRecipientsRequest**](RemoveWhatsAppBroadcastRecipientsRequest.md)|  | |

### Return type

ApiResponse<[**RemoveWhatsAppBroadcastRecipients200Response**](RemoveWhatsAppBroadcastRecipients200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Recipients removed successfully |  -  |
| **400** | Validation error or broadcast not in draft status |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


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


## renameWhatsAppGroup

> RenameWhatsAppGroup200Response renameWhatsAppGroup(renameWhatsAppGroupRequest)

Rename group

**Deprecated.** Use contact tags via &#x60;PATCH /v1/contacts/{id}&#x60; instead. Rename a contact group. This updates the group name on all contacts that belong to the group. 

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
        RenameWhatsAppGroupRequest renameWhatsAppGroupRequest = new RenameWhatsAppGroupRequest(); // RenameWhatsAppGroupRequest | 
        try {
            RenameWhatsAppGroup200Response result = apiInstance.renameWhatsAppGroup(renameWhatsAppGroupRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#renameWhatsAppGroup");
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
| **renameWhatsAppGroupRequest** | [**RenameWhatsAppGroupRequest**](RenameWhatsAppGroupRequest.md)|  | |

### Return type

[**RenameWhatsAppGroup200Response**](RenameWhatsAppGroup200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Group renamed successfully |  -  |
| **400** | Validation error (missing fields |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |

## renameWhatsAppGroupWithHttpInfo

> ApiResponse<RenameWhatsAppGroup200Response> renameWhatsAppGroup renameWhatsAppGroupWithHttpInfo(renameWhatsAppGroupRequest)

Rename group

**Deprecated.** Use contact tags via &#x60;PATCH /v1/contacts/{id}&#x60; instead. Rename a contact group. This updates the group name on all contacts that belong to the group. 

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
        RenameWhatsAppGroupRequest renameWhatsAppGroupRequest = new RenameWhatsAppGroupRequest(); // RenameWhatsAppGroupRequest | 
        try {
            ApiResponse<RenameWhatsAppGroup200Response> response = apiInstance.renameWhatsAppGroupWithHttpInfo(renameWhatsAppGroupRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#renameWhatsAppGroup");
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
| **renameWhatsAppGroupRequest** | [**RenameWhatsAppGroupRequest**](RenameWhatsAppGroupRequest.md)|  | |

### Return type

ApiResponse<[**RenameWhatsAppGroup200Response**](RenameWhatsAppGroup200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Group renamed successfully |  -  |
| **400** | Validation error (missing fields |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |


## scheduleWhatsAppBroadcast

> ScheduleWhatsAppBroadcast200Response scheduleWhatsAppBroadcast(broadcastId, scheduleWhatsAppBroadcastRequest)

Schedule broadcast

**Deprecated.** Use &#x60;POST /v1/broadcasts/{id}/schedule&#x60; instead. Schedule a draft broadcast for future sending. The scheduled time must be in the future and no more than 30 days in advance. The broadcast must be in draft status and have recipients. 

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
        String broadcastId = "broadcastId_example"; // String | Broadcast ID
        ScheduleWhatsAppBroadcastRequest scheduleWhatsAppBroadcastRequest = new ScheduleWhatsAppBroadcastRequest(); // ScheduleWhatsAppBroadcastRequest | 
        try {
            ScheduleWhatsAppBroadcast200Response result = apiInstance.scheduleWhatsAppBroadcast(broadcastId, scheduleWhatsAppBroadcastRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#scheduleWhatsAppBroadcast");
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
| **broadcastId** | **String**| Broadcast ID | |
| **scheduleWhatsAppBroadcastRequest** | [**ScheduleWhatsAppBroadcastRequest**](ScheduleWhatsAppBroadcastRequest.md)|  | |

### Return type

[**ScheduleWhatsAppBroadcast200Response**](ScheduleWhatsAppBroadcast200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Broadcast scheduled successfully |  -  |
| **400** | Invalid schedule time or broadcast not in draft status |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## scheduleWhatsAppBroadcastWithHttpInfo

> ApiResponse<ScheduleWhatsAppBroadcast200Response> scheduleWhatsAppBroadcast scheduleWhatsAppBroadcastWithHttpInfo(broadcastId, scheduleWhatsAppBroadcastRequest)

Schedule broadcast

**Deprecated.** Use &#x60;POST /v1/broadcasts/{id}/schedule&#x60; instead. Schedule a draft broadcast for future sending. The scheduled time must be in the future and no more than 30 days in advance. The broadcast must be in draft status and have recipients. 

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
        String broadcastId = "broadcastId_example"; // String | Broadcast ID
        ScheduleWhatsAppBroadcastRequest scheduleWhatsAppBroadcastRequest = new ScheduleWhatsAppBroadcastRequest(); // ScheduleWhatsAppBroadcastRequest | 
        try {
            ApiResponse<ScheduleWhatsAppBroadcast200Response> response = apiInstance.scheduleWhatsAppBroadcastWithHttpInfo(broadcastId, scheduleWhatsAppBroadcastRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#scheduleWhatsAppBroadcast");
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
| **broadcastId** | **String**| Broadcast ID | |
| **scheduleWhatsAppBroadcastRequest** | [**ScheduleWhatsAppBroadcastRequest**](ScheduleWhatsAppBroadcastRequest.md)|  | |

### Return type

ApiResponse<[**ScheduleWhatsAppBroadcast200Response**](ScheduleWhatsAppBroadcast200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Broadcast scheduled successfully |  -  |
| **400** | Invalid schedule time or broadcast not in draft status |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## sendWhatsAppBroadcast

> SendWhatsAppBroadcast200Response sendWhatsAppBroadcast(broadcastId)

Send broadcast

**Deprecated.** Use &#x60;POST /v1/broadcasts/{id}/send&#x60; instead. Start sending a broadcast immediately. The broadcast must be in draft or scheduled status and have at least one recipient. Messages are sent sequentially with rate limiting. 

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
        String broadcastId = "broadcastId_example"; // String | Broadcast ID
        try {
            SendWhatsAppBroadcast200Response result = apiInstance.sendWhatsAppBroadcast(broadcastId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#sendWhatsAppBroadcast");
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
| **broadcastId** | **String**| Broadcast ID | |

### Return type

[**SendWhatsAppBroadcast200Response**](SendWhatsAppBroadcast200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Broadcast send completed |  -  |
| **400** | Invalid broadcast status or no recipients |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## sendWhatsAppBroadcastWithHttpInfo

> ApiResponse<SendWhatsAppBroadcast200Response> sendWhatsAppBroadcast sendWhatsAppBroadcastWithHttpInfo(broadcastId)

Send broadcast

**Deprecated.** Use &#x60;POST /v1/broadcasts/{id}/send&#x60; instead. Start sending a broadcast immediately. The broadcast must be in draft or scheduled status and have at least one recipient. Messages are sent sequentially with rate limiting. 

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
        String broadcastId = "broadcastId_example"; // String | Broadcast ID
        try {
            ApiResponse<SendWhatsAppBroadcast200Response> response = apiInstance.sendWhatsAppBroadcastWithHttpInfo(broadcastId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#sendWhatsAppBroadcast");
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
| **broadcastId** | **String**| Broadcast ID | |

### Return type

ApiResponse<[**SendWhatsAppBroadcast200Response**](SendWhatsAppBroadcast200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Broadcast send completed |  -  |
| **400** | Invalid broadcast status or no recipients |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## sendWhatsAppBulk

> SendWhatsAppBulk200Response sendWhatsAppBulk(sendWhatsAppBulkRequest)

Bulk send template messages

**Deprecated.** Use &#x60;POST /v1/broadcasts&#x60; to create a broadcast, &#x60;POST /v1/broadcasts/{id}/recipients&#x60; to add recipients, then &#x60;POST /v1/broadcasts/{id}/send&#x60; to send. Send a template message to multiple recipients in a single request. Maximum 100 recipients per request. Only template messages are supported for bulk sending (not free-form text).  Each recipient can have optional per-recipient template variables for personalization. Returns detailed results for each recipient. 

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
        SendWhatsAppBulkRequest sendWhatsAppBulkRequest = new SendWhatsAppBulkRequest(); // SendWhatsAppBulkRequest | 
        try {
            SendWhatsAppBulk200Response result = apiInstance.sendWhatsAppBulk(sendWhatsAppBulkRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#sendWhatsAppBulk");
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
| **sendWhatsAppBulkRequest** | [**SendWhatsAppBulkRequest**](SendWhatsAppBulkRequest.md)|  | |

### Return type

[**SendWhatsAppBulk200Response**](SendWhatsAppBulk200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Bulk send completed |  -  |
| **400** | Validation error (missing fields |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |

## sendWhatsAppBulkWithHttpInfo

> ApiResponse<SendWhatsAppBulk200Response> sendWhatsAppBulk sendWhatsAppBulkWithHttpInfo(sendWhatsAppBulkRequest)

Bulk send template messages

**Deprecated.** Use &#x60;POST /v1/broadcasts&#x60; to create a broadcast, &#x60;POST /v1/broadcasts/{id}/recipients&#x60; to add recipients, then &#x60;POST /v1/broadcasts/{id}/send&#x60; to send. Send a template message to multiple recipients in a single request. Maximum 100 recipients per request. Only template messages are supported for bulk sending (not free-form text).  Each recipient can have optional per-recipient template variables for personalization. Returns detailed results for each recipient. 

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
        SendWhatsAppBulkRequest sendWhatsAppBulkRequest = new SendWhatsAppBulkRequest(); // SendWhatsAppBulkRequest | 
        try {
            ApiResponse<SendWhatsAppBulk200Response> response = apiInstance.sendWhatsAppBulkWithHttpInfo(sendWhatsAppBulkRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#sendWhatsAppBulk");
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
| **sendWhatsAppBulkRequest** | [**SendWhatsAppBulkRequest**](SendWhatsAppBulkRequest.md)|  | |

### Return type

ApiResponse<[**SendWhatsAppBulk200Response**](SendWhatsAppBulk200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Bulk send completed |  -  |
| **400** | Validation error (missing fields |  -  |
| **401** | Unauthorized |  -  |
| **404** | WhatsApp account not found |  -  |


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


## updateWhatsAppContact

> UpdateWhatsAppContact200Response updateWhatsAppContact(contactId, updateWhatsAppContactRequest)

Update contact

**Deprecated.** Use &#x60;PATCH /v1/contacts/{id}&#x60; instead. Update an existing WhatsApp contact. All fields are optional; only provided fields will be updated. Custom fields are merged with existing values. Set a custom field to null to remove it. 

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
        String contactId = "contactId_example"; // String | Contact ID
        UpdateWhatsAppContactRequest updateWhatsAppContactRequest = new UpdateWhatsAppContactRequest(); // UpdateWhatsAppContactRequest | 
        try {
            UpdateWhatsAppContact200Response result = apiInstance.updateWhatsAppContact(contactId, updateWhatsAppContactRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#updateWhatsAppContact");
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
| **contactId** | **String**| Contact ID | |
| **updateWhatsAppContactRequest** | [**UpdateWhatsAppContactRequest**](UpdateWhatsAppContactRequest.md)|  | |

### Return type

[**UpdateWhatsAppContact200Response**](UpdateWhatsAppContact200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Contact updated successfully |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## updateWhatsAppContactWithHttpInfo

> ApiResponse<UpdateWhatsAppContact200Response> updateWhatsAppContact updateWhatsAppContactWithHttpInfo(contactId, updateWhatsAppContactRequest)

Update contact

**Deprecated.** Use &#x60;PATCH /v1/contacts/{id}&#x60; instead. Update an existing WhatsApp contact. All fields are optional; only provided fields will be updated. Custom fields are merged with existing values. Set a custom field to null to remove it. 

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
        String contactId = "contactId_example"; // String | Contact ID
        UpdateWhatsAppContactRequest updateWhatsAppContactRequest = new UpdateWhatsAppContactRequest(); // UpdateWhatsAppContactRequest | 
        try {
            ApiResponse<UpdateWhatsAppContact200Response> response = apiInstance.updateWhatsAppContactWithHttpInfo(contactId, updateWhatsAppContactRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppApi#updateWhatsAppContact");
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
| **contactId** | **String**| Contact ID | |
| **updateWhatsAppContactRequest** | [**UpdateWhatsAppContactRequest**](UpdateWhatsAppContactRequest.md)|  | |

### Return type

ApiResponse<[**UpdateWhatsAppContact200Response**](UpdateWhatsAppContact200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Contact updated successfully |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


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

