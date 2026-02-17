# LinkedInMentionsApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getLinkedInMentions**](LinkedInMentionsApi.md#getLinkedInMentions) | **GET** /v1/accounts/{accountId}/linkedin-mentions | Resolve LinkedIn mention |
| [**getLinkedInMentionsWithHttpInfo**](LinkedInMentionsApi.md#getLinkedInMentionsWithHttpInfo) | **GET** /v1/accounts/{accountId}/linkedin-mentions | Resolve LinkedIn mention |



## getLinkedInMentions

> GetLinkedInMentions200Response getLinkedInMentions(accountId, url, displayName)

Resolve LinkedIn mention

Converts a LinkedIn profile or company URL to a URN for @mentions in posts. Person mentions require org admin access. Use the returned mentionFormat in post content.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.LinkedInMentionsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LinkedInMentionsApi apiInstance = new LinkedInMentionsApi(defaultClient);
        String accountId = "accountId_example"; // String | The LinkedIn account ID
        String url = "miquelpalet"; // String | LinkedIn profile URL, company URL, or vanity name.
        String displayName = "Miquel Palet"; // String | Exact display name as shown on LinkedIn. Required for person mentions to be clickable. Optional for org mentions.
        try {
            GetLinkedInMentions200Response result = apiInstance.getLinkedInMentions(accountId, url, displayName);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling LinkedInMentionsApi#getLinkedInMentions");
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
| **accountId** | **String**| The LinkedIn account ID | |
| **url** | **String**| LinkedIn profile URL, company URL, or vanity name. | |
| **displayName** | **String**| Exact display name as shown on LinkedIn. Required for person mentions to be clickable. Optional for org mentions. | [optional] |

### Return type

[**GetLinkedInMentions200Response**](GetLinkedInMentions200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | URN resolved successfully |  -  |
| **400** | Invalid request or no organization found (for person mentions) |  -  |
| **401** | Unauthorized |  -  |
| **404** | Person or organization not found |  -  |

## getLinkedInMentionsWithHttpInfo

> ApiResponse<GetLinkedInMentions200Response> getLinkedInMentions getLinkedInMentionsWithHttpInfo(accountId, url, displayName)

Resolve LinkedIn mention

Converts a LinkedIn profile or company URL to a URN for @mentions in posts. Person mentions require org admin access. Use the returned mentionFormat in post content.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.LinkedInMentionsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        LinkedInMentionsApi apiInstance = new LinkedInMentionsApi(defaultClient);
        String accountId = "accountId_example"; // String | The LinkedIn account ID
        String url = "miquelpalet"; // String | LinkedIn profile URL, company URL, or vanity name.
        String displayName = "Miquel Palet"; // String | Exact display name as shown on LinkedIn. Required for person mentions to be clickable. Optional for org mentions.
        try {
            ApiResponse<GetLinkedInMentions200Response> response = apiInstance.getLinkedInMentionsWithHttpInfo(accountId, url, displayName);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling LinkedInMentionsApi#getLinkedInMentions");
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
| **accountId** | **String**| The LinkedIn account ID | |
| **url** | **String**| LinkedIn profile URL, company URL, or vanity name. | |
| **displayName** | **String**| Exact display name as shown on LinkedIn. Required for person mentions to be clickable. Optional for org mentions. | [optional] |

### Return type

ApiResponse<[**GetLinkedInMentions200Response**](GetLinkedInMentions200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | URN resolved successfully |  -  |
| **400** | Invalid request or no organization found (for person mentions) |  -  |
| **401** | Unauthorized |  -  |
| **404** | Person or organization not found |  -  |

