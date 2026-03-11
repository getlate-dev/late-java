# WhatsAppPhoneNumbersApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getPreverifiedWhatsAppNumbers**](WhatsAppPhoneNumbersApi.md#getPreverifiedWhatsAppNumbers) | **GET** /v1/whatsapp/phone-numbers/preverified | Get pre-verified numbers |
| [**getPreverifiedWhatsAppNumbersWithHttpInfo**](WhatsAppPhoneNumbersApi.md#getPreverifiedWhatsAppNumbersWithHttpInfo) | **GET** /v1/whatsapp/phone-numbers/preverified | Get pre-verified numbers |
| [**getWhatsAppPhoneNumber**](WhatsAppPhoneNumbersApi.md#getWhatsAppPhoneNumber) | **GET** /v1/whatsapp/phone-numbers/{phoneNumberId} | Get phone number |
| [**getWhatsAppPhoneNumberWithHttpInfo**](WhatsAppPhoneNumbersApi.md#getWhatsAppPhoneNumberWithHttpInfo) | **GET** /v1/whatsapp/phone-numbers/{phoneNumberId} | Get phone number |
| [**getWhatsAppPhoneNumbers**](WhatsAppPhoneNumbersApi.md#getWhatsAppPhoneNumbers) | **GET** /v1/whatsapp/phone-numbers | List phone numbers |
| [**getWhatsAppPhoneNumbersWithHttpInfo**](WhatsAppPhoneNumbersApi.md#getWhatsAppPhoneNumbersWithHttpInfo) | **GET** /v1/whatsapp/phone-numbers | List phone numbers |
| [**purchaseWhatsAppPhoneNumber**](WhatsAppPhoneNumbersApi.md#purchaseWhatsAppPhoneNumber) | **POST** /v1/whatsapp/phone-numbers/purchase | Purchase phone number |
| [**purchaseWhatsAppPhoneNumberWithHttpInfo**](WhatsAppPhoneNumbersApi.md#purchaseWhatsAppPhoneNumberWithHttpInfo) | **POST** /v1/whatsapp/phone-numbers/purchase | Purchase phone number |
| [**releaseWhatsAppPhoneNumber**](WhatsAppPhoneNumbersApi.md#releaseWhatsAppPhoneNumber) | **DELETE** /v1/whatsapp/phone-numbers/{phoneNumberId} | Release phone number |
| [**releaseWhatsAppPhoneNumberWithHttpInfo**](WhatsAppPhoneNumbersApi.md#releaseWhatsAppPhoneNumberWithHttpInfo) | **DELETE** /v1/whatsapp/phone-numbers/{phoneNumberId} | Release phone number |
| [**requestWhatsAppVerificationCode**](WhatsAppPhoneNumbersApi.md#requestWhatsAppVerificationCode) | **POST** /v1/whatsapp/phone-numbers/{phoneNumberId}/request-code | Request OTP |
| [**requestWhatsAppVerificationCodeWithHttpInfo**](WhatsAppPhoneNumbersApi.md#requestWhatsAppVerificationCodeWithHttpInfo) | **POST** /v1/whatsapp/phone-numbers/{phoneNumberId}/request-code | Request OTP |
| [**searchAvailableWhatsAppNumbers**](WhatsAppPhoneNumbersApi.md#searchAvailableWhatsAppNumbers) | **GET** /v1/whatsapp/phone-numbers/available | Search available numbers |
| [**searchAvailableWhatsAppNumbersWithHttpInfo**](WhatsAppPhoneNumbersApi.md#searchAvailableWhatsAppNumbersWithHttpInfo) | **GET** /v1/whatsapp/phone-numbers/available | Search available numbers |
| [**verifyWhatsAppPhoneNumber**](WhatsAppPhoneNumbersApi.md#verifyWhatsAppPhoneNumber) | **POST** /v1/whatsapp/phone-numbers/{phoneNumberId}/verify | Verify OTP |
| [**verifyWhatsAppPhoneNumberWithHttpInfo**](WhatsAppPhoneNumbersApi.md#verifyWhatsAppPhoneNumberWithHttpInfo) | **POST** /v1/whatsapp/phone-numbers/{phoneNumberId}/verify | Verify OTP |



## getPreverifiedWhatsAppNumbers

> GetPreverifiedWhatsAppNumbers200Response getPreverifiedWhatsAppNumbers(profileId)

Get pre-verified numbers

Returns the user&#39;s pre-verified phone number IDs that are ready for OTP-free Embedded Signup. Only returns numbers with verified Meta status and non-expired verification. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.WhatsAppPhoneNumbersApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppPhoneNumbersApi apiInstance = new WhatsAppPhoneNumbersApi(defaultClient);
        String profileId = "profileId_example"; // String | Profile ID to filter by
        try {
            GetPreverifiedWhatsAppNumbers200Response result = apiInstance.getPreverifiedWhatsAppNumbers(profileId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppPhoneNumbersApi#getPreverifiedWhatsAppNumbers");
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
| **profileId** | **String**| Profile ID to filter by | |

### Return type

[**GetPreverifiedWhatsAppNumbers200Response**](GetPreverifiedWhatsAppNumbers200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Pre-verified numbers retrieved |  -  |
| **400** | profileId is required |  -  |
| **401** | Unauthorized |  -  |

## getPreverifiedWhatsAppNumbersWithHttpInfo

> ApiResponse<GetPreverifiedWhatsAppNumbers200Response> getPreverifiedWhatsAppNumbers getPreverifiedWhatsAppNumbersWithHttpInfo(profileId)

Get pre-verified numbers

Returns the user&#39;s pre-verified phone number IDs that are ready for OTP-free Embedded Signup. Only returns numbers with verified Meta status and non-expired verification. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.WhatsAppPhoneNumbersApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppPhoneNumbersApi apiInstance = new WhatsAppPhoneNumbersApi(defaultClient);
        String profileId = "profileId_example"; // String | Profile ID to filter by
        try {
            ApiResponse<GetPreverifiedWhatsAppNumbers200Response> response = apiInstance.getPreverifiedWhatsAppNumbersWithHttpInfo(profileId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppPhoneNumbersApi#getPreverifiedWhatsAppNumbers");
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
| **profileId** | **String**| Profile ID to filter by | |

### Return type

ApiResponse<[**GetPreverifiedWhatsAppNumbers200Response**](GetPreverifiedWhatsAppNumbers200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Pre-verified numbers retrieved |  -  |
| **400** | profileId is required |  -  |
| **401** | Unauthorized |  -  |


## getWhatsAppPhoneNumber

> GetWhatsAppPhoneNumber200Response getWhatsAppPhoneNumber(phoneNumberId)

Get phone number

Retrieve the current status of a purchased phone number. Used to poll for Meta pre-verification completion after purchase. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.WhatsAppPhoneNumbersApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppPhoneNumbersApi apiInstance = new WhatsAppPhoneNumbersApi(defaultClient);
        String phoneNumberId = "phoneNumberId_example"; // String | Phone number record ID
        try {
            GetWhatsAppPhoneNumber200Response result = apiInstance.getWhatsAppPhoneNumber(phoneNumberId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppPhoneNumbersApi#getWhatsAppPhoneNumber");
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
| **phoneNumberId** | **String**| Phone number record ID | |

### Return type

[**GetWhatsAppPhoneNumber200Response**](GetWhatsAppPhoneNumber200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Phone number retrieved successfully |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## getWhatsAppPhoneNumberWithHttpInfo

> ApiResponse<GetWhatsAppPhoneNumber200Response> getWhatsAppPhoneNumber getWhatsAppPhoneNumberWithHttpInfo(phoneNumberId)

Get phone number

Retrieve the current status of a purchased phone number. Used to poll for Meta pre-verification completion after purchase. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.WhatsAppPhoneNumbersApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppPhoneNumbersApi apiInstance = new WhatsAppPhoneNumbersApi(defaultClient);
        String phoneNumberId = "phoneNumberId_example"; // String | Phone number record ID
        try {
            ApiResponse<GetWhatsAppPhoneNumber200Response> response = apiInstance.getWhatsAppPhoneNumberWithHttpInfo(phoneNumberId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppPhoneNumbersApi#getWhatsAppPhoneNumber");
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
| **phoneNumberId** | **String**| Phone number record ID | |

### Return type

ApiResponse<[**GetWhatsAppPhoneNumber200Response**](GetWhatsAppPhoneNumber200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Phone number retrieved successfully |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## getWhatsAppPhoneNumbers

> GetWhatsAppPhoneNumbers200Response getWhatsAppPhoneNumbers(status, profileId)

List phone numbers

List all WhatsApp phone numbers purchased by the authenticated user. By default, released numbers are excluded. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.WhatsAppPhoneNumbersApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppPhoneNumbersApi apiInstance = new WhatsAppPhoneNumbersApi(defaultClient);
        String status = "provisioning"; // String | Filter by status (by default excludes released numbers)
        String profileId = "profileId_example"; // String | Filter by profile
        try {
            GetWhatsAppPhoneNumbers200Response result = apiInstance.getWhatsAppPhoneNumbers(status, profileId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppPhoneNumbersApi#getWhatsAppPhoneNumbers");
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
| **status** | **String**| Filter by status (by default excludes released numbers) | [optional] [enum: provisioning, active, suspended, releasing, released] |
| **profileId** | **String**| Filter by profile | [optional] |

### Return type

[**GetWhatsAppPhoneNumbers200Response**](GetWhatsAppPhoneNumbers200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Phone numbers retrieved successfully |  -  |
| **401** | Unauthorized |  -  |

## getWhatsAppPhoneNumbersWithHttpInfo

> ApiResponse<GetWhatsAppPhoneNumbers200Response> getWhatsAppPhoneNumbers getWhatsAppPhoneNumbersWithHttpInfo(status, profileId)

List phone numbers

List all WhatsApp phone numbers purchased by the authenticated user. By default, released numbers are excluded. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.WhatsAppPhoneNumbersApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppPhoneNumbersApi apiInstance = new WhatsAppPhoneNumbersApi(defaultClient);
        String status = "provisioning"; // String | Filter by status (by default excludes released numbers)
        String profileId = "profileId_example"; // String | Filter by profile
        try {
            ApiResponse<GetWhatsAppPhoneNumbers200Response> response = apiInstance.getWhatsAppPhoneNumbersWithHttpInfo(status, profileId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppPhoneNumbersApi#getWhatsAppPhoneNumbers");
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
| **status** | **String**| Filter by status (by default excludes released numbers) | [optional] [enum: provisioning, active, suspended, releasing, released] |
| **profileId** | **String**| Filter by profile | [optional] |

### Return type

ApiResponse<[**GetWhatsAppPhoneNumbers200Response**](GetWhatsAppPhoneNumbers200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Phone numbers retrieved successfully |  -  |
| **401** | Unauthorized |  -  |


## purchaseWhatsAppPhoneNumber

> PurchaseWhatsAppPhoneNumber200Response purchaseWhatsAppPhoneNumber(purchaseWhatsAppPhoneNumberRequest)

Purchase phone number

Initiate purchasing a WhatsApp phone number. Payment-first flow: the user does not pick a specific number. The system either creates a Stripe Checkout Session (first number) or increments the existing subscription quantity and provisions inline (subsequent numbers).  Requires a paid plan. The maximum number of phone numbers is determined by the user&#39;s plan. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.WhatsAppPhoneNumbersApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppPhoneNumbersApi apiInstance = new WhatsAppPhoneNumbersApi(defaultClient);
        PurchaseWhatsAppPhoneNumberRequest purchaseWhatsAppPhoneNumberRequest = new PurchaseWhatsAppPhoneNumberRequest(); // PurchaseWhatsAppPhoneNumberRequest | 
        try {
            PurchaseWhatsAppPhoneNumber200Response result = apiInstance.purchaseWhatsAppPhoneNumber(purchaseWhatsAppPhoneNumberRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppPhoneNumbersApi#purchaseWhatsAppPhoneNumber");
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
| **purchaseWhatsAppPhoneNumberRequest** | [**PurchaseWhatsAppPhoneNumberRequest**](PurchaseWhatsAppPhoneNumberRequest.md)|  | |

### Return type

[**PurchaseWhatsAppPhoneNumber200Response**](PurchaseWhatsAppPhoneNumber200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Either a checkout URL (first number) or the provisioned phone number (subsequent numbers).  |  -  |
| **400** | Plan limit reached or profileId required |  -  |
| **401** | Unauthorized |  -  |
| **403** | A paid plan is required |  -  |

## purchaseWhatsAppPhoneNumberWithHttpInfo

> ApiResponse<PurchaseWhatsAppPhoneNumber200Response> purchaseWhatsAppPhoneNumber purchaseWhatsAppPhoneNumberWithHttpInfo(purchaseWhatsAppPhoneNumberRequest)

Purchase phone number

Initiate purchasing a WhatsApp phone number. Payment-first flow: the user does not pick a specific number. The system either creates a Stripe Checkout Session (first number) or increments the existing subscription quantity and provisions inline (subsequent numbers).  Requires a paid plan. The maximum number of phone numbers is determined by the user&#39;s plan. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.WhatsAppPhoneNumbersApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppPhoneNumbersApi apiInstance = new WhatsAppPhoneNumbersApi(defaultClient);
        PurchaseWhatsAppPhoneNumberRequest purchaseWhatsAppPhoneNumberRequest = new PurchaseWhatsAppPhoneNumberRequest(); // PurchaseWhatsAppPhoneNumberRequest | 
        try {
            ApiResponse<PurchaseWhatsAppPhoneNumber200Response> response = apiInstance.purchaseWhatsAppPhoneNumberWithHttpInfo(purchaseWhatsAppPhoneNumberRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppPhoneNumbersApi#purchaseWhatsAppPhoneNumber");
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
| **purchaseWhatsAppPhoneNumberRequest** | [**PurchaseWhatsAppPhoneNumberRequest**](PurchaseWhatsAppPhoneNumberRequest.md)|  | |

### Return type

ApiResponse<[**PurchaseWhatsAppPhoneNumber200Response**](PurchaseWhatsAppPhoneNumber200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Either a checkout URL (first number) or the provisioned phone number (subsequent numbers).  |  -  |
| **400** | Plan limit reached or profileId required |  -  |
| **401** | Unauthorized |  -  |
| **403** | A paid plan is required |  -  |


## releaseWhatsAppPhoneNumber

> ReleaseWhatsAppPhoneNumber200Response releaseWhatsAppPhoneNumber(phoneNumberId)

Release phone number

Release a purchased phone number. This will: 1. Disconnect any linked WhatsApp social account 2. Decrement the Stripe subscription quantity (or cancel if last number) 3. Release the number from Telnyx 4. Mark the number as released 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.WhatsAppPhoneNumbersApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppPhoneNumbersApi apiInstance = new WhatsAppPhoneNumbersApi(defaultClient);
        String phoneNumberId = "phoneNumberId_example"; // String | Phone number record ID
        try {
            ReleaseWhatsAppPhoneNumber200Response result = apiInstance.releaseWhatsAppPhoneNumber(phoneNumberId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppPhoneNumbersApi#releaseWhatsAppPhoneNumber");
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
| **phoneNumberId** | **String**| Phone number record ID | |

### Return type

[**ReleaseWhatsAppPhoneNumber200Response**](ReleaseWhatsAppPhoneNumber200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Phone number released successfully |  -  |
| **400** | Phone number is already released or being released |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## releaseWhatsAppPhoneNumberWithHttpInfo

> ApiResponse<ReleaseWhatsAppPhoneNumber200Response> releaseWhatsAppPhoneNumber releaseWhatsAppPhoneNumberWithHttpInfo(phoneNumberId)

Release phone number

Release a purchased phone number. This will: 1. Disconnect any linked WhatsApp social account 2. Decrement the Stripe subscription quantity (or cancel if last number) 3. Release the number from Telnyx 4. Mark the number as released 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.WhatsAppPhoneNumbersApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppPhoneNumbersApi apiInstance = new WhatsAppPhoneNumbersApi(defaultClient);
        String phoneNumberId = "phoneNumberId_example"; // String | Phone number record ID
        try {
            ApiResponse<ReleaseWhatsAppPhoneNumber200Response> response = apiInstance.releaseWhatsAppPhoneNumberWithHttpInfo(phoneNumberId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppPhoneNumbersApi#releaseWhatsAppPhoneNumber");
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
| **phoneNumberId** | **String**| Phone number record ID | |

### Return type

ApiResponse<[**ReleaseWhatsAppPhoneNumber200Response**](ReleaseWhatsAppPhoneNumber200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Phone number released successfully |  -  |
| **400** | Phone number is already released or being released |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## requestWhatsAppVerificationCode

> RequestWhatsAppVerificationCode200Response requestWhatsAppVerificationCode(phoneNumberId, requestWhatsAppVerificationCodeRequest)

Request OTP

Request a new OTP verification code from Meta for a pre-verified phone number. Useful when the initial SMS did not arrive or when re-verifying before the 90-day expiry. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.WhatsAppPhoneNumbersApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppPhoneNumbersApi apiInstance = new WhatsAppPhoneNumbersApi(defaultClient);
        String phoneNumberId = "phoneNumberId_example"; // String | Phone number record ID
        RequestWhatsAppVerificationCodeRequest requestWhatsAppVerificationCodeRequest = new RequestWhatsAppVerificationCodeRequest(); // RequestWhatsAppVerificationCodeRequest | 
        try {
            RequestWhatsAppVerificationCode200Response result = apiInstance.requestWhatsAppVerificationCode(phoneNumberId, requestWhatsAppVerificationCodeRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppPhoneNumbersApi#requestWhatsAppVerificationCode");
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
| **phoneNumberId** | **String**| Phone number record ID | |
| **requestWhatsAppVerificationCodeRequest** | [**RequestWhatsAppVerificationCodeRequest**](RequestWhatsAppVerificationCodeRequest.md)|  | [optional] |

### Return type

[**RequestWhatsAppVerificationCode200Response**](RequestWhatsAppVerificationCode200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Verification code requested successfully |  -  |
| **400** | Number has not been added to Meta pre-verified pool |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## requestWhatsAppVerificationCodeWithHttpInfo

> ApiResponse<RequestWhatsAppVerificationCode200Response> requestWhatsAppVerificationCode requestWhatsAppVerificationCodeWithHttpInfo(phoneNumberId, requestWhatsAppVerificationCodeRequest)

Request OTP

Request a new OTP verification code from Meta for a pre-verified phone number. Useful when the initial SMS did not arrive or when re-verifying before the 90-day expiry. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.WhatsAppPhoneNumbersApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppPhoneNumbersApi apiInstance = new WhatsAppPhoneNumbersApi(defaultClient);
        String phoneNumberId = "phoneNumberId_example"; // String | Phone number record ID
        RequestWhatsAppVerificationCodeRequest requestWhatsAppVerificationCodeRequest = new RequestWhatsAppVerificationCodeRequest(); // RequestWhatsAppVerificationCodeRequest | 
        try {
            ApiResponse<RequestWhatsAppVerificationCode200Response> response = apiInstance.requestWhatsAppVerificationCodeWithHttpInfo(phoneNumberId, requestWhatsAppVerificationCodeRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppPhoneNumbersApi#requestWhatsAppVerificationCode");
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
| **phoneNumberId** | **String**| Phone number record ID | |
| **requestWhatsAppVerificationCodeRequest** | [**RequestWhatsAppVerificationCodeRequest**](RequestWhatsAppVerificationCodeRequest.md)|  | [optional] |

### Return type

ApiResponse<[**RequestWhatsAppVerificationCode200Response**](RequestWhatsAppVerificationCode200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Verification code requested successfully |  -  |
| **400** | Number has not been added to Meta pre-verified pool |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |


## searchAvailableWhatsAppNumbers

> SearchAvailableWhatsAppNumbers200Response searchAvailableWhatsAppNumbers(prefix, locality, contains, limit)

Search available numbers

Search for available US phone numbers that can be purchased for WhatsApp Business. Requires a paid plan. Numbers are sourced from Telnyx. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.WhatsAppPhoneNumbersApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppPhoneNumbersApi apiInstance = new WhatsAppPhoneNumbersApi(defaultClient);
        String prefix = "prefix_example"; // String | Area code to search (e.g., \"212\" for New York)
        String locality = "locality_example"; // String | City name (e.g., \"New York\")
        String contains = "contains_example"; // String | Pattern to match within the phone number
        Integer limit = 20; // Integer | Maximum results (default 20, max 100)
        try {
            SearchAvailableWhatsAppNumbers200Response result = apiInstance.searchAvailableWhatsAppNumbers(prefix, locality, contains, limit);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppPhoneNumbersApi#searchAvailableWhatsAppNumbers");
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
| **prefix** | **String**| Area code to search (e.g., \&quot;212\&quot; for New York) | [optional] |
| **locality** | **String**| City name (e.g., \&quot;New York\&quot;) | [optional] |
| **contains** | **String**| Pattern to match within the phone number | [optional] |
| **limit** | **Integer**| Maximum results (default 20, max 100) | [optional] [default to 20] |

### Return type

[**SearchAvailableWhatsAppNumbers200Response**](SearchAvailableWhatsAppNumbers200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Available numbers retrieved |  -  |
| **401** | Unauthorized |  -  |
| **403** | A paid plan is required |  -  |

## searchAvailableWhatsAppNumbersWithHttpInfo

> ApiResponse<SearchAvailableWhatsAppNumbers200Response> searchAvailableWhatsAppNumbers searchAvailableWhatsAppNumbersWithHttpInfo(prefix, locality, contains, limit)

Search available numbers

Search for available US phone numbers that can be purchased for WhatsApp Business. Requires a paid plan. Numbers are sourced from Telnyx. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.WhatsAppPhoneNumbersApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppPhoneNumbersApi apiInstance = new WhatsAppPhoneNumbersApi(defaultClient);
        String prefix = "prefix_example"; // String | Area code to search (e.g., \"212\" for New York)
        String locality = "locality_example"; // String | City name (e.g., \"New York\")
        String contains = "contains_example"; // String | Pattern to match within the phone number
        Integer limit = 20; // Integer | Maximum results (default 20, max 100)
        try {
            ApiResponse<SearchAvailableWhatsAppNumbers200Response> response = apiInstance.searchAvailableWhatsAppNumbersWithHttpInfo(prefix, locality, contains, limit);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppPhoneNumbersApi#searchAvailableWhatsAppNumbers");
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
| **prefix** | **String**| Area code to search (e.g., \&quot;212\&quot; for New York) | [optional] |
| **locality** | **String**| City name (e.g., \&quot;New York\&quot;) | [optional] |
| **contains** | **String**| Pattern to match within the phone number | [optional] |
| **limit** | **Integer**| Maximum results (default 20, max 100) | [optional] [default to 20] |

### Return type

ApiResponse<[**SearchAvailableWhatsAppNumbers200Response**](SearchAvailableWhatsAppNumbers200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Available numbers retrieved |  -  |
| **401** | Unauthorized |  -  |
| **403** | A paid plan is required |  -  |


## verifyWhatsAppPhoneNumber

> VerifyWhatsAppPhoneNumber200Response verifyWhatsAppPhoneNumber(phoneNumberId, verifyWhatsAppPhoneNumberRequest)

Verify OTP

Manually verify a phone number by entering the OTP code received via SMS or voice call. This is a fallback for when the auto-verification webhook does not capture the code. Verification is valid for 90 days. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.WhatsAppPhoneNumbersApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppPhoneNumbersApi apiInstance = new WhatsAppPhoneNumbersApi(defaultClient);
        String phoneNumberId = "phoneNumberId_example"; // String | Phone number record ID
        VerifyWhatsAppPhoneNumberRequest verifyWhatsAppPhoneNumberRequest = new VerifyWhatsAppPhoneNumberRequest(); // VerifyWhatsAppPhoneNumberRequest | 
        try {
            VerifyWhatsAppPhoneNumber200Response result = apiInstance.verifyWhatsAppPhoneNumber(phoneNumberId, verifyWhatsAppPhoneNumberRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppPhoneNumbersApi#verifyWhatsAppPhoneNumber");
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
| **phoneNumberId** | **String**| Phone number record ID | |
| **verifyWhatsAppPhoneNumberRequest** | [**VerifyWhatsAppPhoneNumberRequest**](VerifyWhatsAppPhoneNumberRequest.md)|  | |

### Return type

[**VerifyWhatsAppPhoneNumber200Response**](VerifyWhatsAppPhoneNumber200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Phone number verified successfully (or already verified) |  -  |
| **400** | Invalid code or number not in Meta pre-verified pool |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

## verifyWhatsAppPhoneNumberWithHttpInfo

> ApiResponse<VerifyWhatsAppPhoneNumber200Response> verifyWhatsAppPhoneNumber verifyWhatsAppPhoneNumberWithHttpInfo(phoneNumberId, verifyWhatsAppPhoneNumberRequest)

Verify OTP

Manually verify a phone number by entering the OTP code received via SMS or voice call. This is a fallback for when the auto-verification webhook does not capture the code. Verification is valid for 90 days. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.WhatsAppPhoneNumbersApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        WhatsAppPhoneNumbersApi apiInstance = new WhatsAppPhoneNumbersApi(defaultClient);
        String phoneNumberId = "phoneNumberId_example"; // String | Phone number record ID
        VerifyWhatsAppPhoneNumberRequest verifyWhatsAppPhoneNumberRequest = new VerifyWhatsAppPhoneNumberRequest(); // VerifyWhatsAppPhoneNumberRequest | 
        try {
            ApiResponse<VerifyWhatsAppPhoneNumber200Response> response = apiInstance.verifyWhatsAppPhoneNumberWithHttpInfo(phoneNumberId, verifyWhatsAppPhoneNumberRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling WhatsAppPhoneNumbersApi#verifyWhatsAppPhoneNumber");
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
| **phoneNumberId** | **String**| Phone number record ID | |
| **verifyWhatsAppPhoneNumberRequest** | [**VerifyWhatsAppPhoneNumberRequest**](VerifyWhatsAppPhoneNumberRequest.md)|  | |

### Return type

ApiResponse<[**VerifyWhatsAppPhoneNumber200Response**](VerifyWhatsAppPhoneNumber200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Phone number verified successfully (or already verified) |  -  |
| **400** | Invalid code or number not in Meta pre-verified pool |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |

