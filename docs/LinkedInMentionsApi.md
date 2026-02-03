# LinkedInMentionsApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getLinkedInMentions**](LinkedInMentionsApi.md#getLinkedInMentions) | **GET** /v1/accounts/{accountId}/linkedin-mentions | Resolve a LinkedIn profile or company URL to a URN for @mentions |
| [**getLinkedInMentionsWithHttpInfo**](LinkedInMentionsApi.md#getLinkedInMentionsWithHttpInfo) | **GET** /v1/accounts/{accountId}/linkedin-mentions | Resolve a LinkedIn profile or company URL to a URN for @mentions |



## getLinkedInMentions

> GetLinkedInMentions200Response getLinkedInMentions(accountId, url, displayName)

Resolve a LinkedIn profile or company URL to a URN for @mentions

Converts a LinkedIn profile URL (person) or company page URL (organization) to a URN that can be used to @mention them in posts.  **Supports both:** - **Person mentions:** &#x60;linkedin.com/in/username&#x60; or just &#x60;username&#x60; - **Organization mentions:** &#x60;linkedin.com/company/company-name&#x60; or &#x60;company/company-name&#x60;  **⚠️ Organization Admin Required for Person Mentions Only:** Person mentions require the connected LinkedIn account to have admin access to at least one LinkedIn Organization (Company Page). Organization mentions do NOT have this requirement - any LinkedIn account can tag companies.  **IMPORTANT - Display Name Requirement:** For **person mentions** to be clickable, the display name must **exactly match** what appears on their LinkedIn profile. - Organization mentions automatically retrieve the company name from LinkedIn API - Person mentions require the exact name, so provide the &#x60;displayName&#x60; parameter  **Mention Format:** Use the returned &#x60;mentionFormat&#x60; value directly in your post content: &#x60;&#x60;&#x60; Great insights from @[Miquel Palet](urn:li:person:4qj5ox-agD) on this topic! Excited to partner with @[Microsoft](urn:li:organization:1035)! &#x60;&#x60;&#x60; 

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
        String url = "miquelpalet"; // String | LinkedIn profile URL, company URL, or vanity name. - Person: `miquelpalet`, `linkedin.com/in/miquelpalet` - Organization: `company/microsoft`, `linkedin.com/company/microsoft` 
        String displayName = "Miquel Palet"; // String | The exact display name as shown on LinkedIn. - **Person mentions:** Required for clickable mentions. If not provided, a name is derived from the vanity URL which may not match exactly. - **Organization mentions:** Optional. If not provided, the company name is automatically retrieved from LinkedIn. 
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
| **url** | **String**| LinkedIn profile URL, company URL, or vanity name. - Person: &#x60;miquelpalet&#x60;, &#x60;linkedin.com/in/miquelpalet&#x60; - Organization: &#x60;company/microsoft&#x60;, &#x60;linkedin.com/company/microsoft&#x60;  | |
| **displayName** | **String**| The exact display name as shown on LinkedIn. - **Person mentions:** Required for clickable mentions. If not provided, a name is derived from the vanity URL which may not match exactly. - **Organization mentions:** Optional. If not provided, the company name is automatically retrieved from LinkedIn.  | [optional] |

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

Resolve a LinkedIn profile or company URL to a URN for @mentions

Converts a LinkedIn profile URL (person) or company page URL (organization) to a URN that can be used to @mention them in posts.  **Supports both:** - **Person mentions:** &#x60;linkedin.com/in/username&#x60; or just &#x60;username&#x60; - **Organization mentions:** &#x60;linkedin.com/company/company-name&#x60; or &#x60;company/company-name&#x60;  **⚠️ Organization Admin Required for Person Mentions Only:** Person mentions require the connected LinkedIn account to have admin access to at least one LinkedIn Organization (Company Page). Organization mentions do NOT have this requirement - any LinkedIn account can tag companies.  **IMPORTANT - Display Name Requirement:** For **person mentions** to be clickable, the display name must **exactly match** what appears on their LinkedIn profile. - Organization mentions automatically retrieve the company name from LinkedIn API - Person mentions require the exact name, so provide the &#x60;displayName&#x60; parameter  **Mention Format:** Use the returned &#x60;mentionFormat&#x60; value directly in your post content: &#x60;&#x60;&#x60; Great insights from @[Miquel Palet](urn:li:person:4qj5ox-agD) on this topic! Excited to partner with @[Microsoft](urn:li:organization:1035)! &#x60;&#x60;&#x60; 

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
        String url = "miquelpalet"; // String | LinkedIn profile URL, company URL, or vanity name. - Person: `miquelpalet`, `linkedin.com/in/miquelpalet` - Organization: `company/microsoft`, `linkedin.com/company/microsoft` 
        String displayName = "Miquel Palet"; // String | The exact display name as shown on LinkedIn. - **Person mentions:** Required for clickable mentions. If not provided, a name is derived from the vanity URL which may not match exactly. - **Organization mentions:** Optional. If not provided, the company name is automatically retrieved from LinkedIn. 
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
| **url** | **String**| LinkedIn profile URL, company URL, or vanity name. - Person: &#x60;miquelpalet&#x60;, &#x60;linkedin.com/in/miquelpalet&#x60; - Organization: &#x60;company/microsoft&#x60;, &#x60;linkedin.com/company/microsoft&#x60;  | |
| **displayName** | **String**| The exact display name as shown on LinkedIn. - **Person mentions:** Required for clickable mentions. If not provided, a name is derived from the vanity URL which may not match exactly. - **Organization mentions:** Optional. If not provided, the company name is automatically retrieved from LinkedIn.  | [optional] |

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

