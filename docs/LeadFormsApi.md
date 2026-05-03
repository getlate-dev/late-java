# LeadFormsApi

All URIs are relative to *https://zernio.com/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createLeadForm**](LeadFormsApi.md#createLeadForm) | **POST** /v1/ads/lead-forms | Create a Meta Lead Gen Form |
| [**createLeadFormWithHttpInfo**](LeadFormsApi.md#createLeadFormWithHttpInfo) | **POST** /v1/ads/lead-forms | Create a Meta Lead Gen Form |
| [**createLeadFormTestLead**](LeadFormsApi.md#createLeadFormTestLead) | **POST** /v1/ads/lead-forms/{formId}/test-leads | Create a synthetic test lead |
| [**createLeadFormTestLeadWithHttpInfo**](LeadFormsApi.md#createLeadFormTestLeadWithHttpInfo) | **POST** /v1/ads/lead-forms/{formId}/test-leads | Create a synthetic test lead |
| [**deleteLeadForm**](LeadFormsApi.md#deleteLeadForm) | **DELETE** /v1/ads/lead-forms/{formId} | Delete a Lead Gen Form |
| [**deleteLeadFormWithHttpInfo**](LeadFormsApi.md#deleteLeadFormWithHttpInfo) | **DELETE** /v1/ads/lead-forms/{formId} | Delete a Lead Gen Form |
| [**deleteLeadFormTestLead**](LeadFormsApi.md#deleteLeadFormTestLead) | **DELETE** /v1/ads/lead-forms/{formId}/test-leads/{leadId} | Delete a (test) lead |
| [**deleteLeadFormTestLeadWithHttpInfo**](LeadFormsApi.md#deleteLeadFormTestLeadWithHttpInfo) | **DELETE** /v1/ads/lead-forms/{formId}/test-leads/{leadId} | Delete a (test) lead |
| [**getLeadForm**](LeadFormsApi.md#getLeadForm) | **GET** /v1/ads/lead-forms/{formId} | Get a Lead Gen Form |
| [**getLeadFormWithHttpInfo**](LeadFormsApi.md#getLeadFormWithHttpInfo) | **GET** /v1/ads/lead-forms/{formId} | Get a Lead Gen Form |
| [**listLeadFormLeads**](LeadFormsApi.md#listLeadFormLeads) | **GET** /v1/ads/lead-forms/{formId}/leads | List submitted leads for a form |
| [**listLeadFormLeadsWithHttpInfo**](LeadFormsApi.md#listLeadFormLeadsWithHttpInfo) | **GET** /v1/ads/lead-forms/{formId}/leads | List submitted leads for a form |
| [**listLeadForms**](LeadFormsApi.md#listLeadForms) | **GET** /v1/ads/lead-forms | List Meta Lead Gen Forms |
| [**listLeadFormsWithHttpInfo**](LeadFormsApi.md#listLeadFormsWithHttpInfo) | **GET** /v1/ads/lead-forms | List Meta Lead Gen Forms |
| [**updateLeadForm**](LeadFormsApi.md#updateLeadForm) | **PATCH** /v1/ads/lead-forms/{formId} | Update a Lead Gen Form (status only) |
| [**updateLeadFormWithHttpInfo**](LeadFormsApi.md#updateLeadFormWithHttpInfo) | **PATCH** /v1/ads/lead-forms/{formId} | Update a Lead Gen Form (status only) |



## createLeadForm

> CreateLeadForm201Response createLeadForm(createLeadFormBody)

Create a Meta Lead Gen Form

Creates a new Instant Form on the Facebook Page tied to the given social account. The form is created in &#x60;ACTIVE&#x60; status and is immediately attachable to ads (see &#x60;leadGenFormId&#x60; on POST /v1/ads/create).  Once a form has received any leads, its questions / privacy policy / thank-you page become immutable on Meta&#39;s side; only &#x60;status&#x60; may be changed via PATCH. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LeadFormsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LeadFormsApi apiInstance = new LeadFormsApi(defaultClient);
        CreateLeadFormBody createLeadFormBody = new CreateLeadFormBody(); // CreateLeadFormBody | 
        try {
            CreateLeadForm201Response result = apiInstance.createLeadForm(createLeadFormBody);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling LeadFormsApi#createLeadForm");
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
| **createLeadFormBody** | [**CreateLeadFormBody**](CreateLeadFormBody.md)|  | |

### Return type

[**CreateLeadForm201Response**](CreateLeadForm201Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Form created |  -  |
| **400** | Validation failure |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Social account not found |  -  |

## createLeadFormWithHttpInfo

> ApiResponse<CreateLeadForm201Response> createLeadForm createLeadFormWithHttpInfo(createLeadFormBody)

Create a Meta Lead Gen Form

Creates a new Instant Form on the Facebook Page tied to the given social account. The form is created in &#x60;ACTIVE&#x60; status and is immediately attachable to ads (see &#x60;leadGenFormId&#x60; on POST /v1/ads/create).  Once a form has received any leads, its questions / privacy policy / thank-you page become immutable on Meta&#39;s side; only &#x60;status&#x60; may be changed via PATCH. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LeadFormsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LeadFormsApi apiInstance = new LeadFormsApi(defaultClient);
        CreateLeadFormBody createLeadFormBody = new CreateLeadFormBody(); // CreateLeadFormBody | 
        try {
            ApiResponse<CreateLeadForm201Response> response = apiInstance.createLeadFormWithHttpInfo(createLeadFormBody);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling LeadFormsApi#createLeadForm");
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
| **createLeadFormBody** | [**CreateLeadFormBody**](CreateLeadFormBody.md)|  | |

### Return type

ApiResponse<[**CreateLeadForm201Response**](CreateLeadForm201Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Form created |  -  |
| **400** | Validation failure |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Social account not found |  -  |


## createLeadFormTestLead

> CreateLeadFormTestLead200Response createLeadFormTestLead(formId, createLeadFormTestLeadRequest)

Create a synthetic test lead

Submits a fake lead against a form. Useful for QA, App Review demos, and exercising webhook subscribers without waiting for real ad impressions. Meta caps a form to one outstanding test lead — call DELETE on the returned id before re-submitting. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LeadFormsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LeadFormsApi apiInstance = new LeadFormsApi(defaultClient);
        String formId = "formId_example"; // String | 
        CreateLeadFormTestLeadRequest createLeadFormTestLeadRequest = new CreateLeadFormTestLeadRequest(); // CreateLeadFormTestLeadRequest | 
        try {
            CreateLeadFormTestLead200Response result = apiInstance.createLeadFormTestLead(formId, createLeadFormTestLeadRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling LeadFormsApi#createLeadFormTestLead");
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
| **formId** | **String**|  | |
| **createLeadFormTestLeadRequest** | [**CreateLeadFormTestLeadRequest**](CreateLeadFormTestLeadRequest.md)|  | |

### Return type

[**CreateLeadFormTestLead200Response**](CreateLeadFormTestLead200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Test lead created |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Form or account not found |  -  |

## createLeadFormTestLeadWithHttpInfo

> ApiResponse<CreateLeadFormTestLead200Response> createLeadFormTestLead createLeadFormTestLeadWithHttpInfo(formId, createLeadFormTestLeadRequest)

Create a synthetic test lead

Submits a fake lead against a form. Useful for QA, App Review demos, and exercising webhook subscribers without waiting for real ad impressions. Meta caps a form to one outstanding test lead — call DELETE on the returned id before re-submitting. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LeadFormsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LeadFormsApi apiInstance = new LeadFormsApi(defaultClient);
        String formId = "formId_example"; // String | 
        CreateLeadFormTestLeadRequest createLeadFormTestLeadRequest = new CreateLeadFormTestLeadRequest(); // CreateLeadFormTestLeadRequest | 
        try {
            ApiResponse<CreateLeadFormTestLead200Response> response = apiInstance.createLeadFormTestLeadWithHttpInfo(formId, createLeadFormTestLeadRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling LeadFormsApi#createLeadFormTestLead");
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
| **formId** | **String**|  | |
| **createLeadFormTestLeadRequest** | [**CreateLeadFormTestLeadRequest**](CreateLeadFormTestLeadRequest.md)|  | |

### Return type

ApiResponse<[**CreateLeadFormTestLead200Response**](CreateLeadFormTestLead200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Test lead created |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Form or account not found |  -  |


## deleteLeadForm

> DeleteLeadForm200Response deleteLeadForm(formId, accountId)

Delete a Lead Gen Form

Deletes the form from Meta. If the form has already received leads, Meta archives it instead of hard-deleting; the response is the same either way. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LeadFormsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LeadFormsApi apiInstance = new LeadFormsApi(defaultClient);
        String formId = "formId_example"; // String | 
        String accountId = "accountId_example"; // String | 
        try {
            DeleteLeadForm200Response result = apiInstance.deleteLeadForm(formId, accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling LeadFormsApi#deleteLeadForm");
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
| **formId** | **String**|  | |
| **accountId** | **String**|  | |

### Return type

[**DeleteLeadForm200Response**](DeleteLeadForm200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Form deleted (or archived) |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Form not found |  -  |

## deleteLeadFormWithHttpInfo

> ApiResponse<DeleteLeadForm200Response> deleteLeadForm deleteLeadFormWithHttpInfo(formId, accountId)

Delete a Lead Gen Form

Deletes the form from Meta. If the form has already received leads, Meta archives it instead of hard-deleting; the response is the same either way. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LeadFormsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LeadFormsApi apiInstance = new LeadFormsApi(defaultClient);
        String formId = "formId_example"; // String | 
        String accountId = "accountId_example"; // String | 
        try {
            ApiResponse<DeleteLeadForm200Response> response = apiInstance.deleteLeadFormWithHttpInfo(formId, accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling LeadFormsApi#deleteLeadForm");
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
| **formId** | **String**|  | |
| **accountId** | **String**|  | |

### Return type

ApiResponse<[**DeleteLeadForm200Response**](DeleteLeadForm200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Form deleted (or archived) |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Form not found |  -  |


## deleteLeadFormTestLead

> DeleteLeadForm200Response deleteLeadFormTestLead(formId, leadId, accountId)

Delete a (test) lead

Deletes a single lead by ID. Primarily used to clear the outstanding test lead so you can submit a new one. The same Graph API call works on real leads too; for production lead deletion (GDPR/CCPA) prefer a dedicated flow. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LeadFormsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LeadFormsApi apiInstance = new LeadFormsApi(defaultClient);
        String formId = "formId_example"; // String | 
        String leadId = "leadId_example"; // String | 
        String accountId = "accountId_example"; // String | 
        try {
            DeleteLeadForm200Response result = apiInstance.deleteLeadFormTestLead(formId, leadId, accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling LeadFormsApi#deleteLeadFormTestLead");
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
| **formId** | **String**|  | |
| **leadId** | **String**|  | |
| **accountId** | **String**|  | |

### Return type

[**DeleteLeadForm200Response**](DeleteLeadForm200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Lead deleted |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Lead not found |  -  |

## deleteLeadFormTestLeadWithHttpInfo

> ApiResponse<DeleteLeadForm200Response> deleteLeadFormTestLead deleteLeadFormTestLeadWithHttpInfo(formId, leadId, accountId)

Delete a (test) lead

Deletes a single lead by ID. Primarily used to clear the outstanding test lead so you can submit a new one. The same Graph API call works on real leads too; for production lead deletion (GDPR/CCPA) prefer a dedicated flow. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LeadFormsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LeadFormsApi apiInstance = new LeadFormsApi(defaultClient);
        String formId = "formId_example"; // String | 
        String leadId = "leadId_example"; // String | 
        String accountId = "accountId_example"; // String | 
        try {
            ApiResponse<DeleteLeadForm200Response> response = apiInstance.deleteLeadFormTestLeadWithHttpInfo(formId, leadId, accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling LeadFormsApi#deleteLeadFormTestLead");
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
| **formId** | **String**|  | |
| **leadId** | **String**|  | |
| **accountId** | **String**|  | |

### Return type

ApiResponse<[**DeleteLeadForm200Response**](DeleteLeadForm200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Lead deleted |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Lead not found |  -  |


## getLeadForm

> GetLeadForm200Response getLeadForm(formId, accountId)

Get a Lead Gen Form

Returns full details for a single form, including questions, privacy policy, and lead counts.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LeadFormsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LeadFormsApi apiInstance = new LeadFormsApi(defaultClient);
        String formId = "formId_example"; // String | Meta lead form ID (numeric string)
        String accountId = "accountId_example"; // String | 
        try {
            GetLeadForm200Response result = apiInstance.getLeadForm(formId, accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling LeadFormsApi#getLeadForm");
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
| **formId** | **String**| Meta lead form ID (numeric string) | |
| **accountId** | **String**|  | |

### Return type

[**GetLeadForm200Response**](GetLeadForm200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Form details |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Form or account not found |  -  |

## getLeadFormWithHttpInfo

> ApiResponse<GetLeadForm200Response> getLeadForm getLeadFormWithHttpInfo(formId, accountId)

Get a Lead Gen Form

Returns full details for a single form, including questions, privacy policy, and lead counts.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LeadFormsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LeadFormsApi apiInstance = new LeadFormsApi(defaultClient);
        String formId = "formId_example"; // String | Meta lead form ID (numeric string)
        String accountId = "accountId_example"; // String | 
        try {
            ApiResponse<GetLeadForm200Response> response = apiInstance.getLeadFormWithHttpInfo(formId, accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling LeadFormsApi#getLeadForm");
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
| **formId** | **String**| Meta lead form ID (numeric string) | |
| **accountId** | **String**|  | |

### Return type

ApiResponse<[**GetLeadForm200Response**](GetLeadForm200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Form details |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Form or account not found |  -  |


## listLeadFormLeads

> ListLeadFormLeads200Response listLeadFormLeads(formId, accountId, limit, cursor, since)

List submitted leads for a form

Returns leads submitted against a Lead Gen Form. The page access token on the connected account must have the &#x60;leads_retrieval&#x60; permission — if the token was minted before that scope was approved, this endpoint returns &#x60;code: scope_reconnect_required&#x60; (HTTP 422) and the customer must reconnect the Facebook account.  For real-time delivery without polling, subscribe a webhook to the &#x60;lead.received&#x60; event. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LeadFormsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LeadFormsApi apiInstance = new LeadFormsApi(defaultClient);
        String formId = "formId_example"; // String | 
        String accountId = "accountId_example"; // String | 
        Integer limit = 25; // Integer | 
        String cursor = "cursor_example"; // String | 
        Integer since = 56; // Integer | Unix timestamp; only return leads created strictly after this.
        try {
            ListLeadFormLeads200Response result = apiInstance.listLeadFormLeads(formId, accountId, limit, cursor, since);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling LeadFormsApi#listLeadFormLeads");
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
| **formId** | **String**|  | |
| **accountId** | **String**|  | |
| **limit** | **Integer**|  | [optional] [default to 25] |
| **cursor** | **String**|  | [optional] |
| **since** | **Integer**| Unix timestamp; only return leads created strictly after this. | [optional] |

### Return type

[**ListLeadFormLeads200Response**](ListLeadFormLeads200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Leads |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **422** | Connected account is missing the &#x60;leads_retrieval&#x60; scope and must be reconnected. &#x60;code&#x60; is &#x60;scope_reconnect_required&#x60;. |  -  |

## listLeadFormLeadsWithHttpInfo

> ApiResponse<ListLeadFormLeads200Response> listLeadFormLeads listLeadFormLeadsWithHttpInfo(formId, accountId, limit, cursor, since)

List submitted leads for a form

Returns leads submitted against a Lead Gen Form. The page access token on the connected account must have the &#x60;leads_retrieval&#x60; permission — if the token was minted before that scope was approved, this endpoint returns &#x60;code: scope_reconnect_required&#x60; (HTTP 422) and the customer must reconnect the Facebook account.  For real-time delivery without polling, subscribe a webhook to the &#x60;lead.received&#x60; event. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LeadFormsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LeadFormsApi apiInstance = new LeadFormsApi(defaultClient);
        String formId = "formId_example"; // String | 
        String accountId = "accountId_example"; // String | 
        Integer limit = 25; // Integer | 
        String cursor = "cursor_example"; // String | 
        Integer since = 56; // Integer | Unix timestamp; only return leads created strictly after this.
        try {
            ApiResponse<ListLeadFormLeads200Response> response = apiInstance.listLeadFormLeadsWithHttpInfo(formId, accountId, limit, cursor, since);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling LeadFormsApi#listLeadFormLeads");
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
| **formId** | **String**|  | |
| **accountId** | **String**|  | |
| **limit** | **Integer**|  | [optional] [default to 25] |
| **cursor** | **String**|  | [optional] |
| **since** | **Integer**| Unix timestamp; only return leads created strictly after this. | [optional] |

### Return type

ApiResponse<[**ListLeadFormLeads200Response**](ListLeadFormLeads200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Leads |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **422** | Connected account is missing the &#x60;leads_retrieval&#x60; scope and must be reconnected. &#x60;code&#x60; is &#x60;scope_reconnect_required&#x60;. |  -  |


## listLeadForms

> ListLeadForms200Response listLeadForms(accountId, limit, cursor)

List Meta Lead Gen Forms

Returns Meta Instant Forms attached to the Facebook Page connected via the given social account. Forms live on Facebook Pages — Instagram lead ads reuse the linked Page under the hood, so even Instagram-only ad accounts list forms from the linked Facebook Page. Requires the Ads add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LeadFormsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LeadFormsApi apiInstance = new LeadFormsApi(defaultClient);
        String accountId = "accountId_example"; // String | Facebook social account ID (Late SocialAccount _id)
        Integer limit = 25; // Integer | 
        String cursor = "cursor_example"; // String | Meta `paging.cursors.after` from a prior page
        try {
            ListLeadForms200Response result = apiInstance.listLeadForms(accountId, limit, cursor);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling LeadFormsApi#listLeadForms");
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
| **accountId** | **String**| Facebook social account ID (Late SocialAccount _id) | |
| **limit** | **Integer**|  | [optional] [default to 25] |
| **cursor** | **String**| Meta &#x60;paging.cursors.after&#x60; from a prior page | [optional] |

### Return type

[**ListLeadForms200Response**](ListLeadForms200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Forms list |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Social account not found |  -  |

## listLeadFormsWithHttpInfo

> ApiResponse<ListLeadForms200Response> listLeadForms listLeadFormsWithHttpInfo(accountId, limit, cursor)

List Meta Lead Gen Forms

Returns Meta Instant Forms attached to the Facebook Page connected via the given social account. Forms live on Facebook Pages — Instagram lead ads reuse the linked Page under the hood, so even Instagram-only ad accounts list forms from the linked Facebook Page. Requires the Ads add-on. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LeadFormsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LeadFormsApi apiInstance = new LeadFormsApi(defaultClient);
        String accountId = "accountId_example"; // String | Facebook social account ID (Late SocialAccount _id)
        Integer limit = 25; // Integer | 
        String cursor = "cursor_example"; // String | Meta `paging.cursors.after` from a prior page
        try {
            ApiResponse<ListLeadForms200Response> response = apiInstance.listLeadFormsWithHttpInfo(accountId, limit, cursor);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling LeadFormsApi#listLeadForms");
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
| **accountId** | **String**| Facebook social account ID (Late SocialAccount _id) | |
| **limit** | **Integer**|  | [optional] [default to 25] |
| **cursor** | **String**| Meta &#x60;paging.cursors.after&#x60; from a prior page | [optional] |

### Return type

ApiResponse<[**ListLeadForms200Response**](ListLeadForms200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Forms list |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Social account not found |  -  |


## updateLeadForm

> DeleteLeadForm200Response updateLeadForm(formId, updateLeadFormRequest)

Update a Lead Gen Form (status only)

Update mutable fields on an existing form. Today only &#x60;status&#x60; is mutable on Meta&#39;s side — questions / privacy_policy / thank_you_page are immutable once a form has received any leads. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LeadFormsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LeadFormsApi apiInstance = new LeadFormsApi(defaultClient);
        String formId = "formId_example"; // String | 
        UpdateLeadFormRequest updateLeadFormRequest = new UpdateLeadFormRequest(); // UpdateLeadFormRequest | 
        try {
            DeleteLeadForm200Response result = apiInstance.updateLeadForm(formId, updateLeadFormRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling LeadFormsApi#updateLeadForm");
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
| **formId** | **String**|  | |
| **updateLeadFormRequest** | [**UpdateLeadFormRequest**](UpdateLeadFormRequest.md)|  | |

### Return type

[**DeleteLeadForm200Response**](DeleteLeadForm200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Form updated |  -  |
| **400** | Validation failure |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Form not found |  -  |

## updateLeadFormWithHttpInfo

> ApiResponse<DeleteLeadForm200Response> updateLeadForm updateLeadFormWithHttpInfo(formId, updateLeadFormRequest)

Update a Lead Gen Form (status only)

Update mutable fields on an existing form. Today only &#x60;status&#x60; is mutable on Meta&#39;s side — questions / privacy_policy / thank_you_page are immutable once a form has received any leads. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LeadFormsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LeadFormsApi apiInstance = new LeadFormsApi(defaultClient);
        String formId = "formId_example"; // String | 
        UpdateLeadFormRequest updateLeadFormRequest = new UpdateLeadFormRequest(); // UpdateLeadFormRequest | 
        try {
            ApiResponse<DeleteLeadForm200Response> response = apiInstance.updateLeadFormWithHttpInfo(formId, updateLeadFormRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling LeadFormsApi#updateLeadForm");
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
| **formId** | **String**|  | |
| **updateLeadFormRequest** | [**UpdateLeadFormRequest**](UpdateLeadFormRequest.md)|  | |

### Return type

ApiResponse<[**DeleteLeadForm200Response**](DeleteLeadForm200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Form updated |  -  |
| **400** | Validation failure |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required |  -  |
| **404** | Form not found |  -  |

