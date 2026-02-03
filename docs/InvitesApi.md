# InvitesApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createInviteToken**](InvitesApi.md#createInviteToken) | **POST** /v1/invite/tokens | Create a team member invite token |
| [**createInviteTokenWithHttpInfo**](InvitesApi.md#createInviteTokenWithHttpInfo) | **POST** /v1/invite/tokens | Create a team member invite token |



## createInviteToken

> CreateInviteToken201Response createInviteToken(createInviteTokenRequest)

Create a team member invite token

Generate a secure invite link to grant team members access to your profiles. Invites expire after 7 days and are single-use. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.InvitesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        InvitesApi apiInstance = new InvitesApi(defaultClient);
        CreateInviteTokenRequest createInviteTokenRequest = new CreateInviteTokenRequest(); // CreateInviteTokenRequest | 
        try {
            CreateInviteToken201Response result = apiInstance.createInviteToken(createInviteTokenRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling InvitesApi#createInviteToken");
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
| **createInviteTokenRequest** | [**CreateInviteTokenRequest**](CreateInviteTokenRequest.md)|  | |

### Return type

[**CreateInviteToken201Response**](CreateInviteToken201Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Invite token created |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |
| **403** | One or more profiles not found or not owned |  -  |

## createInviteTokenWithHttpInfo

> ApiResponse<CreateInviteToken201Response> createInviteToken createInviteTokenWithHttpInfo(createInviteTokenRequest)

Create a team member invite token

Generate a secure invite link to grant team members access to your profiles. Invites expire after 7 days and are single-use. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.InvitesApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        InvitesApi apiInstance = new InvitesApi(defaultClient);
        CreateInviteTokenRequest createInviteTokenRequest = new CreateInviteTokenRequest(); // CreateInviteTokenRequest | 
        try {
            ApiResponse<CreateInviteToken201Response> response = apiInstance.createInviteTokenWithHttpInfo(createInviteTokenRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling InvitesApi#createInviteToken");
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
| **createInviteTokenRequest** | [**CreateInviteTokenRequest**](CreateInviteTokenRequest.md)|  | |

### Return type

ApiResponse<[**CreateInviteToken201Response**](CreateInviteToken201Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Invite token created |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |
| **403** | One or more profiles not found or not owned |  -  |

