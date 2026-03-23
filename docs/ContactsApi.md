# ContactsApi

All URIs are relative to *https://zernio.com/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**bulkCreateContacts**](ContactsApi.md#bulkCreateContacts) | **POST** /v1/contacts/bulk | Bulk create contacts |
| [**bulkCreateContactsWithHttpInfo**](ContactsApi.md#bulkCreateContactsWithHttpInfo) | **POST** /v1/contacts/bulk | Bulk create contacts |
| [**createContact**](ContactsApi.md#createContact) | **POST** /v1/contacts | Create a contact |
| [**createContactWithHttpInfo**](ContactsApi.md#createContactWithHttpInfo) | **POST** /v1/contacts | Create a contact |
| [**deleteContact**](ContactsApi.md#deleteContact) | **DELETE** /v1/contacts/{contactId} | Delete a contact |
| [**deleteContactWithHttpInfo**](ContactsApi.md#deleteContactWithHttpInfo) | **DELETE** /v1/contacts/{contactId} | Delete a contact |
| [**getContact**](ContactsApi.md#getContact) | **GET** /v1/contacts/{contactId} | Get contact with channels |
| [**getContactWithHttpInfo**](ContactsApi.md#getContactWithHttpInfo) | **GET** /v1/contacts/{contactId} | Get contact with channels |
| [**getContactChannels**](ContactsApi.md#getContactChannels) | **GET** /v1/contacts/{contactId}/channels | List channels for a contact |
| [**getContactChannelsWithHttpInfo**](ContactsApi.md#getContactChannelsWithHttpInfo) | **GET** /v1/contacts/{contactId}/channels | List channels for a contact |
| [**listContacts**](ContactsApi.md#listContacts) | **GET** /v1/contacts | List contacts |
| [**listContactsWithHttpInfo**](ContactsApi.md#listContactsWithHttpInfo) | **GET** /v1/contacts | List contacts |
| [**updateContact**](ContactsApi.md#updateContact) | **PATCH** /v1/contacts/{contactId} | Update a contact |
| [**updateContactWithHttpInfo**](ContactsApi.md#updateContactWithHttpInfo) | **PATCH** /v1/contacts/{contactId} | Update a contact |



## bulkCreateContacts

> void bulkCreateContacts(bulkCreateContactsRequest)

Bulk create contacts

Import up to 1000 contacts at a time. Skips duplicates.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ContactsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ContactsApi apiInstance = new ContactsApi(defaultClient);
        BulkCreateContactsRequest bulkCreateContactsRequest = new BulkCreateContactsRequest(); // BulkCreateContactsRequest | 
        try {
            apiInstance.bulkCreateContacts(bulkCreateContactsRequest);
        } catch (ApiException e) {
            System.err.println("Exception when calling ContactsApi#bulkCreateContacts");
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
| **bulkCreateContactsRequest** | [**BulkCreateContactsRequest**](BulkCreateContactsRequest.md)|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Bulk import results |  -  |
| **401** | Unauthorized |  -  |

## bulkCreateContactsWithHttpInfo

> ApiResponse<Void> bulkCreateContacts bulkCreateContactsWithHttpInfo(bulkCreateContactsRequest)

Bulk create contacts

Import up to 1000 contacts at a time. Skips duplicates.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ContactsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ContactsApi apiInstance = new ContactsApi(defaultClient);
        BulkCreateContactsRequest bulkCreateContactsRequest = new BulkCreateContactsRequest(); // BulkCreateContactsRequest | 
        try {
            ApiResponse<Void> response = apiInstance.bulkCreateContactsWithHttpInfo(bulkCreateContactsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling ContactsApi#bulkCreateContacts");
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
| **bulkCreateContactsRequest** | [**BulkCreateContactsRequest**](BulkCreateContactsRequest.md)|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Bulk import results |  -  |
| **401** | Unauthorized |  -  |


## createContact

> void createContact(createContactRequest)

Create a contact

Create a new contact. Optionally create a platform channel in the same request by providing accountId, platform, and platformIdentifier.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ContactsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ContactsApi apiInstance = new ContactsApi(defaultClient);
        CreateContactRequest createContactRequest = new CreateContactRequest(); // CreateContactRequest | 
        try {
            apiInstance.createContact(createContactRequest);
        } catch (ApiException e) {
            System.err.println("Exception when calling ContactsApi#createContact");
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
| **createContactRequest** | [**CreateContactRequest**](CreateContactRequest.md)|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Contact created |  -  |
| **401** | Unauthorized |  -  |
| **409** | Duplicate contact |  -  |

## createContactWithHttpInfo

> ApiResponse<Void> createContact createContactWithHttpInfo(createContactRequest)

Create a contact

Create a new contact. Optionally create a platform channel in the same request by providing accountId, platform, and platformIdentifier.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ContactsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ContactsApi apiInstance = new ContactsApi(defaultClient);
        CreateContactRequest createContactRequest = new CreateContactRequest(); // CreateContactRequest | 
        try {
            ApiResponse<Void> response = apiInstance.createContactWithHttpInfo(createContactRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling ContactsApi#createContact");
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
| **createContactRequest** | [**CreateContactRequest**](CreateContactRequest.md)|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Contact created |  -  |
| **401** | Unauthorized |  -  |
| **409** | Duplicate contact |  -  |


## deleteContact

> void deleteContact(contactId)

Delete a contact

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ContactsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ContactsApi apiInstance = new ContactsApi(defaultClient);
        String contactId = "contactId_example"; // String | 
        try {
            apiInstance.deleteContact(contactId);
        } catch (ApiException e) {
            System.err.println("Exception when calling ContactsApi#deleteContact");
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
| **contactId** | **String**|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Contact deleted |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## deleteContactWithHttpInfo

> ApiResponse<Void> deleteContact deleteContactWithHttpInfo(contactId)

Delete a contact

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ContactsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ContactsApi apiInstance = new ContactsApi(defaultClient);
        String contactId = "contactId_example"; // String | 
        try {
            ApiResponse<Void> response = apiInstance.deleteContactWithHttpInfo(contactId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling ContactsApi#deleteContact");
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
| **contactId** | **String**|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Contact deleted |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## getContact

> void getContact(contactId)

Get contact with channels

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ContactsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ContactsApi apiInstance = new ContactsApi(defaultClient);
        String contactId = "contactId_example"; // String | 
        try {
            apiInstance.getContact(contactId);
        } catch (ApiException e) {
            System.err.println("Exception when calling ContactsApi#getContact");
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
| **contactId** | **String**|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Contact with channels |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## getContactWithHttpInfo

> ApiResponse<Void> getContact getContactWithHttpInfo(contactId)

Get contact with channels

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ContactsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ContactsApi apiInstance = new ContactsApi(defaultClient);
        String contactId = "contactId_example"; // String | 
        try {
            ApiResponse<Void> response = apiInstance.getContactWithHttpInfo(contactId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling ContactsApi#getContact");
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
| **contactId** | **String**|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Contact with channels |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## getContactChannels

> void getContactChannels(contactId)

List channels for a contact

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ContactsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ContactsApi apiInstance = new ContactsApi(defaultClient);
        String contactId = "contactId_example"; // String | 
        try {
            apiInstance.getContactChannels(contactId);
        } catch (ApiException e) {
            System.err.println("Exception when calling ContactsApi#getContactChannels");
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
| **contactId** | **String**|  | |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of contact channels |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## getContactChannelsWithHttpInfo

> ApiResponse<Void> getContactChannels getContactChannelsWithHttpInfo(contactId)

List channels for a contact

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ContactsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ContactsApi apiInstance = new ContactsApi(defaultClient);
        String contactId = "contactId_example"; // String | 
        try {
            ApiResponse<Void> response = apiInstance.getContactChannelsWithHttpInfo(contactId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling ContactsApi#getContactChannels");
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
| **contactId** | **String**|  | |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of contact channels |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## listContacts

> void listContacts(profileId, search, tag, platform, isSubscribed, limit, skip)

List contacts

List and search contacts for a profile. Supports filtering by tags, platform, subscription status, and full-text search.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ContactsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ContactsApi apiInstance = new ContactsApi(defaultClient);
        String profileId = "profileId_example"; // String | Filter by profile. Omit to list across all profiles
        String search = "search_example"; // String | 
        String tag = "tag_example"; // String | 
        String platform = "instagram"; // String | 
        String isSubscribed = "true"; // String | 
        Integer limit = 50; // Integer | 
        Integer skip = 0; // Integer | 
        try {
            apiInstance.listContacts(profileId, search, tag, platform, isSubscribed, limit, skip);
        } catch (ApiException e) {
            System.err.println("Exception when calling ContactsApi#listContacts");
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
| **profileId** | **String**| Filter by profile. Omit to list across all profiles | [optional] |
| **search** | **String**|  | [optional] |
| **tag** | **String**|  | [optional] |
| **platform** | **String**|  | [optional] [enum: instagram, facebook, telegram, twitter, bluesky, reddit, whatsapp] |
| **isSubscribed** | **String**|  | [optional] [enum: true, false] |
| **limit** | **Integer**|  | [optional] [default to 50] |
| **skip** | **Integer**|  | [optional] [default to 0] |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Contacts list with pagination and filter metadata |  -  |
| **401** | Unauthorized |  -  |

## listContactsWithHttpInfo

> ApiResponse<Void> listContacts listContactsWithHttpInfo(profileId, search, tag, platform, isSubscribed, limit, skip)

List contacts

List and search contacts for a profile. Supports filtering by tags, platform, subscription status, and full-text search.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ContactsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ContactsApi apiInstance = new ContactsApi(defaultClient);
        String profileId = "profileId_example"; // String | Filter by profile. Omit to list across all profiles
        String search = "search_example"; // String | 
        String tag = "tag_example"; // String | 
        String platform = "instagram"; // String | 
        String isSubscribed = "true"; // String | 
        Integer limit = 50; // Integer | 
        Integer skip = 0; // Integer | 
        try {
            ApiResponse<Void> response = apiInstance.listContactsWithHttpInfo(profileId, search, tag, platform, isSubscribed, limit, skip);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling ContactsApi#listContacts");
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
| **profileId** | **String**| Filter by profile. Omit to list across all profiles | [optional] |
| **search** | **String**|  | [optional] |
| **tag** | **String**|  | [optional] |
| **platform** | **String**|  | [optional] [enum: instagram, facebook, telegram, twitter, bluesky, reddit, whatsapp] |
| **isSubscribed** | **String**|  | [optional] [enum: true, false] |
| **limit** | **Integer**|  | [optional] [default to 50] |
| **skip** | **Integer**|  | [optional] [default to 0] |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Contacts list with pagination and filter metadata |  -  |
| **401** | Unauthorized |  -  |


## updateContact

> void updateContact(contactId, updateContactRequest)

Update a contact

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ContactsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ContactsApi apiInstance = new ContactsApi(defaultClient);
        String contactId = "contactId_example"; // String | 
        UpdateContactRequest updateContactRequest = new UpdateContactRequest(); // UpdateContactRequest | 
        try {
            apiInstance.updateContact(contactId, updateContactRequest);
        } catch (ApiException e) {
            System.err.println("Exception when calling ContactsApi#updateContact");
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
| **contactId** | **String**|  | |
| **updateContactRequest** | [**UpdateContactRequest**](UpdateContactRequest.md)|  | [optional] |

### Return type


null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Contact updated |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## updateContactWithHttpInfo

> ApiResponse<Void> updateContact updateContactWithHttpInfo(contactId, updateContactRequest)

Update a contact

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ContactsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ContactsApi apiInstance = new ContactsApi(defaultClient);
        String contactId = "contactId_example"; // String | 
        UpdateContactRequest updateContactRequest = new UpdateContactRequest(); // UpdateContactRequest | 
        try {
            ApiResponse<Void> response = apiInstance.updateContactWithHttpInfo(contactId, updateContactRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling ContactsApi#updateContact");
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
| **contactId** | **String**|  | |
| **updateContactRequest** | [**UpdateContactRequest**](UpdateContactRequest.md)|  | [optional] |

### Return type


ApiResponse<Void>

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Contact updated |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

