# AccountGroupsApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createAccountGroup**](AccountGroupsApi.md#createAccountGroup) | **POST** /v1/account-groups | Create group |
| [**createAccountGroupWithHttpInfo**](AccountGroupsApi.md#createAccountGroupWithHttpInfo) | **POST** /v1/account-groups | Create group |
| [**deleteAccountGroup**](AccountGroupsApi.md#deleteAccountGroup) | **DELETE** /v1/account-groups/{groupId} | Delete group |
| [**deleteAccountGroupWithHttpInfo**](AccountGroupsApi.md#deleteAccountGroupWithHttpInfo) | **DELETE** /v1/account-groups/{groupId} | Delete group |
| [**listAccountGroups**](AccountGroupsApi.md#listAccountGroups) | **GET** /v1/account-groups | List groups |
| [**listAccountGroupsWithHttpInfo**](AccountGroupsApi.md#listAccountGroupsWithHttpInfo) | **GET** /v1/account-groups | List groups |
| [**updateAccountGroup**](AccountGroupsApi.md#updateAccountGroup) | **PUT** /v1/account-groups/{groupId} | Update group |
| [**updateAccountGroupWithHttpInfo**](AccountGroupsApi.md#updateAccountGroupWithHttpInfo) | **PUT** /v1/account-groups/{groupId} | Update group |



## createAccountGroup

> CreateAccountGroup201Response createAccountGroup(createAccountGroupRequest)

Create group

Creates a new account group with a name and a list of social account IDs.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AccountGroupsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AccountGroupsApi apiInstance = new AccountGroupsApi(defaultClient);
        CreateAccountGroupRequest createAccountGroupRequest = new CreateAccountGroupRequest(); // CreateAccountGroupRequest | 
        try {
            CreateAccountGroup201Response result = apiInstance.createAccountGroup(createAccountGroupRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AccountGroupsApi#createAccountGroup");
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
| **createAccountGroupRequest** | [**CreateAccountGroupRequest**](CreateAccountGroupRequest.md)|  | |

### Return type

[**CreateAccountGroup201Response**](CreateAccountGroup201Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Created |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |
| **409** | Group name already exists |  -  |

## createAccountGroupWithHttpInfo

> ApiResponse<CreateAccountGroup201Response> createAccountGroup createAccountGroupWithHttpInfo(createAccountGroupRequest)

Create group

Creates a new account group with a name and a list of social account IDs.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AccountGroupsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AccountGroupsApi apiInstance = new AccountGroupsApi(defaultClient);
        CreateAccountGroupRequest createAccountGroupRequest = new CreateAccountGroupRequest(); // CreateAccountGroupRequest | 
        try {
            ApiResponse<CreateAccountGroup201Response> response = apiInstance.createAccountGroupWithHttpInfo(createAccountGroupRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AccountGroupsApi#createAccountGroup");
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
| **createAccountGroupRequest** | [**CreateAccountGroupRequest**](CreateAccountGroupRequest.md)|  | |

### Return type

ApiResponse<[**CreateAccountGroup201Response**](CreateAccountGroup201Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Created |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |
| **409** | Group name already exists |  -  |


## deleteAccountGroup

> DeleteAccountGroup200Response deleteAccountGroup(groupId)

Delete group

Permanently deletes an account group. The accounts themselves are not affected.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AccountGroupsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AccountGroupsApi apiInstance = new AccountGroupsApi(defaultClient);
        String groupId = "groupId_example"; // String | 
        try {
            DeleteAccountGroup200Response result = apiInstance.deleteAccountGroup(groupId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AccountGroupsApi#deleteAccountGroup");
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
| **groupId** | **String**|  | |

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
| **200** | Deleted |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## deleteAccountGroupWithHttpInfo

> ApiResponse<DeleteAccountGroup200Response> deleteAccountGroup deleteAccountGroupWithHttpInfo(groupId)

Delete group

Permanently deletes an account group. The accounts themselves are not affected.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AccountGroupsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AccountGroupsApi apiInstance = new AccountGroupsApi(defaultClient);
        String groupId = "groupId_example"; // String | 
        try {
            ApiResponse<DeleteAccountGroup200Response> response = apiInstance.deleteAccountGroupWithHttpInfo(groupId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AccountGroupsApi#deleteAccountGroup");
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
| **groupId** | **String**|  | |

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
| **200** | Deleted |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## listAccountGroups

> ListAccountGroups200Response listAccountGroups()

List groups

Returns all account groups for the authenticated user, including group names and associated account IDs.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AccountGroupsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AccountGroupsApi apiInstance = new AccountGroupsApi(defaultClient);
        try {
            ListAccountGroups200Response result = apiInstance.listAccountGroups();
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AccountGroupsApi#listAccountGroups");
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

[**ListAccountGroups200Response**](ListAccountGroups200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Groups |  -  |
| **401** | Unauthorized |  -  |

## listAccountGroupsWithHttpInfo

> ApiResponse<ListAccountGroups200Response> listAccountGroups listAccountGroupsWithHttpInfo()

List groups

Returns all account groups for the authenticated user, including group names and associated account IDs.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AccountGroupsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AccountGroupsApi apiInstance = new AccountGroupsApi(defaultClient);
        try {
            ApiResponse<ListAccountGroups200Response> response = apiInstance.listAccountGroupsWithHttpInfo();
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AccountGroupsApi#listAccountGroups");
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

ApiResponse<[**ListAccountGroups200Response**](ListAccountGroups200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Groups |  -  |
| **401** | Unauthorized |  -  |


## updateAccountGroup

> UpdateAccountGroup200Response updateAccountGroup(groupId, updateAccountGroupRequest)

Update group

Updates the name or account list of an existing group. You can rename the group, change its accounts, or both.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AccountGroupsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AccountGroupsApi apiInstance = new AccountGroupsApi(defaultClient);
        String groupId = "groupId_example"; // String | 
        UpdateAccountGroupRequest updateAccountGroupRequest = new UpdateAccountGroupRequest(); // UpdateAccountGroupRequest | 
        try {
            UpdateAccountGroup200Response result = apiInstance.updateAccountGroup(groupId, updateAccountGroupRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AccountGroupsApi#updateAccountGroup");
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
| **groupId** | **String**|  | |
| **updateAccountGroupRequest** | [**UpdateAccountGroupRequest**](UpdateAccountGroupRequest.md)|  | |

### Return type

[**UpdateAccountGroup200Response**](UpdateAccountGroup200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **409** | Group name already exists |  -  |

## updateAccountGroupWithHttpInfo

> ApiResponse<UpdateAccountGroup200Response> updateAccountGroup updateAccountGroupWithHttpInfo(groupId, updateAccountGroupRequest)

Update group

Updates the name or account list of an existing group. You can rename the group, change its accounts, or both.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.AccountGroupsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        AccountGroupsApi apiInstance = new AccountGroupsApi(defaultClient);
        String groupId = "groupId_example"; // String | 
        UpdateAccountGroupRequest updateAccountGroupRequest = new UpdateAccountGroupRequest(); // UpdateAccountGroupRequest | 
        try {
            ApiResponse<UpdateAccountGroup200Response> response = apiInstance.updateAccountGroupWithHttpInfo(groupId, updateAccountGroupRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling AccountGroupsApi#updateAccountGroup");
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
| **groupId** | **String**|  | |
| **updateAccountGroupRequest** | [**UpdateAccountGroupRequest**](UpdateAccountGroupRequest.md)|  | |

### Return type

ApiResponse<[**UpdateAccountGroup200Response**](UpdateAccountGroup200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **409** | Group name already exists |  -  |

