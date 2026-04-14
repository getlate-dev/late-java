# CustomFieldsApi

All URIs are relative to *https://zernio.com/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**clearContactFieldValue**](CustomFieldsApi.md#clearContactFieldValue) | **DELETE** /v1/contacts/{contactId}/fields/{slug} | Clear custom field value |
| [**clearContactFieldValueWithHttpInfo**](CustomFieldsApi.md#clearContactFieldValueWithHttpInfo) | **DELETE** /v1/contacts/{contactId}/fields/{slug} | Clear custom field value |
| [**createCustomField**](CustomFieldsApi.md#createCustomField) | **POST** /v1/custom-fields | Create custom field |
| [**createCustomFieldWithHttpInfo**](CustomFieldsApi.md#createCustomFieldWithHttpInfo) | **POST** /v1/custom-fields | Create custom field |
| [**deleteCustomField**](CustomFieldsApi.md#deleteCustomField) | **DELETE** /v1/custom-fields/{fieldId} | Delete custom field |
| [**deleteCustomFieldWithHttpInfo**](CustomFieldsApi.md#deleteCustomFieldWithHttpInfo) | **DELETE** /v1/custom-fields/{fieldId} | Delete custom field |
| [**listCustomFields**](CustomFieldsApi.md#listCustomFields) | **GET** /v1/custom-fields | List custom field definitions |
| [**listCustomFieldsWithHttpInfo**](CustomFieldsApi.md#listCustomFieldsWithHttpInfo) | **GET** /v1/custom-fields | List custom field definitions |
| [**setContactFieldValue**](CustomFieldsApi.md#setContactFieldValue) | **PUT** /v1/contacts/{contactId}/fields/{slug} | Set custom field value |
| [**setContactFieldValueWithHttpInfo**](CustomFieldsApi.md#setContactFieldValueWithHttpInfo) | **PUT** /v1/contacts/{contactId}/fields/{slug} | Set custom field value |
| [**updateCustomField**](CustomFieldsApi.md#updateCustomField) | **PATCH** /v1/custom-fields/{fieldId} | Update custom field |
| [**updateCustomFieldWithHttpInfo**](CustomFieldsApi.md#updateCustomFieldWithHttpInfo) | **PATCH** /v1/custom-fields/{fieldId} | Update custom field |



## clearContactFieldValue

> void clearContactFieldValue(contactId, slug)

Clear custom field value

Remove a custom field value from a contact. The field definition is not affected.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CustomFieldsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CustomFieldsApi apiInstance = new CustomFieldsApi(defaultClient);
        String contactId = "contactId_example"; // String | 
        String slug = "slug_example"; // String | 
        try {
            apiInstance.clearContactFieldValue(contactId, slug);
        } catch (ApiException e) {
            System.err.println("Exception when calling CustomFieldsApi#clearContactFieldValue");
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
| **slug** | **String**|  | |

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
| **200** | Field value cleared |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## clearContactFieldValueWithHttpInfo

> ApiResponse<Void> clearContactFieldValue clearContactFieldValueWithHttpInfo(contactId, slug)

Clear custom field value

Remove a custom field value from a contact. The field definition is not affected.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CustomFieldsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CustomFieldsApi apiInstance = new CustomFieldsApi(defaultClient);
        String contactId = "contactId_example"; // String | 
        String slug = "slug_example"; // String | 
        try {
            ApiResponse<Void> response = apiInstance.clearContactFieldValueWithHttpInfo(contactId, slug);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling CustomFieldsApi#clearContactFieldValue");
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
| **slug** | **String**|  | |

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
| **200** | Field value cleared |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## createCustomField

> CreateCustomField200Response createCustomField(createCustomFieldRequest)

Create custom field

Create a new custom field definition. Supported types are text, number, date, boolean, and select.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CustomFieldsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CustomFieldsApi apiInstance = new CustomFieldsApi(defaultClient);
        CreateCustomFieldRequest createCustomFieldRequest = new CreateCustomFieldRequest(); // CreateCustomFieldRequest | 
        try {
            CreateCustomField200Response result = apiInstance.createCustomField(createCustomFieldRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling CustomFieldsApi#createCustomField");
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
| **createCustomFieldRequest** | [**CreateCustomFieldRequest**](CreateCustomFieldRequest.md)|  | |

### Return type

[**CreateCustomField200Response**](CreateCustomField200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Custom field created |  -  |
| **401** | Unauthorized |  -  |
| **409** | Duplicate slug |  -  |

## createCustomFieldWithHttpInfo

> ApiResponse<CreateCustomField200Response> createCustomField createCustomFieldWithHttpInfo(createCustomFieldRequest)

Create custom field

Create a new custom field definition. Supported types are text, number, date, boolean, and select.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CustomFieldsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CustomFieldsApi apiInstance = new CustomFieldsApi(defaultClient);
        CreateCustomFieldRequest createCustomFieldRequest = new CreateCustomFieldRequest(); // CreateCustomFieldRequest | 
        try {
            ApiResponse<CreateCustomField200Response> response = apiInstance.createCustomFieldWithHttpInfo(createCustomFieldRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling CustomFieldsApi#createCustomField");
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
| **createCustomFieldRequest** | [**CreateCustomFieldRequest**](CreateCustomFieldRequest.md)|  | |

### Return type

ApiResponse<[**CreateCustomField200Response**](CreateCustomField200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Custom field created |  -  |
| **401** | Unauthorized |  -  |
| **409** | Duplicate slug |  -  |


## deleteCustomField

> void deleteCustomField(fieldId)

Delete custom field

Delete a custom field definition and remove its values from all contacts.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CustomFieldsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CustomFieldsApi apiInstance = new CustomFieldsApi(defaultClient);
        String fieldId = "fieldId_example"; // String | 
        try {
            apiInstance.deleteCustomField(fieldId);
        } catch (ApiException e) {
            System.err.println("Exception when calling CustomFieldsApi#deleteCustomField");
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
| **fieldId** | **String**|  | |

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
| **200** | Custom field deleted |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## deleteCustomFieldWithHttpInfo

> ApiResponse<Void> deleteCustomField deleteCustomFieldWithHttpInfo(fieldId)

Delete custom field

Delete a custom field definition and remove its values from all contacts.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CustomFieldsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CustomFieldsApi apiInstance = new CustomFieldsApi(defaultClient);
        String fieldId = "fieldId_example"; // String | 
        try {
            ApiResponse<Void> response = apiInstance.deleteCustomFieldWithHttpInfo(fieldId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling CustomFieldsApi#deleteCustomField");
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
| **fieldId** | **String**|  | |

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
| **200** | Custom field deleted |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## listCustomFields

> ListCustomFields200Response listCustomFields(profileId)

List custom field definitions

Returns all custom field definitions. Optionally filter by profile.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CustomFieldsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CustomFieldsApi apiInstance = new CustomFieldsApi(defaultClient);
        String profileId = "profileId_example"; // String | Filter by profile. Omit to list across all profiles
        try {
            ListCustomFields200Response result = apiInstance.listCustomFields(profileId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling CustomFieldsApi#listCustomFields");
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

### Return type

[**ListCustomFields200Response**](ListCustomFields200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of custom field definitions |  -  |
| **401** | Unauthorized |  -  |

## listCustomFieldsWithHttpInfo

> ApiResponse<ListCustomFields200Response> listCustomFields listCustomFieldsWithHttpInfo(profileId)

List custom field definitions

Returns all custom field definitions. Optionally filter by profile.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CustomFieldsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CustomFieldsApi apiInstance = new CustomFieldsApi(defaultClient);
        String profileId = "profileId_example"; // String | Filter by profile. Omit to list across all profiles
        try {
            ApiResponse<ListCustomFields200Response> response = apiInstance.listCustomFieldsWithHttpInfo(profileId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling CustomFieldsApi#listCustomFields");
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

### Return type

ApiResponse<[**ListCustomFields200Response**](ListCustomFields200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of custom field definitions |  -  |
| **401** | Unauthorized |  -  |


## setContactFieldValue

> void setContactFieldValue(contactId, slug, setContactFieldValueRequest)

Set custom field value

Set or overwrite a custom field value on a contact. The value type must match the field definition.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CustomFieldsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CustomFieldsApi apiInstance = new CustomFieldsApi(defaultClient);
        String contactId = "contactId_example"; // String | 
        String slug = "slug_example"; // String | 
        SetContactFieldValueRequest setContactFieldValueRequest = new SetContactFieldValueRequest(); // SetContactFieldValueRequest | 
        try {
            apiInstance.setContactFieldValue(contactId, slug, setContactFieldValueRequest);
        } catch (ApiException e) {
            System.err.println("Exception when calling CustomFieldsApi#setContactFieldValue");
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
| **slug** | **String**|  | |
| **setContactFieldValueRequest** | [**SetContactFieldValueRequest**](SetContactFieldValueRequest.md)|  | |

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
| **200** | Field value set |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## setContactFieldValueWithHttpInfo

> ApiResponse<Void> setContactFieldValue setContactFieldValueWithHttpInfo(contactId, slug, setContactFieldValueRequest)

Set custom field value

Set or overwrite a custom field value on a contact. The value type must match the field definition.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CustomFieldsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CustomFieldsApi apiInstance = new CustomFieldsApi(defaultClient);
        String contactId = "contactId_example"; // String | 
        String slug = "slug_example"; // String | 
        SetContactFieldValueRequest setContactFieldValueRequest = new SetContactFieldValueRequest(); // SetContactFieldValueRequest | 
        try {
            ApiResponse<Void> response = apiInstance.setContactFieldValueWithHttpInfo(contactId, slug, setContactFieldValueRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling CustomFieldsApi#setContactFieldValue");
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
| **slug** | **String**|  | |
| **setContactFieldValueRequest** | [**SetContactFieldValueRequest**](SetContactFieldValueRequest.md)|  | |

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
| **200** | Field value set |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## updateCustomField

> UpdateCustomField200Response updateCustomField(fieldId, updateCustomFieldRequest)

Update custom field

Update a custom field definition. The field type cannot be changed after creation.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CustomFieldsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CustomFieldsApi apiInstance = new CustomFieldsApi(defaultClient);
        String fieldId = "fieldId_example"; // String | 
        UpdateCustomFieldRequest updateCustomFieldRequest = new UpdateCustomFieldRequest(); // UpdateCustomFieldRequest | 
        try {
            UpdateCustomField200Response result = apiInstance.updateCustomField(fieldId, updateCustomFieldRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling CustomFieldsApi#updateCustomField");
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
| **fieldId** | **String**|  | |
| **updateCustomFieldRequest** | [**UpdateCustomFieldRequest**](UpdateCustomFieldRequest.md)|  | [optional] |

### Return type

[**UpdateCustomField200Response**](UpdateCustomField200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Custom field updated |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## updateCustomFieldWithHttpInfo

> ApiResponse<UpdateCustomField200Response> updateCustomField updateCustomFieldWithHttpInfo(fieldId, updateCustomFieldRequest)

Update custom field

Update a custom field definition. The field type cannot be changed after creation.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.CustomFieldsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CustomFieldsApi apiInstance = new CustomFieldsApi(defaultClient);
        String fieldId = "fieldId_example"; // String | 
        UpdateCustomFieldRequest updateCustomFieldRequest = new UpdateCustomFieldRequest(); // UpdateCustomFieldRequest | 
        try {
            ApiResponse<UpdateCustomField200Response> response = apiInstance.updateCustomFieldWithHttpInfo(fieldId, updateCustomFieldRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling CustomFieldsApi#updateCustomField");
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
| **fieldId** | **String**|  | |
| **updateCustomFieldRequest** | [**UpdateCustomFieldRequest**](UpdateCustomFieldRequest.md)|  | [optional] |

### Return type

ApiResponse<[**UpdateCustomField200Response**](UpdateCustomField200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Custom field updated |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

