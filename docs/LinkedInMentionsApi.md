# LinkedInMentionsApi

All URIs are relative to *https://zernio.com/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getLinkedInMentions**](LinkedInMentionsApi.md#getLinkedInMentions) | **GET** /v1/accounts/{accountId}/linkedin-mentions | Resolve LinkedIn mention |
| [**getLinkedInMentionsWithHttpInfo**](LinkedInMentionsApi.md#getLinkedInMentionsWithHttpInfo) | **GET** /v1/accounts/{accountId}/linkedin-mentions | Resolve LinkedIn mention |



## getLinkedInMentions

> GetLinkedInMentions200Response getLinkedInMentions(accountId, url, displayName)

Resolve LinkedIn mention

Converts a LinkedIn profile or company URL to a URN for @mentions in posts.  **How to use LinkedIn @mentions (2-step workflow):**  1. Call this endpoint with the LinkedIn profile/company URL to get the mention URN and format. 2. Embed the returned &#x60;mentionFormat&#x60; (e.g. &#x60;@[Vincent Jong](urn:li:person:xxx)&#x60;) directly in your post&#39;s &#x60;content&#x60; field.  **Example:** - Resolve: &#x60;GET /v1/accounts/{id}/linkedin-mentions?url&#x3D;linkedin.com/in/vincentjong&amp;displayName&#x3D;Vincent Jong&#x60; - Returns: &#x60;mentionFormat: \&quot;@[Vincent Jong](urn:li:person:xxx)\&quot;&#x60; - Use in post content: &#x60;\&quot;Great talk with @[Vincent Jong](urn:li:person:xxx) today!\&quot;&#x60;  **Important:** The &#x60;mentions&#x60; array field in POST /v1/posts is stored for reference only and does NOT trigger @mentions on LinkedIn. You must embed the mention format directly in the content text.  **Requirements:** - **Person mentions** require the LinkedIn account to be admin of at least one organization. This is a LinkedIn API limitation: the only endpoints that resolve profile URLs to member URNs (&#x60;vanityUrl&#x60;, &#x60;peopleTypeahead&#x60;) are scoped to organization followers. There is no public LinkedIn API to resolve a vanity URL without organization context. - **Organization mentions** (e.g. @Microsoft) work without this requirement. - For person mentions to be clickable, the &#x60;displayName&#x60; parameter must exactly match the name shown on their LinkedIn profile. - Person mentions DO work when published from personal profiles (the URN just needs to be valid). The limitation is only in the resolution step (URL to URN), not in publishing. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LinkedInMentionsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Converts a LinkedIn profile or company URL to a URN for @mentions in posts.  **How to use LinkedIn @mentions (2-step workflow):**  1. Call this endpoint with the LinkedIn profile/company URL to get the mention URN and format. 2. Embed the returned &#x60;mentionFormat&#x60; (e.g. &#x60;@[Vincent Jong](urn:li:person:xxx)&#x60;) directly in your post&#39;s &#x60;content&#x60; field.  **Example:** - Resolve: &#x60;GET /v1/accounts/{id}/linkedin-mentions?url&#x3D;linkedin.com/in/vincentjong&amp;displayName&#x3D;Vincent Jong&#x60; - Returns: &#x60;mentionFormat: \&quot;@[Vincent Jong](urn:li:person:xxx)\&quot;&#x60; - Use in post content: &#x60;\&quot;Great talk with @[Vincent Jong](urn:li:person:xxx) today!\&quot;&#x60;  **Important:** The &#x60;mentions&#x60; array field in POST /v1/posts is stored for reference only and does NOT trigger @mentions on LinkedIn. You must embed the mention format directly in the content text.  **Requirements:** - **Person mentions** require the LinkedIn account to be admin of at least one organization. This is a LinkedIn API limitation: the only endpoints that resolve profile URLs to member URNs (&#x60;vanityUrl&#x60;, &#x60;peopleTypeahead&#x60;) are scoped to organization followers. There is no public LinkedIn API to resolve a vanity URL without organization context. - **Organization mentions** (e.g. @Microsoft) work without this requirement. - For person mentions to be clickable, the &#x60;displayName&#x60; parameter must exactly match the name shown on their LinkedIn profile. - Person mentions DO work when published from personal profiles (the URN just needs to be valid). The limitation is only in the resolution step (URL to URN), not in publishing. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.LinkedInMentionsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

