# ConnectApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**completeTelegramConnect**](ConnectApi.md#completeTelegramConnect) | **PATCH** /v1/connect/telegram | Check Telegram status |
| [**completeTelegramConnectWithHttpInfo**](ConnectApi.md#completeTelegramConnectWithHttpInfo) | **PATCH** /v1/connect/telegram | Check Telegram status |
| [**connectBlueskyCredentials**](ConnectApi.md#connectBlueskyCredentials) | **POST** /v1/connect/bluesky/credentials | Connect Bluesky account |
| [**connectBlueskyCredentialsWithHttpInfo**](ConnectApi.md#connectBlueskyCredentialsWithHttpInfo) | **POST** /v1/connect/bluesky/credentials | Connect Bluesky account |
| [**getConnectUrl**](ConnectApi.md#getConnectUrl) | **GET** /v1/connect/{platform} | Get OAuth connect URL |
| [**getConnectUrlWithHttpInfo**](ConnectApi.md#getConnectUrlWithHttpInfo) | **GET** /v1/connect/{platform} | Get OAuth connect URL |
| [**getFacebookPages**](ConnectApi.md#getFacebookPages) | **GET** /v1/accounts/{accountId}/facebook-page | List Facebook pages |
| [**getFacebookPagesWithHttpInfo**](ConnectApi.md#getFacebookPagesWithHttpInfo) | **GET** /v1/accounts/{accountId}/facebook-page | List Facebook pages |
| [**getGmbLocations**](ConnectApi.md#getGmbLocations) | **GET** /v1/accounts/{accountId}/gmb-locations | List Google Business locations |
| [**getGmbLocationsWithHttpInfo**](ConnectApi.md#getGmbLocationsWithHttpInfo) | **GET** /v1/accounts/{accountId}/gmb-locations | List Google Business locations |
| [**getLinkedInOrganizations**](ConnectApi.md#getLinkedInOrganizations) | **GET** /v1/accounts/{accountId}/linkedin-organizations | List LinkedIn orgs |
| [**getLinkedInOrganizationsWithHttpInfo**](ConnectApi.md#getLinkedInOrganizationsWithHttpInfo) | **GET** /v1/accounts/{accountId}/linkedin-organizations | List LinkedIn orgs |
| [**getPendingOAuthData**](ConnectApi.md#getPendingOAuthData) | **GET** /v1/connect/pending-data | Get pending OAuth data |
| [**getPendingOAuthDataWithHttpInfo**](ConnectApi.md#getPendingOAuthDataWithHttpInfo) | **GET** /v1/connect/pending-data | Get pending OAuth data |
| [**getPinterestBoards**](ConnectApi.md#getPinterestBoards) | **GET** /v1/accounts/{accountId}/pinterest-boards | List Pinterest boards |
| [**getPinterestBoardsWithHttpInfo**](ConnectApi.md#getPinterestBoardsWithHttpInfo) | **GET** /v1/accounts/{accountId}/pinterest-boards | List Pinterest boards |
| [**getRedditFlairs**](ConnectApi.md#getRedditFlairs) | **GET** /v1/accounts/{accountId}/reddit-flairs | List subreddit flairs |
| [**getRedditFlairsWithHttpInfo**](ConnectApi.md#getRedditFlairsWithHttpInfo) | **GET** /v1/accounts/{accountId}/reddit-flairs | List subreddit flairs |
| [**getRedditSubreddits**](ConnectApi.md#getRedditSubreddits) | **GET** /v1/accounts/{accountId}/reddit-subreddits | List Reddit subreddits |
| [**getRedditSubredditsWithHttpInfo**](ConnectApi.md#getRedditSubredditsWithHttpInfo) | **GET** /v1/accounts/{accountId}/reddit-subreddits | List Reddit subreddits |
| [**getTelegramConnectStatus**](ConnectApi.md#getTelegramConnectStatus) | **GET** /v1/connect/telegram | Generate Telegram code |
| [**getTelegramConnectStatusWithHttpInfo**](ConnectApi.md#getTelegramConnectStatusWithHttpInfo) | **GET** /v1/connect/telegram | Generate Telegram code |
| [**handleOAuthCallback**](ConnectApi.md#handleOAuthCallback) | **POST** /v1/connect/{platform} | Complete OAuth callback |
| [**handleOAuthCallbackWithHttpInfo**](ConnectApi.md#handleOAuthCallbackWithHttpInfo) | **POST** /v1/connect/{platform} | Complete OAuth callback |
| [**initiateTelegramConnect**](ConnectApi.md#initiateTelegramConnect) | **POST** /v1/connect/telegram | Connect Telegram directly |
| [**initiateTelegramConnectWithHttpInfo**](ConnectApi.md#initiateTelegramConnectWithHttpInfo) | **POST** /v1/connect/telegram | Connect Telegram directly |
| [**listFacebookPages**](ConnectApi.md#listFacebookPages) | **GET** /v1/connect/facebook/select-page | List Facebook pages |
| [**listFacebookPagesWithHttpInfo**](ConnectApi.md#listFacebookPagesWithHttpInfo) | **GET** /v1/connect/facebook/select-page | List Facebook pages |
| [**listGoogleBusinessLocations**](ConnectApi.md#listGoogleBusinessLocations) | **GET** /v1/connect/googlebusiness/locations | List Google Business locations |
| [**listGoogleBusinessLocationsWithHttpInfo**](ConnectApi.md#listGoogleBusinessLocationsWithHttpInfo) | **GET** /v1/connect/googlebusiness/locations | List Google Business locations |
| [**listLinkedInOrganizations**](ConnectApi.md#listLinkedInOrganizations) | **GET** /v1/connect/linkedin/organizations | List LinkedIn orgs |
| [**listLinkedInOrganizationsWithHttpInfo**](ConnectApi.md#listLinkedInOrganizationsWithHttpInfo) | **GET** /v1/connect/linkedin/organizations | List LinkedIn orgs |
| [**listPinterestBoardsForSelection**](ConnectApi.md#listPinterestBoardsForSelection) | **GET** /v1/connect/pinterest/select-board | List Pinterest boards |
| [**listPinterestBoardsForSelectionWithHttpInfo**](ConnectApi.md#listPinterestBoardsForSelectionWithHttpInfo) | **GET** /v1/connect/pinterest/select-board | List Pinterest boards |
| [**listSnapchatProfiles**](ConnectApi.md#listSnapchatProfiles) | **GET** /v1/connect/snapchat/select-profile | List Snapchat profiles |
| [**listSnapchatProfilesWithHttpInfo**](ConnectApi.md#listSnapchatProfilesWithHttpInfo) | **GET** /v1/connect/snapchat/select-profile | List Snapchat profiles |
| [**selectFacebookPage**](ConnectApi.md#selectFacebookPage) | **POST** /v1/connect/facebook/select-page | Select Facebook page |
| [**selectFacebookPageWithHttpInfo**](ConnectApi.md#selectFacebookPageWithHttpInfo) | **POST** /v1/connect/facebook/select-page | Select Facebook page |
| [**selectGoogleBusinessLocation**](ConnectApi.md#selectGoogleBusinessLocation) | **POST** /v1/connect/googlebusiness/select-location | Select Google Business location |
| [**selectGoogleBusinessLocationWithHttpInfo**](ConnectApi.md#selectGoogleBusinessLocationWithHttpInfo) | **POST** /v1/connect/googlebusiness/select-location | Select Google Business location |
| [**selectLinkedInOrganization**](ConnectApi.md#selectLinkedInOrganization) | **POST** /v1/connect/linkedin/select-organization | Select LinkedIn org |
| [**selectLinkedInOrganizationWithHttpInfo**](ConnectApi.md#selectLinkedInOrganizationWithHttpInfo) | **POST** /v1/connect/linkedin/select-organization | Select LinkedIn org |
| [**selectPinterestBoard**](ConnectApi.md#selectPinterestBoard) | **POST** /v1/connect/pinterest/select-board | Select Pinterest board |
| [**selectPinterestBoardWithHttpInfo**](ConnectApi.md#selectPinterestBoardWithHttpInfo) | **POST** /v1/connect/pinterest/select-board | Select Pinterest board |
| [**selectSnapchatProfile**](ConnectApi.md#selectSnapchatProfile) | **POST** /v1/connect/snapchat/select-profile | Select Snapchat profile |
| [**selectSnapchatProfileWithHttpInfo**](ConnectApi.md#selectSnapchatProfileWithHttpInfo) | **POST** /v1/connect/snapchat/select-profile | Select Snapchat profile |
| [**updateFacebookPage**](ConnectApi.md#updateFacebookPage) | **PUT** /v1/accounts/{accountId}/facebook-page | Update Facebook page |
| [**updateFacebookPageWithHttpInfo**](ConnectApi.md#updateFacebookPageWithHttpInfo) | **PUT** /v1/accounts/{accountId}/facebook-page | Update Facebook page |
| [**updateGmbLocation**](ConnectApi.md#updateGmbLocation) | **PUT** /v1/accounts/{accountId}/gmb-locations | Update Google Business location |
| [**updateGmbLocationWithHttpInfo**](ConnectApi.md#updateGmbLocationWithHttpInfo) | **PUT** /v1/accounts/{accountId}/gmb-locations | Update Google Business location |
| [**updateLinkedInOrganization**](ConnectApi.md#updateLinkedInOrganization) | **PUT** /v1/accounts/{accountId}/linkedin-organization | Switch LinkedIn account type |
| [**updateLinkedInOrganizationWithHttpInfo**](ConnectApi.md#updateLinkedInOrganizationWithHttpInfo) | **PUT** /v1/accounts/{accountId}/linkedin-organization | Switch LinkedIn account type |
| [**updatePinterestBoards**](ConnectApi.md#updatePinterestBoards) | **PUT** /v1/accounts/{accountId}/pinterest-boards | Set default Pinterest board |
| [**updatePinterestBoardsWithHttpInfo**](ConnectApi.md#updatePinterestBoardsWithHttpInfo) | **PUT** /v1/accounts/{accountId}/pinterest-boards | Set default Pinterest board |
| [**updateRedditSubreddits**](ConnectApi.md#updateRedditSubreddits) | **PUT** /v1/accounts/{accountId}/reddit-subreddits | Set default subreddit |
| [**updateRedditSubredditsWithHttpInfo**](ConnectApi.md#updateRedditSubredditsWithHttpInfo) | **PUT** /v1/accounts/{accountId}/reddit-subreddits | Set default subreddit |



## completeTelegramConnect

> CompleteTelegramConnect200Response completeTelegramConnect(code)

Check Telegram status

Poll this endpoint to check if a Telegram access code has been used to connect a channel/group.  **Recommended polling interval:** 3 seconds  **Status values:** - &#x60;pending&#x60;: Code is valid, waiting for user to complete connection - &#x60;connected&#x60;: Connection successful - channel/group is now linked - &#x60;expired&#x60;: Code has expired, generate a new one 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String code = "LATE-ABC123"; // String | The access code to check status for
        try {
            CompleteTelegramConnect200Response result = apiInstance.completeTelegramConnect(code);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#completeTelegramConnect");
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
| **code** | **String**| The access code to check status for | |

### Return type

[**CompleteTelegramConnect200Response**](CompleteTelegramConnect200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Connection status |  -  |
| **401** | Unauthorized |  -  |
| **404** | Code not found |  -  |
| **500** | Internal error |  -  |

## completeTelegramConnectWithHttpInfo

> ApiResponse<CompleteTelegramConnect200Response> completeTelegramConnect completeTelegramConnectWithHttpInfo(code)

Check Telegram status

Poll this endpoint to check if a Telegram access code has been used to connect a channel/group.  **Recommended polling interval:** 3 seconds  **Status values:** - &#x60;pending&#x60;: Code is valid, waiting for user to complete connection - &#x60;connected&#x60;: Connection successful - channel/group is now linked - &#x60;expired&#x60;: Code has expired, generate a new one 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String code = "LATE-ABC123"; // String | The access code to check status for
        try {
            ApiResponse<CompleteTelegramConnect200Response> response = apiInstance.completeTelegramConnectWithHttpInfo(code);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#completeTelegramConnect");
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
| **code** | **String**| The access code to check status for | |

### Return type

ApiResponse<[**CompleteTelegramConnect200Response**](CompleteTelegramConnect200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Connection status |  -  |
| **401** | Unauthorized |  -  |
| **404** | Code not found |  -  |
| **500** | Internal error |  -  |


## connectBlueskyCredentials

> ConnectBlueskyCredentials200Response connectBlueskyCredentials(connectBlueskyCredentialsRequest)

Connect Bluesky account

Connect a Bluesky account using identifier (handle or email) and an app password.  To get your userId for the state parameter, call &#x60;GET /v1/users&#x60; - the response includes a &#x60;currentUserId&#x60; field. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        ConnectBlueskyCredentialsRequest connectBlueskyCredentialsRequest = new ConnectBlueskyCredentialsRequest(); // ConnectBlueskyCredentialsRequest | 
        try {
            ConnectBlueskyCredentials200Response result = apiInstance.connectBlueskyCredentials(connectBlueskyCredentialsRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#connectBlueskyCredentials");
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
| **connectBlueskyCredentialsRequest** | [**ConnectBlueskyCredentialsRequest**](ConnectBlueskyCredentialsRequest.md)|  | |

### Return type

[**ConnectBlueskyCredentials200Response**](ConnectBlueskyCredentials200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Bluesky connected successfully |  -  |
| **400** | Invalid request - missing fields or invalid state format |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal error |  -  |

## connectBlueskyCredentialsWithHttpInfo

> ApiResponse<ConnectBlueskyCredentials200Response> connectBlueskyCredentials connectBlueskyCredentialsWithHttpInfo(connectBlueskyCredentialsRequest)

Connect Bluesky account

Connect a Bluesky account using identifier (handle or email) and an app password.  To get your userId for the state parameter, call &#x60;GET /v1/users&#x60; - the response includes a &#x60;currentUserId&#x60; field. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        ConnectBlueskyCredentialsRequest connectBlueskyCredentialsRequest = new ConnectBlueskyCredentialsRequest(); // ConnectBlueskyCredentialsRequest | 
        try {
            ApiResponse<ConnectBlueskyCredentials200Response> response = apiInstance.connectBlueskyCredentialsWithHttpInfo(connectBlueskyCredentialsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#connectBlueskyCredentials");
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
| **connectBlueskyCredentialsRequest** | [**ConnectBlueskyCredentialsRequest**](ConnectBlueskyCredentialsRequest.md)|  | |

### Return type

ApiResponse<[**ConnectBlueskyCredentials200Response**](ConnectBlueskyCredentials200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Bluesky connected successfully |  -  |
| **400** | Invalid request - missing fields or invalid state format |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal error |  -  |


## getConnectUrl

> GetConnectUrl200Response getConnectUrl(platform, profileId, redirectUrl)

Get OAuth connect URL

Initiate an OAuth connection flow for any supported social media platform.  **Standard Flow (Hosted UI):** 1. Call this endpoint with your API key and &#x60;redirect_url&#x60; (optional) 2. Redirect your user to the returned &#x60;authUrl&#x60; 3. After OAuth, Late hosts the page/account selection UI 4. Once the user picks, Late saves the connection and redirects to your &#x60;redirect_url&#x60; (if provided)  **Headless Mode (Facebook, LinkedIn, Pinterest, Google Business, Snapchat):** Build your own branded selection UI while Late handles OAuth. Add &#x60;&amp;headless&#x3D;true&#x60; to this endpoint:  &#x60;GET /v1/connect/{platform}?profileId&#x3D;PROFILE_ID&amp;redirect_url&#x3D;https://yourapp.com/callback&amp;headless&#x3D;true&#x60;  After OAuth, the user is redirected to your &#x60;redirect_url&#x60; with OAuth data including &#x60;profileId&#x60;, &#x60;tempToken&#x60;, &#x60;userProfile&#x60;, &#x60;connect_token&#x60;, &#x60;platform&#x60;, and a &#x60;step&#x60; parameter indicating what selection is needed.  **Facebook example:** 1. Redirect params include &#x60;step&#x3D;select_page&#x60; 2. Use &#x60;GET /v1/connect/facebook/select-page&#x60; to fetch pages 3. Use &#x60;POST /v1/connect/facebook/select-page&#x60; to save the selected page  LinkedIn, Pinterest, Google Business, and Snapchat follow the same pattern with their respective selection endpoints. LinkedIn uses &#x60;pendingDataToken&#x60; instead of &#x60;tempToken&#x60; in redirect params; call &#x60;GET /v1/connect/pending-data?token&#x3D;TOKEN&#x60; to retrieve the OAuth data (one-time use, expires in 10 minutes). 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String platform = "facebook"; // String | Social media platform to connect
        String profileId = "profileId_example"; // String | Your Late profile ID (get from /v1/profiles)
        URI redirectUrl = new URI(); // URI | Your custom redirect URL after connection completes.  **Standard Mode:** After the user selects an account, Late redirects here with `?connected={platform}&profileId=X&username=Y`.  **Headless Mode:** Pass `headless=true` as a query parameter on this endpoint. After OAuth, the user is redirected to your URL with OAuth data (`profileId`, `tempToken`, `userProfile`, `connect_token`, `platform`, `step`). See the main endpoint description for details.  Example: `https://yourdomain.com/integrations/callback` 
        try {
            GetConnectUrl200Response result = apiInstance.getConnectUrl(platform, profileId, redirectUrl);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#getConnectUrl");
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
| **platform** | **String**| Social media platform to connect | [enum: facebook, instagram, linkedin, twitter, tiktok, youtube, threads, reddit, pinterest, bluesky, googlebusiness, telegram, snapchat] |
| **profileId** | **String**| Your Late profile ID (get from /v1/profiles) | |
| **redirectUrl** | **URI**| Your custom redirect URL after connection completes.  **Standard Mode:** After the user selects an account, Late redirects here with &#x60;?connected&#x3D;{platform}&amp;profileId&#x3D;X&amp;username&#x3D;Y&#x60;.  **Headless Mode:** Pass &#x60;headless&#x3D;true&#x60; as a query parameter on this endpoint. After OAuth, the user is redirected to your URL with OAuth data (&#x60;profileId&#x60;, &#x60;tempToken&#x60;, &#x60;userProfile&#x60;, &#x60;connect_token&#x60;, &#x60;platform&#x60;, &#x60;step&#x60;). See the main endpoint description for details.  Example: &#x60;https://yourdomain.com/integrations/callback&#x60;  | [optional] |

### Return type

[**GetConnectUrl200Response**](GetConnectUrl200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OAuth authorization URL to redirect user to |  -  |
| **400** | Missing/invalid parameters (e.g., invalid profileId format) |  -  |
| **401** | Unauthorized |  -  |
| **403** | No access to profile, or BYOK required for AppSumo Twitter |  -  |
| **404** | Profile not found |  -  |

## getConnectUrlWithHttpInfo

> ApiResponse<GetConnectUrl200Response> getConnectUrl getConnectUrlWithHttpInfo(platform, profileId, redirectUrl)

Get OAuth connect URL

Initiate an OAuth connection flow for any supported social media platform.  **Standard Flow (Hosted UI):** 1. Call this endpoint with your API key and &#x60;redirect_url&#x60; (optional) 2. Redirect your user to the returned &#x60;authUrl&#x60; 3. After OAuth, Late hosts the page/account selection UI 4. Once the user picks, Late saves the connection and redirects to your &#x60;redirect_url&#x60; (if provided)  **Headless Mode (Facebook, LinkedIn, Pinterest, Google Business, Snapchat):** Build your own branded selection UI while Late handles OAuth. Add &#x60;&amp;headless&#x3D;true&#x60; to this endpoint:  &#x60;GET /v1/connect/{platform}?profileId&#x3D;PROFILE_ID&amp;redirect_url&#x3D;https://yourapp.com/callback&amp;headless&#x3D;true&#x60;  After OAuth, the user is redirected to your &#x60;redirect_url&#x60; with OAuth data including &#x60;profileId&#x60;, &#x60;tempToken&#x60;, &#x60;userProfile&#x60;, &#x60;connect_token&#x60;, &#x60;platform&#x60;, and a &#x60;step&#x60; parameter indicating what selection is needed.  **Facebook example:** 1. Redirect params include &#x60;step&#x3D;select_page&#x60; 2. Use &#x60;GET /v1/connect/facebook/select-page&#x60; to fetch pages 3. Use &#x60;POST /v1/connect/facebook/select-page&#x60; to save the selected page  LinkedIn, Pinterest, Google Business, and Snapchat follow the same pattern with their respective selection endpoints. LinkedIn uses &#x60;pendingDataToken&#x60; instead of &#x60;tempToken&#x60; in redirect params; call &#x60;GET /v1/connect/pending-data?token&#x3D;TOKEN&#x60; to retrieve the OAuth data (one-time use, expires in 10 minutes). 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String platform = "facebook"; // String | Social media platform to connect
        String profileId = "profileId_example"; // String | Your Late profile ID (get from /v1/profiles)
        URI redirectUrl = new URI(); // URI | Your custom redirect URL after connection completes.  **Standard Mode:** After the user selects an account, Late redirects here with `?connected={platform}&profileId=X&username=Y`.  **Headless Mode:** Pass `headless=true` as a query parameter on this endpoint. After OAuth, the user is redirected to your URL with OAuth data (`profileId`, `tempToken`, `userProfile`, `connect_token`, `platform`, `step`). See the main endpoint description for details.  Example: `https://yourdomain.com/integrations/callback` 
        try {
            ApiResponse<GetConnectUrl200Response> response = apiInstance.getConnectUrlWithHttpInfo(platform, profileId, redirectUrl);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#getConnectUrl");
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
| **platform** | **String**| Social media platform to connect | [enum: facebook, instagram, linkedin, twitter, tiktok, youtube, threads, reddit, pinterest, bluesky, googlebusiness, telegram, snapchat] |
| **profileId** | **String**| Your Late profile ID (get from /v1/profiles) | |
| **redirectUrl** | **URI**| Your custom redirect URL after connection completes.  **Standard Mode:** After the user selects an account, Late redirects here with &#x60;?connected&#x3D;{platform}&amp;profileId&#x3D;X&amp;username&#x3D;Y&#x60;.  **Headless Mode:** Pass &#x60;headless&#x3D;true&#x60; as a query parameter on this endpoint. After OAuth, the user is redirected to your URL with OAuth data (&#x60;profileId&#x60;, &#x60;tempToken&#x60;, &#x60;userProfile&#x60;, &#x60;connect_token&#x60;, &#x60;platform&#x60;, &#x60;step&#x60;). See the main endpoint description for details.  Example: &#x60;https://yourdomain.com/integrations/callback&#x60;  | [optional] |

### Return type

ApiResponse<[**GetConnectUrl200Response**](GetConnectUrl200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OAuth authorization URL to redirect user to |  -  |
| **400** | Missing/invalid parameters (e.g., invalid profileId format) |  -  |
| **401** | Unauthorized |  -  |
| **403** | No access to profile, or BYOK required for AppSumo Twitter |  -  |
| **404** | Profile not found |  -  |


## getFacebookPages

> GetFacebookPages200Response getFacebookPages(accountId)

List Facebook pages

Returns all Facebook pages the connected account has access to, including the currently selected page.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        try {
            GetFacebookPages200Response result = apiInstance.getFacebookPages(accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#getFacebookPages");
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
| **accountId** | **String**|  | |

### Return type

[**GetFacebookPages200Response**](GetFacebookPages200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Pages list |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## getFacebookPagesWithHttpInfo

> ApiResponse<GetFacebookPages200Response> getFacebookPages getFacebookPagesWithHttpInfo(accountId)

List Facebook pages

Returns all Facebook pages the connected account has access to, including the currently selected page.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        try {
            ApiResponse<GetFacebookPages200Response> response = apiInstance.getFacebookPagesWithHttpInfo(accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#getFacebookPages");
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
| **accountId** | **String**|  | |

### Return type

ApiResponse<[**GetFacebookPages200Response**](GetFacebookPages200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Pages list |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |


## getGmbLocations

> GetGmbLocations200Response getGmbLocations(accountId)

List Google Business locations

Returns all Google Business Profile locations the connected account has access to, including the currently selected location.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        try {
            GetGmbLocations200Response result = apiInstance.getGmbLocations(accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#getGmbLocations");
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
| **accountId** | **String**|  | |

### Return type

[**GetGmbLocations200Response**](GetGmbLocations200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Locations list |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## getGmbLocationsWithHttpInfo

> ApiResponse<GetGmbLocations200Response> getGmbLocations getGmbLocationsWithHttpInfo(accountId)

List Google Business locations

Returns all Google Business Profile locations the connected account has access to, including the currently selected location.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        try {
            ApiResponse<GetGmbLocations200Response> response = apiInstance.getGmbLocationsWithHttpInfo(accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#getGmbLocations");
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
| **accountId** | **String**|  | |

### Return type

ApiResponse<[**GetGmbLocations200Response**](GetGmbLocations200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Locations list |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |


## getLinkedInOrganizations

> GetLinkedInOrganizations200Response getLinkedInOrganizations(accountId)

List LinkedIn orgs

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        try {
            GetLinkedInOrganizations200Response result = apiInstance.getLinkedInOrganizations(accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#getLinkedInOrganizations");
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
| **accountId** | **String**|  | |

### Return type

[**GetLinkedInOrganizations200Response**](GetLinkedInOrganizations200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Organizations list |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## getLinkedInOrganizationsWithHttpInfo

> ApiResponse<GetLinkedInOrganizations200Response> getLinkedInOrganizations getLinkedInOrganizationsWithHttpInfo(accountId)

List LinkedIn orgs

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        try {
            ApiResponse<GetLinkedInOrganizations200Response> response = apiInstance.getLinkedInOrganizationsWithHttpInfo(accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#getLinkedInOrganizations");
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
| **accountId** | **String**|  | |

### Return type

ApiResponse<[**GetLinkedInOrganizations200Response**](GetLinkedInOrganizations200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Organizations list |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |


## getPendingOAuthData

> GetPendingOAuthData200Response getPendingOAuthData(token)

Get pending OAuth data

**Fetch Pending OAuth Data for Headless Mode**  In headless mode, platforms like LinkedIn store OAuth selection data (organizations, pages, etc.) in the database instead of passing it via URL parameters. This prevents URI_TOO_LONG errors when users have many organizations/pages to select from.  After OAuth redirect, use the &#x60;pendingDataToken&#x60; from the URL to fetch the stored data.  **Important:** - This endpoint is one-time use: data is deleted after being fetched - Data expires automatically after 10 minutes if not fetched - No authentication required, just the token from the redirect URL 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String token = "token_example"; // String | The pending data token from the OAuth redirect URL (`pendingDataToken` parameter)
        try {
            GetPendingOAuthData200Response result = apiInstance.getPendingOAuthData(token);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#getPendingOAuthData");
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
| **token** | **String**| The pending data token from the OAuth redirect URL (&#x60;pendingDataToken&#x60; parameter) | |

### Return type

[**GetPendingOAuthData200Response**](GetPendingOAuthData200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OAuth data fetched successfully |  -  |
| **400** | Missing token parameter |  -  |
| **404** | Token not found or expired |  -  |

## getPendingOAuthDataWithHttpInfo

> ApiResponse<GetPendingOAuthData200Response> getPendingOAuthData getPendingOAuthDataWithHttpInfo(token)

Get pending OAuth data

**Fetch Pending OAuth Data for Headless Mode**  In headless mode, platforms like LinkedIn store OAuth selection data (organizations, pages, etc.) in the database instead of passing it via URL parameters. This prevents URI_TOO_LONG errors when users have many organizations/pages to select from.  After OAuth redirect, use the &#x60;pendingDataToken&#x60; from the URL to fetch the stored data.  **Important:** - This endpoint is one-time use: data is deleted after being fetched - Data expires automatically after 10 minutes if not fetched - No authentication required, just the token from the redirect URL 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String token = "token_example"; // String | The pending data token from the OAuth redirect URL (`pendingDataToken` parameter)
        try {
            ApiResponse<GetPendingOAuthData200Response> response = apiInstance.getPendingOAuthDataWithHttpInfo(token);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#getPendingOAuthData");
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
| **token** | **String**| The pending data token from the OAuth redirect URL (&#x60;pendingDataToken&#x60; parameter) | |

### Return type

ApiResponse<[**GetPendingOAuthData200Response**](GetPendingOAuthData200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OAuth data fetched successfully |  -  |
| **400** | Missing token parameter |  -  |
| **404** | Token not found or expired |  -  |


## getPinterestBoards

> GetPinterestBoards200Response getPinterestBoards(accountId)

List Pinterest boards

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        try {
            GetPinterestBoards200Response result = apiInstance.getPinterestBoards(accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#getPinterestBoards");
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
| **accountId** | **String**|  | |

### Return type

[**GetPinterestBoards200Response**](GetPinterestBoards200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Boards list |  -  |
| **400** | Not a Pinterest account |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## getPinterestBoardsWithHttpInfo

> ApiResponse<GetPinterestBoards200Response> getPinterestBoards getPinterestBoardsWithHttpInfo(accountId)

List Pinterest boards

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        try {
            ApiResponse<GetPinterestBoards200Response> response = apiInstance.getPinterestBoardsWithHttpInfo(accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#getPinterestBoards");
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
| **accountId** | **String**|  | |

### Return type

ApiResponse<[**GetPinterestBoards200Response**](GetPinterestBoards200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Boards list |  -  |
| **400** | Not a Pinterest account |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |


## getRedditFlairs

> GetRedditFlairs200Response getRedditFlairs(accountId, subreddit)

List subreddit flairs

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        String subreddit = "subreddit_example"; // String | Subreddit name (without \"r/\" prefix) to fetch flairs for
        try {
            GetRedditFlairs200Response result = apiInstance.getRedditFlairs(accountId, subreddit);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#getRedditFlairs");
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
| **accountId** | **String**|  | |
| **subreddit** | **String**| Subreddit name (without \&quot;r/\&quot; prefix) to fetch flairs for | |

### Return type

[**GetRedditFlairs200Response**](GetRedditFlairs200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Flairs list |  -  |
| **400** | Not a Reddit account or missing subreddit parameter |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## getRedditFlairsWithHttpInfo

> ApiResponse<GetRedditFlairs200Response> getRedditFlairs getRedditFlairsWithHttpInfo(accountId, subreddit)

List subreddit flairs

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        String subreddit = "subreddit_example"; // String | Subreddit name (without \"r/\" prefix) to fetch flairs for
        try {
            ApiResponse<GetRedditFlairs200Response> response = apiInstance.getRedditFlairsWithHttpInfo(accountId, subreddit);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#getRedditFlairs");
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
| **accountId** | **String**|  | |
| **subreddit** | **String**| Subreddit name (without \&quot;r/\&quot; prefix) to fetch flairs for | |

### Return type

ApiResponse<[**GetRedditFlairs200Response**](GetRedditFlairs200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Flairs list |  -  |
| **400** | Not a Reddit account or missing subreddit parameter |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |


## getRedditSubreddits

> GetRedditSubreddits200Response getRedditSubreddits(accountId)

List Reddit subreddits

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        try {
            GetRedditSubreddits200Response result = apiInstance.getRedditSubreddits(accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#getRedditSubreddits");
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
| **accountId** | **String**|  | |

### Return type

[**GetRedditSubreddits200Response**](GetRedditSubreddits200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Subreddits list |  -  |
| **400** | Not a Reddit account |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## getRedditSubredditsWithHttpInfo

> ApiResponse<GetRedditSubreddits200Response> getRedditSubreddits getRedditSubredditsWithHttpInfo(accountId)

List Reddit subreddits

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        try {
            ApiResponse<GetRedditSubreddits200Response> response = apiInstance.getRedditSubredditsWithHttpInfo(accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#getRedditSubreddits");
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
| **accountId** | **String**|  | |

### Return type

ApiResponse<[**GetRedditSubreddits200Response**](GetRedditSubreddits200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Subreddits list |  -  |
| **400** | Not a Reddit account |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |


## getTelegramConnectStatus

> GetTelegramConnectStatus200Response getTelegramConnectStatus(profileId)

Generate Telegram code

Generate a unique access code for connecting a Telegram channel or group.  **Connection Flow:** 1. Call this endpoint to get an access code (valid for 15 minutes) 2. Add the bot (@LateScheduleBot or your configured bot) as an administrator in your Telegram channel/group 3. Open a private chat with the bot 4. Send: &#x60;{CODE} @yourchannel&#x60; (e.g., &#x60;LATE-ABC123 @mychannel&#x60;) 5. Poll &#x60;PATCH /v1/connect/telegram?code&#x3D;{CODE}&#x60; to check connection status  **Alternative for private channels:** If your channel has no public username, forward any message from the channel to the bot along with the access code. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String profileId = "profileId_example"; // String | The profile ID to connect the Telegram account to
        try {
            GetTelegramConnectStatus200Response result = apiInstance.getTelegramConnectStatus(profileId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#getTelegramConnectStatus");
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
| **profileId** | **String**| The profile ID to connect the Telegram account to | |

### Return type

[**GetTelegramConnectStatus200Response**](GetTelegramConnectStatus200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Access code generated |  -  |
| **400** | Profile ID required or invalid format |  -  |
| **401** | Unauthorized |  -  |
| **403** | No access to this profile |  -  |
| **404** | Profile not found |  -  |
| **500** | Internal error |  -  |

## getTelegramConnectStatusWithHttpInfo

> ApiResponse<GetTelegramConnectStatus200Response> getTelegramConnectStatus getTelegramConnectStatusWithHttpInfo(profileId)

Generate Telegram code

Generate a unique access code for connecting a Telegram channel or group.  **Connection Flow:** 1. Call this endpoint to get an access code (valid for 15 minutes) 2. Add the bot (@LateScheduleBot or your configured bot) as an administrator in your Telegram channel/group 3. Open a private chat with the bot 4. Send: &#x60;{CODE} @yourchannel&#x60; (e.g., &#x60;LATE-ABC123 @mychannel&#x60;) 5. Poll &#x60;PATCH /v1/connect/telegram?code&#x3D;{CODE}&#x60; to check connection status  **Alternative for private channels:** If your channel has no public username, forward any message from the channel to the bot along with the access code. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String profileId = "profileId_example"; // String | The profile ID to connect the Telegram account to
        try {
            ApiResponse<GetTelegramConnectStatus200Response> response = apiInstance.getTelegramConnectStatusWithHttpInfo(profileId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#getTelegramConnectStatus");
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
| **profileId** | **String**| The profile ID to connect the Telegram account to | |

### Return type

ApiResponse<[**GetTelegramConnectStatus200Response**](GetTelegramConnectStatus200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Access code generated |  -  |
| **400** | Profile ID required or invalid format |  -  |
| **401** | Unauthorized |  -  |
| **403** | No access to this profile |  -  |
| **404** | Profile not found |  -  |
| **500** | Internal error |  -  |


## handleOAuthCallback

> void handleOAuthCallback(platform, handleOAuthCallbackRequest)

Complete OAuth callback

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String platform = "platform_example"; // String | 
        HandleOAuthCallbackRequest handleOAuthCallbackRequest = new HandleOAuthCallbackRequest(); // HandleOAuthCallbackRequest | 
        try {
            apiInstance.handleOAuthCallback(platform, handleOAuthCallbackRequest);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#handleOAuthCallback");
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
| **platform** | **String**|  | |
| **handleOAuthCallbackRequest** | [**HandleOAuthCallbackRequest**](HandleOAuthCallbackRequest.md)|  | |

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
| **200** | Account connected |  -  |
| **400** | Invalid params |  -  |
| **401** | Unauthorized |  -  |
| **403** | BYOK required for AppSumo Twitter |  -  |
| **500** | Failed to connect account |  -  |

## handleOAuthCallbackWithHttpInfo

> ApiResponse<Void> handleOAuthCallback handleOAuthCallbackWithHttpInfo(platform, handleOAuthCallbackRequest)

Complete OAuth callback

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String platform = "platform_example"; // String | 
        HandleOAuthCallbackRequest handleOAuthCallbackRequest = new HandleOAuthCallbackRequest(); // HandleOAuthCallbackRequest | 
        try {
            ApiResponse<Void> response = apiInstance.handleOAuthCallbackWithHttpInfo(platform, handleOAuthCallbackRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#handleOAuthCallback");
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
| **platform** | **String**|  | |
| **handleOAuthCallbackRequest** | [**HandleOAuthCallbackRequest**](HandleOAuthCallbackRequest.md)|  | |

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
| **200** | Account connected |  -  |
| **400** | Invalid params |  -  |
| **401** | Unauthorized |  -  |
| **403** | BYOK required for AppSumo Twitter |  -  |
| **500** | Failed to connect account |  -  |


## initiateTelegramConnect

> InitiateTelegramConnect200Response initiateTelegramConnect(initiateTelegramConnectRequest)

Connect Telegram directly

Connect a Telegram channel/group directly using the chat ID.  This is an alternative to the access code flow for power users who know their Telegram chat ID. The bot must already be added as an administrator in the channel/group. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        InitiateTelegramConnectRequest initiateTelegramConnectRequest = new InitiateTelegramConnectRequest(); // InitiateTelegramConnectRequest | 
        try {
            InitiateTelegramConnect200Response result = apiInstance.initiateTelegramConnect(initiateTelegramConnectRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#initiateTelegramConnect");
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
| **initiateTelegramConnectRequest** | [**InitiateTelegramConnectRequest**](InitiateTelegramConnectRequest.md)|  | |

### Return type

[**InitiateTelegramConnect200Response**](InitiateTelegramConnect200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Telegram channel connected successfully |  -  |
| **400** | Chat ID required |  -  |
| **401** | Unauthorized |  -  |
| **403** | No access to this profile |  -  |
| **404** | Profile not found |  -  |
| **500** | Internal error |  -  |

## initiateTelegramConnectWithHttpInfo

> ApiResponse<InitiateTelegramConnect200Response> initiateTelegramConnect initiateTelegramConnectWithHttpInfo(initiateTelegramConnectRequest)

Connect Telegram directly

Connect a Telegram channel/group directly using the chat ID.  This is an alternative to the access code flow for power users who know their Telegram chat ID. The bot must already be added as an administrator in the channel/group. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        InitiateTelegramConnectRequest initiateTelegramConnectRequest = new InitiateTelegramConnectRequest(); // InitiateTelegramConnectRequest | 
        try {
            ApiResponse<InitiateTelegramConnect200Response> response = apiInstance.initiateTelegramConnectWithHttpInfo(initiateTelegramConnectRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#initiateTelegramConnect");
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
| **initiateTelegramConnectRequest** | [**InitiateTelegramConnectRequest**](InitiateTelegramConnectRequest.md)|  | |

### Return type

ApiResponse<[**InitiateTelegramConnect200Response**](InitiateTelegramConnect200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Telegram channel connected successfully |  -  |
| **400** | Chat ID required |  -  |
| **401** | Unauthorized |  -  |
| **403** | No access to this profile |  -  |
| **404** | Profile not found |  -  |
| **500** | Internal error |  -  |


## listFacebookPages

> ListFacebookPages200Response listFacebookPages(profileId, tempToken)

List Facebook pages

**Headless Mode for Custom UI**  After initiating Facebook OAuth via &#x60;/v1/connect/facebook&#x60;, you&#39;ll be redirected to  &#x60;/connect/facebook/select-page&#x60; with query params including &#x60;tempToken&#x60; and &#x60;userProfile&#x60;.  For a **headless/whitelabeled flow**, extract these params from the URL and call this  endpoint to retrieve the list of Facebook Pages the user can manage. Then build your  own UI to let users select a page.  **Note:** Use the &#x60;X-Connect-Token&#x60; header if you initiated the connection via API key  (rather than a browser session). 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure API key authorization: connectToken
        ApiKeyAuth connectToken = (ApiKeyAuth) defaultClient.getAuthentication("connectToken");
        connectToken.setApiKey("YOUR API KEY");
        // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
        //connectToken.setApiKeyPrefix("Token");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String profileId = "profileId_example"; // String | Profile ID from your connection flow
        String tempToken = "tempToken_example"; // String | Temporary Facebook access token from the OAuth callback redirect
        try {
            ListFacebookPages200Response result = apiInstance.listFacebookPages(profileId, tempToken);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#listFacebookPages");
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
| **profileId** | **String**| Profile ID from your connection flow | |
| **tempToken** | **String**| Temporary Facebook access token from the OAuth callback redirect | |

### Return type

[**ListFacebookPages200Response**](ListFacebookPages200Response.md)


### Authorization

[connectToken](../README.md#connectToken), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of Facebook Pages available for connection |  -  |
| **400** | Missing required parameters (profileId or tempToken) |  -  |
| **401** | Unauthorized |  -  |
| **500** | Failed to fetch pages (e.g., invalid token, insufficient permissions) |  -  |

## listFacebookPagesWithHttpInfo

> ApiResponse<ListFacebookPages200Response> listFacebookPages listFacebookPagesWithHttpInfo(profileId, tempToken)

List Facebook pages

**Headless Mode for Custom UI**  After initiating Facebook OAuth via &#x60;/v1/connect/facebook&#x60;, you&#39;ll be redirected to  &#x60;/connect/facebook/select-page&#x60; with query params including &#x60;tempToken&#x60; and &#x60;userProfile&#x60;.  For a **headless/whitelabeled flow**, extract these params from the URL and call this  endpoint to retrieve the list of Facebook Pages the user can manage. Then build your  own UI to let users select a page.  **Note:** Use the &#x60;X-Connect-Token&#x60; header if you initiated the connection via API key  (rather than a browser session). 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure API key authorization: connectToken
        ApiKeyAuth connectToken = (ApiKeyAuth) defaultClient.getAuthentication("connectToken");
        connectToken.setApiKey("YOUR API KEY");
        // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
        //connectToken.setApiKeyPrefix("Token");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String profileId = "profileId_example"; // String | Profile ID from your connection flow
        String tempToken = "tempToken_example"; // String | Temporary Facebook access token from the OAuth callback redirect
        try {
            ApiResponse<ListFacebookPages200Response> response = apiInstance.listFacebookPagesWithHttpInfo(profileId, tempToken);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#listFacebookPages");
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
| **profileId** | **String**| Profile ID from your connection flow | |
| **tempToken** | **String**| Temporary Facebook access token from the OAuth callback redirect | |

### Return type

ApiResponse<[**ListFacebookPages200Response**](ListFacebookPages200Response.md)>


### Authorization

[connectToken](../README.md#connectToken), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of Facebook Pages available for connection |  -  |
| **400** | Missing required parameters (profileId or tempToken) |  -  |
| **401** | Unauthorized |  -  |
| **500** | Failed to fetch pages (e.g., invalid token, insufficient permissions) |  -  |


## listGoogleBusinessLocations

> ListGoogleBusinessLocations200Response listGoogleBusinessLocations(profileId, tempToken)

List Google Business locations

**Headless Mode for Custom UI**  After initiating Google Business OAuth via &#x60;/v1/connect/googlebusiness?headless&#x3D;true&#x60;, you&#39;ll be redirected  to your &#x60;redirect_url&#x60; with query params including &#x60;tempToken&#x60; and &#x60;userProfile&#x60;.  For a **headless/whitelabeled flow**, extract these params from the URL and call this  endpoint to retrieve the list of Google Business locations the user can manage. Then build your  own UI to let users select a location.  **Note:** Use the &#x60;X-Connect-Token&#x60; header if you initiated the connection via API key  (rather than a browser session). 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure API key authorization: connectToken
        ApiKeyAuth connectToken = (ApiKeyAuth) defaultClient.getAuthentication("connectToken");
        connectToken.setApiKey("YOUR API KEY");
        // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
        //connectToken.setApiKeyPrefix("Token");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String profileId = "profileId_example"; // String | Profile ID from your connection flow
        String tempToken = "tempToken_example"; // String | Temporary Google access token from the OAuth callback redirect
        try {
            ListGoogleBusinessLocations200Response result = apiInstance.listGoogleBusinessLocations(profileId, tempToken);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#listGoogleBusinessLocations");
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
| **profileId** | **String**| Profile ID from your connection flow | |
| **tempToken** | **String**| Temporary Google access token from the OAuth callback redirect | |

### Return type

[**ListGoogleBusinessLocations200Response**](ListGoogleBusinessLocations200Response.md)


### Authorization

[connectToken](../README.md#connectToken), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of Google Business locations available for connection |  -  |
| **400** | Missing required parameters (profileId or tempToken) |  -  |
| **401** | Unauthorized |  -  |
| **500** | Failed to fetch locations (e.g., invalid token, insufficient permissions) |  -  |

## listGoogleBusinessLocationsWithHttpInfo

> ApiResponse<ListGoogleBusinessLocations200Response> listGoogleBusinessLocations listGoogleBusinessLocationsWithHttpInfo(profileId, tempToken)

List Google Business locations

**Headless Mode for Custom UI**  After initiating Google Business OAuth via &#x60;/v1/connect/googlebusiness?headless&#x3D;true&#x60;, you&#39;ll be redirected  to your &#x60;redirect_url&#x60; with query params including &#x60;tempToken&#x60; and &#x60;userProfile&#x60;.  For a **headless/whitelabeled flow**, extract these params from the URL and call this  endpoint to retrieve the list of Google Business locations the user can manage. Then build your  own UI to let users select a location.  **Note:** Use the &#x60;X-Connect-Token&#x60; header if you initiated the connection via API key  (rather than a browser session). 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure API key authorization: connectToken
        ApiKeyAuth connectToken = (ApiKeyAuth) defaultClient.getAuthentication("connectToken");
        connectToken.setApiKey("YOUR API KEY");
        // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
        //connectToken.setApiKeyPrefix("Token");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String profileId = "profileId_example"; // String | Profile ID from your connection flow
        String tempToken = "tempToken_example"; // String | Temporary Google access token from the OAuth callback redirect
        try {
            ApiResponse<ListGoogleBusinessLocations200Response> response = apiInstance.listGoogleBusinessLocationsWithHttpInfo(profileId, tempToken);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#listGoogleBusinessLocations");
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
| **profileId** | **String**| Profile ID from your connection flow | |
| **tempToken** | **String**| Temporary Google access token from the OAuth callback redirect | |

### Return type

ApiResponse<[**ListGoogleBusinessLocations200Response**](ListGoogleBusinessLocations200Response.md)>


### Authorization

[connectToken](../README.md#connectToken), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of Google Business locations available for connection |  -  |
| **400** | Missing required parameters (profileId or tempToken) |  -  |
| **401** | Unauthorized |  -  |
| **500** | Failed to fetch locations (e.g., invalid token, insufficient permissions) |  -  |


## listLinkedInOrganizations

> ListLinkedInOrganizations200Response listLinkedInOrganizations(tempToken, orgIds)

List LinkedIn orgs

**Fetch Full Organization Details for Custom UI**  After LinkedIn OAuth in headless mode, the redirect URL contains organization data with only &#x60;id&#x60;, &#x60;urn&#x60;, and &#x60;name&#x60; fields (additional details are excluded to prevent URL length issues with many organizations).  Use this endpoint to fetch full organization details including logos, vanity names, websites, and more if you want to display them in your custom selection UI.  **Note:** This endpoint requires no authentication - just the &#x60;tempToken&#x60; from the OAuth redirect. Details are fetched directly from LinkedIn&#39;s API in parallel for fast response times. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String tempToken = "tempToken_example"; // String | The temporary LinkedIn access token from the OAuth redirect
        String orgIds = "12345678,87654321,11111111"; // String | Comma-separated list of organization IDs to fetch details for (max 100)
        try {
            ListLinkedInOrganizations200Response result = apiInstance.listLinkedInOrganizations(tempToken, orgIds);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#listLinkedInOrganizations");
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
| **tempToken** | **String**| The temporary LinkedIn access token from the OAuth redirect | |
| **orgIds** | **String**| Comma-separated list of organization IDs to fetch details for (max 100) | |

### Return type

[**ListLinkedInOrganizations200Response**](ListLinkedInOrganizations200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Organization details fetched successfully |  -  |
| **400** | Missing required parameters or too many organization IDs |  -  |
| **500** | Failed to fetch organization details |  -  |

## listLinkedInOrganizationsWithHttpInfo

> ApiResponse<ListLinkedInOrganizations200Response> listLinkedInOrganizations listLinkedInOrganizationsWithHttpInfo(tempToken, orgIds)

List LinkedIn orgs

**Fetch Full Organization Details for Custom UI**  After LinkedIn OAuth in headless mode, the redirect URL contains organization data with only &#x60;id&#x60;, &#x60;urn&#x60;, and &#x60;name&#x60; fields (additional details are excluded to prevent URL length issues with many organizations).  Use this endpoint to fetch full organization details including logos, vanity names, websites, and more if you want to display them in your custom selection UI.  **Note:** This endpoint requires no authentication - just the &#x60;tempToken&#x60; from the OAuth redirect. Details are fetched directly from LinkedIn&#39;s API in parallel for fast response times. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String tempToken = "tempToken_example"; // String | The temporary LinkedIn access token from the OAuth redirect
        String orgIds = "12345678,87654321,11111111"; // String | Comma-separated list of organization IDs to fetch details for (max 100)
        try {
            ApiResponse<ListLinkedInOrganizations200Response> response = apiInstance.listLinkedInOrganizationsWithHttpInfo(tempToken, orgIds);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#listLinkedInOrganizations");
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
| **tempToken** | **String**| The temporary LinkedIn access token from the OAuth redirect | |
| **orgIds** | **String**| Comma-separated list of organization IDs to fetch details for (max 100) | |

### Return type

ApiResponse<[**ListLinkedInOrganizations200Response**](ListLinkedInOrganizations200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Organization details fetched successfully |  -  |
| **400** | Missing required parameters or too many organization IDs |  -  |
| **500** | Failed to fetch organization details |  -  |


## listPinterestBoardsForSelection

> ListPinterestBoardsForSelection200Response listPinterestBoardsForSelection(xConnectToken, profileId, tempToken)

List Pinterest boards

**Retrieve Pinterest Boards for Selection UI**  After initiating Pinterest OAuth via &#x60;/v1/connect/pinterest&#x60; with &#x60;headless&#x3D;true&#x60;, you&#39;ll be redirected to your &#x60;redirect_url&#x60; with query params including &#x60;tempToken&#x60; and &#x60;userProfile&#x60;.  If you want to build your own fully-branded board selector (instead of Late&#39;s hosted UI), call this endpoint to retrieve the list of Pinterest Boards the user can post to. Then build your UI and call &#x60;POST /v1/connect/pinterest/select-board&#x60; to save the selection.  **Authentication:** Use &#x60;X-Connect-Token&#x60; header with the &#x60;connect_token&#x60; from the redirect URL. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String xConnectToken = "xConnectToken_example"; // String | Short-lived connect token from the OAuth redirect
        String profileId = "profileId_example"; // String | Your Late profile ID
        String tempToken = "tempToken_example"; // String | Temporary Pinterest access token from the OAuth callback redirect
        try {
            ListPinterestBoardsForSelection200Response result = apiInstance.listPinterestBoardsForSelection(xConnectToken, profileId, tempToken);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#listPinterestBoardsForSelection");
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
| **xConnectToken** | **String**| Short-lived connect token from the OAuth redirect | |
| **profileId** | **String**| Your Late profile ID | |
| **tempToken** | **String**| Temporary Pinterest access token from the OAuth callback redirect | |

### Return type

[**ListPinterestBoardsForSelection200Response**](ListPinterestBoardsForSelection200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of Pinterest Boards available for connection |  -  |
| **400** | Missing required parameters |  -  |
| **401** | Unauthorized |  -  |
| **403** | No access to profile |  -  |
| **500** | Failed to fetch boards |  -  |

## listPinterestBoardsForSelectionWithHttpInfo

> ApiResponse<ListPinterestBoardsForSelection200Response> listPinterestBoardsForSelection listPinterestBoardsForSelectionWithHttpInfo(xConnectToken, profileId, tempToken)

List Pinterest boards

**Retrieve Pinterest Boards for Selection UI**  After initiating Pinterest OAuth via &#x60;/v1/connect/pinterest&#x60; with &#x60;headless&#x3D;true&#x60;, you&#39;ll be redirected to your &#x60;redirect_url&#x60; with query params including &#x60;tempToken&#x60; and &#x60;userProfile&#x60;.  If you want to build your own fully-branded board selector (instead of Late&#39;s hosted UI), call this endpoint to retrieve the list of Pinterest Boards the user can post to. Then build your UI and call &#x60;POST /v1/connect/pinterest/select-board&#x60; to save the selection.  **Authentication:** Use &#x60;X-Connect-Token&#x60; header with the &#x60;connect_token&#x60; from the redirect URL. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String xConnectToken = "xConnectToken_example"; // String | Short-lived connect token from the OAuth redirect
        String profileId = "profileId_example"; // String | Your Late profile ID
        String tempToken = "tempToken_example"; // String | Temporary Pinterest access token from the OAuth callback redirect
        try {
            ApiResponse<ListPinterestBoardsForSelection200Response> response = apiInstance.listPinterestBoardsForSelectionWithHttpInfo(xConnectToken, profileId, tempToken);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#listPinterestBoardsForSelection");
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
| **xConnectToken** | **String**| Short-lived connect token from the OAuth redirect | |
| **profileId** | **String**| Your Late profile ID | |
| **tempToken** | **String**| Temporary Pinterest access token from the OAuth callback redirect | |

### Return type

ApiResponse<[**ListPinterestBoardsForSelection200Response**](ListPinterestBoardsForSelection200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of Pinterest Boards available for connection |  -  |
| **400** | Missing required parameters |  -  |
| **401** | Unauthorized |  -  |
| **403** | No access to profile |  -  |
| **500** | Failed to fetch boards |  -  |


## listSnapchatProfiles

> ListSnapchatProfiles200Response listSnapchatProfiles(xConnectToken, profileId, tempToken)

List Snapchat profiles

**Headless Mode for Custom UI**  After initiating Snapchat OAuth via &#x60;/v1/connect/snapchat?headless&#x3D;true&#x60;, you&#39;ll be redirected to your &#x60;redirect_url&#x60; with query params including &#x60;tempToken&#x60;, &#x60;userProfile&#x60;, and &#x60;publicProfiles&#x60;.  If you want to build your own fully-branded profile selector (instead of Late&#39;s hosted UI), call this endpoint to retrieve the list of Snapchat Public Profiles the user can post to. Then build your UI and call &#x60;POST /v1/connect/snapchat/select-profile&#x60; to save the selection.  **Authentication:** Use &#x60;X-Connect-Token&#x60; header with the &#x60;connect_token&#x60; from the redirect URL. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String xConnectToken = "xConnectToken_example"; // String | Short-lived connect token from the OAuth redirect
        String profileId = "profileId_example"; // String | Your Late profile ID
        String tempToken = "tempToken_example"; // String | Temporary Snapchat access token from the OAuth callback redirect
        try {
            ListSnapchatProfiles200Response result = apiInstance.listSnapchatProfiles(xConnectToken, profileId, tempToken);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#listSnapchatProfiles");
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
| **xConnectToken** | **String**| Short-lived connect token from the OAuth redirect | |
| **profileId** | **String**| Your Late profile ID | |
| **tempToken** | **String**| Temporary Snapchat access token from the OAuth callback redirect | |

### Return type

[**ListSnapchatProfiles200Response**](ListSnapchatProfiles200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of Snapchat Public Profiles available for connection |  -  |
| **400** | Missing required parameters (profileId or tempToken) |  -  |
| **401** | Unauthorized |  -  |
| **403** | No access to profile |  -  |
| **500** | Failed to fetch public profiles |  -  |

## listSnapchatProfilesWithHttpInfo

> ApiResponse<ListSnapchatProfiles200Response> listSnapchatProfiles listSnapchatProfilesWithHttpInfo(xConnectToken, profileId, tempToken)

List Snapchat profiles

**Headless Mode for Custom UI**  After initiating Snapchat OAuth via &#x60;/v1/connect/snapchat?headless&#x3D;true&#x60;, you&#39;ll be redirected to your &#x60;redirect_url&#x60; with query params including &#x60;tempToken&#x60;, &#x60;userProfile&#x60;, and &#x60;publicProfiles&#x60;.  If you want to build your own fully-branded profile selector (instead of Late&#39;s hosted UI), call this endpoint to retrieve the list of Snapchat Public Profiles the user can post to. Then build your UI and call &#x60;POST /v1/connect/snapchat/select-profile&#x60; to save the selection.  **Authentication:** Use &#x60;X-Connect-Token&#x60; header with the &#x60;connect_token&#x60; from the redirect URL. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String xConnectToken = "xConnectToken_example"; // String | Short-lived connect token from the OAuth redirect
        String profileId = "profileId_example"; // String | Your Late profile ID
        String tempToken = "tempToken_example"; // String | Temporary Snapchat access token from the OAuth callback redirect
        try {
            ApiResponse<ListSnapchatProfiles200Response> response = apiInstance.listSnapchatProfilesWithHttpInfo(xConnectToken, profileId, tempToken);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#listSnapchatProfiles");
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
| **xConnectToken** | **String**| Short-lived connect token from the OAuth redirect | |
| **profileId** | **String**| Your Late profile ID | |
| **tempToken** | **String**| Temporary Snapchat access token from the OAuth callback redirect | |

### Return type

ApiResponse<[**ListSnapchatProfiles200Response**](ListSnapchatProfiles200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of Snapchat Public Profiles available for connection |  -  |
| **400** | Missing required parameters (profileId or tempToken) |  -  |
| **401** | Unauthorized |  -  |
| **403** | No access to profile |  -  |
| **500** | Failed to fetch public profiles |  -  |


## selectFacebookPage

> SelectFacebookPage200Response selectFacebookPage(selectFacebookPageRequest)

Select Facebook page

**Complete the Headless Flow**  After displaying your custom UI with the list of pages from the GET endpoint, call this  endpoint to finalize the connection with the user&#39;s selected page.  The &#x60;userProfile&#x60; should be the decoded JSON object from the &#x60;userProfile&#x60; query param  in the OAuth callback redirect URL.  **Note:** Use the &#x60;X-Connect-Token&#x60; header if you initiated the connection via API key. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure API key authorization: connectToken
        ApiKeyAuth connectToken = (ApiKeyAuth) defaultClient.getAuthentication("connectToken");
        connectToken.setApiKey("YOUR API KEY");
        // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
        //connectToken.setApiKeyPrefix("Token");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        SelectFacebookPageRequest selectFacebookPageRequest = new SelectFacebookPageRequest(); // SelectFacebookPageRequest | 
        try {
            SelectFacebookPage200Response result = apiInstance.selectFacebookPage(selectFacebookPageRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#selectFacebookPage");
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
| **selectFacebookPageRequest** | [**SelectFacebookPageRequest**](SelectFacebookPageRequest.md)|  | |

### Return type

[**SelectFacebookPage200Response**](SelectFacebookPage200Response.md)


### Authorization

[connectToken](../README.md#connectToken), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Facebook Page connected successfully |  -  |
| **400** | Missing required fields (profileId, pageId, or tempToken) |  -  |
| **401** | Unauthorized |  -  |
| **403** | User does not have access to the specified profile |  -  |
| **404** | Selected page not found in available pages |  -  |
| **500** | Failed to save Facebook connection |  -  |

## selectFacebookPageWithHttpInfo

> ApiResponse<SelectFacebookPage200Response> selectFacebookPage selectFacebookPageWithHttpInfo(selectFacebookPageRequest)

Select Facebook page

**Complete the Headless Flow**  After displaying your custom UI with the list of pages from the GET endpoint, call this  endpoint to finalize the connection with the user&#39;s selected page.  The &#x60;userProfile&#x60; should be the decoded JSON object from the &#x60;userProfile&#x60; query param  in the OAuth callback redirect URL.  **Note:** Use the &#x60;X-Connect-Token&#x60; header if you initiated the connection via API key. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure API key authorization: connectToken
        ApiKeyAuth connectToken = (ApiKeyAuth) defaultClient.getAuthentication("connectToken");
        connectToken.setApiKey("YOUR API KEY");
        // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
        //connectToken.setApiKeyPrefix("Token");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        SelectFacebookPageRequest selectFacebookPageRequest = new SelectFacebookPageRequest(); // SelectFacebookPageRequest | 
        try {
            ApiResponse<SelectFacebookPage200Response> response = apiInstance.selectFacebookPageWithHttpInfo(selectFacebookPageRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#selectFacebookPage");
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
| **selectFacebookPageRequest** | [**SelectFacebookPageRequest**](SelectFacebookPageRequest.md)|  | |

### Return type

ApiResponse<[**SelectFacebookPage200Response**](SelectFacebookPage200Response.md)>


### Authorization

[connectToken](../README.md#connectToken), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Facebook Page connected successfully |  -  |
| **400** | Missing required fields (profileId, pageId, or tempToken) |  -  |
| **401** | Unauthorized |  -  |
| **403** | User does not have access to the specified profile |  -  |
| **404** | Selected page not found in available pages |  -  |
| **500** | Failed to save Facebook connection |  -  |


## selectGoogleBusinessLocation

> SelectGoogleBusinessLocation200Response selectGoogleBusinessLocation(selectGoogleBusinessLocationRequest)

Select Google Business location

**Complete the Headless Flow**  After displaying your custom UI with the list of locations from the GET &#x60;/v1/connect/googlebusiness/locations&#x60;  endpoint, call this endpoint to finalize the connection with the user&#39;s selected location.  The &#x60;userProfile&#x60; should be the decoded JSON object from the &#x60;userProfile&#x60; query param  in the OAuth callback redirect URL. It contains important token information (including refresh token).  **Note:** Use the &#x60;X-Connect-Token&#x60; header if you initiated the connection via API key. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure API key authorization: connectToken
        ApiKeyAuth connectToken = (ApiKeyAuth) defaultClient.getAuthentication("connectToken");
        connectToken.setApiKey("YOUR API KEY");
        // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
        //connectToken.setApiKeyPrefix("Token");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        SelectGoogleBusinessLocationRequest selectGoogleBusinessLocationRequest = new SelectGoogleBusinessLocationRequest(); // SelectGoogleBusinessLocationRequest | 
        try {
            SelectGoogleBusinessLocation200Response result = apiInstance.selectGoogleBusinessLocation(selectGoogleBusinessLocationRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#selectGoogleBusinessLocation");
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
| **selectGoogleBusinessLocationRequest** | [**SelectGoogleBusinessLocationRequest**](SelectGoogleBusinessLocationRequest.md)|  | |

### Return type

[**SelectGoogleBusinessLocation200Response**](SelectGoogleBusinessLocation200Response.md)


### Authorization

[connectToken](../README.md#connectToken), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Google Business location connected successfully |  -  |
| **400** | Missing required fields (profileId, locationId, or tempToken) |  -  |
| **401** | Unauthorized |  -  |
| **403** | User does not have access to the specified profile |  -  |
| **404** | Selected location not found in available locations |  -  |
| **500** | Failed to save Google Business connection |  -  |

## selectGoogleBusinessLocationWithHttpInfo

> ApiResponse<SelectGoogleBusinessLocation200Response> selectGoogleBusinessLocation selectGoogleBusinessLocationWithHttpInfo(selectGoogleBusinessLocationRequest)

Select Google Business location

**Complete the Headless Flow**  After displaying your custom UI with the list of locations from the GET &#x60;/v1/connect/googlebusiness/locations&#x60;  endpoint, call this endpoint to finalize the connection with the user&#39;s selected location.  The &#x60;userProfile&#x60; should be the decoded JSON object from the &#x60;userProfile&#x60; query param  in the OAuth callback redirect URL. It contains important token information (including refresh token).  **Note:** Use the &#x60;X-Connect-Token&#x60; header if you initiated the connection via API key. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure API key authorization: connectToken
        ApiKeyAuth connectToken = (ApiKeyAuth) defaultClient.getAuthentication("connectToken");
        connectToken.setApiKey("YOUR API KEY");
        // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
        //connectToken.setApiKeyPrefix("Token");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        SelectGoogleBusinessLocationRequest selectGoogleBusinessLocationRequest = new SelectGoogleBusinessLocationRequest(); // SelectGoogleBusinessLocationRequest | 
        try {
            ApiResponse<SelectGoogleBusinessLocation200Response> response = apiInstance.selectGoogleBusinessLocationWithHttpInfo(selectGoogleBusinessLocationRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#selectGoogleBusinessLocation");
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
| **selectGoogleBusinessLocationRequest** | [**SelectGoogleBusinessLocationRequest**](SelectGoogleBusinessLocationRequest.md)|  | |

### Return type

ApiResponse<[**SelectGoogleBusinessLocation200Response**](SelectGoogleBusinessLocation200Response.md)>


### Authorization

[connectToken](../README.md#connectToken), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Google Business location connected successfully |  -  |
| **400** | Missing required fields (profileId, locationId, or tempToken) |  -  |
| **401** | Unauthorized |  -  |
| **403** | User does not have access to the specified profile |  -  |
| **404** | Selected location not found in available locations |  -  |
| **500** | Failed to save Google Business connection |  -  |


## selectLinkedInOrganization

> SelectLinkedInOrganization200Response selectLinkedInOrganization(selectLinkedInOrganizationRequest)

Select LinkedIn org

**Complete the LinkedIn Connection Flow**  After OAuth, the user is redirected with &#x60;organizations&#x60; in the URL params (if they have org admin access). The organizations array contains &#x60;id&#x60;, &#x60;urn&#x60;, and &#x60;name&#x60; fields. Use this data to build your UI,  then call this endpoint to save the selection.  Set &#x60;accountType&#x60; to &#x60;personal&#x60; to connect as the user&#39;s personal LinkedIn profile, or &#x60;organization&#x60; to connect as a company page (requires &#x60;selectedOrganization&#x60; object).  **Personal Profile:** To connect a personal LinkedIn account, set &#x60;accountType&#x60; to &#x60;\&quot;personal\&quot;&#x60; and **omit** the &#x60;selectedOrganization&#x60; field entirely. This is the simplest flow.  **Headless Mode:** Use the &#x60;X-Connect-Token&#x60; header if you initiated the connection via API key. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        SelectLinkedInOrganizationRequest selectLinkedInOrganizationRequest = new SelectLinkedInOrganizationRequest(); // SelectLinkedInOrganizationRequest | 
        try {
            SelectLinkedInOrganization200Response result = apiInstance.selectLinkedInOrganization(selectLinkedInOrganizationRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#selectLinkedInOrganization");
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
| **selectLinkedInOrganizationRequest** | [**SelectLinkedInOrganizationRequest**](SelectLinkedInOrganizationRequest.md)|  | |

### Return type

[**SelectLinkedInOrganization200Response**](SelectLinkedInOrganization200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | LinkedIn account connected |  -  |
| **400** | Missing required fields |  -  |
| **401** | Unauthorized |  -  |
| **500** | Failed to connect LinkedIn account |  -  |

## selectLinkedInOrganizationWithHttpInfo

> ApiResponse<SelectLinkedInOrganization200Response> selectLinkedInOrganization selectLinkedInOrganizationWithHttpInfo(selectLinkedInOrganizationRequest)

Select LinkedIn org

**Complete the LinkedIn Connection Flow**  After OAuth, the user is redirected with &#x60;organizations&#x60; in the URL params (if they have org admin access). The organizations array contains &#x60;id&#x60;, &#x60;urn&#x60;, and &#x60;name&#x60; fields. Use this data to build your UI,  then call this endpoint to save the selection.  Set &#x60;accountType&#x60; to &#x60;personal&#x60; to connect as the user&#39;s personal LinkedIn profile, or &#x60;organization&#x60; to connect as a company page (requires &#x60;selectedOrganization&#x60; object).  **Personal Profile:** To connect a personal LinkedIn account, set &#x60;accountType&#x60; to &#x60;\&quot;personal\&quot;&#x60; and **omit** the &#x60;selectedOrganization&#x60; field entirely. This is the simplest flow.  **Headless Mode:** Use the &#x60;X-Connect-Token&#x60; header if you initiated the connection via API key. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        SelectLinkedInOrganizationRequest selectLinkedInOrganizationRequest = new SelectLinkedInOrganizationRequest(); // SelectLinkedInOrganizationRequest | 
        try {
            ApiResponse<SelectLinkedInOrganization200Response> response = apiInstance.selectLinkedInOrganizationWithHttpInfo(selectLinkedInOrganizationRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#selectLinkedInOrganization");
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
| **selectLinkedInOrganizationRequest** | [**SelectLinkedInOrganizationRequest**](SelectLinkedInOrganizationRequest.md)|  | |

### Return type

ApiResponse<[**SelectLinkedInOrganization200Response**](SelectLinkedInOrganization200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | LinkedIn account connected |  -  |
| **400** | Missing required fields |  -  |
| **401** | Unauthorized |  -  |
| **500** | Failed to connect LinkedIn account |  -  |


## selectPinterestBoard

> SelectPinterestBoard200Response selectPinterestBoard(selectPinterestBoardRequest)

Select Pinterest board

**Complete the Pinterest Connection Flow**  After OAuth, use this endpoint to save the selected board and complete the Pinterest account connection.  **Headless Mode:** Use the &#x60;X-Connect-Token&#x60; header if you initiated the connection via API key. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        SelectPinterestBoardRequest selectPinterestBoardRequest = new SelectPinterestBoardRequest(); // SelectPinterestBoardRequest | 
        try {
            SelectPinterestBoard200Response result = apiInstance.selectPinterestBoard(selectPinterestBoardRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#selectPinterestBoard");
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
| **selectPinterestBoardRequest** | [**SelectPinterestBoardRequest**](SelectPinterestBoardRequest.md)|  | |

### Return type

[**SelectPinterestBoard200Response**](SelectPinterestBoard200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Pinterest Board connected successfully |  -  |
| **400** | Missing required fields |  -  |
| **401** | Unauthorized |  -  |
| **403** | No access to profile or profile limit exceeded |  -  |
| **500** | Failed to save Pinterest connection |  -  |

## selectPinterestBoardWithHttpInfo

> ApiResponse<SelectPinterestBoard200Response> selectPinterestBoard selectPinterestBoardWithHttpInfo(selectPinterestBoardRequest)

Select Pinterest board

**Complete the Pinterest Connection Flow**  After OAuth, use this endpoint to save the selected board and complete the Pinterest account connection.  **Headless Mode:** Use the &#x60;X-Connect-Token&#x60; header if you initiated the connection via API key. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        SelectPinterestBoardRequest selectPinterestBoardRequest = new SelectPinterestBoardRequest(); // SelectPinterestBoardRequest | 
        try {
            ApiResponse<SelectPinterestBoard200Response> response = apiInstance.selectPinterestBoardWithHttpInfo(selectPinterestBoardRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#selectPinterestBoard");
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
| **selectPinterestBoardRequest** | [**SelectPinterestBoardRequest**](SelectPinterestBoardRequest.md)|  | |

### Return type

ApiResponse<[**SelectPinterestBoard200Response**](SelectPinterestBoard200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Pinterest Board connected successfully |  -  |
| **400** | Missing required fields |  -  |
| **401** | Unauthorized |  -  |
| **403** | No access to profile or profile limit exceeded |  -  |
| **500** | Failed to save Pinterest connection |  -  |


## selectSnapchatProfile

> SelectSnapchatProfile200Response selectSnapchatProfile(selectSnapchatProfileRequest, xConnectToken)

Select Snapchat profile

**Complete the Snapchat Connection Flow**  After OAuth, use this endpoint to save the selected Public Profile and complete the Snapchat account connection. Snapchat requires a Public Profile to publish Stories, Saved Stories, and Spotlight content.  **Headless Mode:** Use the &#x60;X-Connect-Token&#x60; header if you initiated the connection via API key.  After initiating Snapchat OAuth via &#x60;/v1/connect/snapchat?headless&#x3D;true&#x60;, you&#39;ll be redirected to your &#x60;redirect_url&#x60; with query params including: - &#x60;tempToken&#x60; - Temporary access token - &#x60;userProfile&#x60; - URL-encoded JSON with user info - &#x60;publicProfiles&#x60; - URL-encoded JSON array of available public profiles - &#x60;connect_token&#x60; - Short-lived token for API authentication - &#x60;platform&#x3D;snapchat&#x60; - &#x60;step&#x3D;select_public_profile&#x60;  Parse &#x60;publicProfiles&#x60; to build your custom selector UI, then call this endpoint with the selected profile. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        SelectSnapchatProfileRequest selectSnapchatProfileRequest = new SelectSnapchatProfileRequest(); // SelectSnapchatProfileRequest | 
        String xConnectToken = "xConnectToken_example"; // String | Short-lived connect token from the OAuth redirect (for API users)
        try {
            SelectSnapchatProfile200Response result = apiInstance.selectSnapchatProfile(selectSnapchatProfileRequest, xConnectToken);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#selectSnapchatProfile");
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
| **selectSnapchatProfileRequest** | [**SelectSnapchatProfileRequest**](SelectSnapchatProfileRequest.md)|  | |
| **xConnectToken** | **String**| Short-lived connect token from the OAuth redirect (for API users) | [optional] |

### Return type

[**SelectSnapchatProfile200Response**](SelectSnapchatProfile200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Snapchat Public Profile connected successfully |  -  |
| **400** | Missing required fields |  -  |
| **401** | Unauthorized |  -  |
| **403** | No access to profile or profile limit exceeded |  -  |
| **500** | Failed to connect Snapchat account |  -  |

## selectSnapchatProfileWithHttpInfo

> ApiResponse<SelectSnapchatProfile200Response> selectSnapchatProfile selectSnapchatProfileWithHttpInfo(selectSnapchatProfileRequest, xConnectToken)

Select Snapchat profile

**Complete the Snapchat Connection Flow**  After OAuth, use this endpoint to save the selected Public Profile and complete the Snapchat account connection. Snapchat requires a Public Profile to publish Stories, Saved Stories, and Spotlight content.  **Headless Mode:** Use the &#x60;X-Connect-Token&#x60; header if you initiated the connection via API key.  After initiating Snapchat OAuth via &#x60;/v1/connect/snapchat?headless&#x3D;true&#x60;, you&#39;ll be redirected to your &#x60;redirect_url&#x60; with query params including: - &#x60;tempToken&#x60; - Temporary access token - &#x60;userProfile&#x60; - URL-encoded JSON with user info - &#x60;publicProfiles&#x60; - URL-encoded JSON array of available public profiles - &#x60;connect_token&#x60; - Short-lived token for API authentication - &#x60;platform&#x3D;snapchat&#x60; - &#x60;step&#x3D;select_public_profile&#x60;  Parse &#x60;publicProfiles&#x60; to build your custom selector UI, then call this endpoint with the selected profile. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        SelectSnapchatProfileRequest selectSnapchatProfileRequest = new SelectSnapchatProfileRequest(); // SelectSnapchatProfileRequest | 
        String xConnectToken = "xConnectToken_example"; // String | Short-lived connect token from the OAuth redirect (for API users)
        try {
            ApiResponse<SelectSnapchatProfile200Response> response = apiInstance.selectSnapchatProfileWithHttpInfo(selectSnapchatProfileRequest, xConnectToken);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#selectSnapchatProfile");
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
| **selectSnapchatProfileRequest** | [**SelectSnapchatProfileRequest**](SelectSnapchatProfileRequest.md)|  | |
| **xConnectToken** | **String**| Short-lived connect token from the OAuth redirect (for API users) | [optional] |

### Return type

ApiResponse<[**SelectSnapchatProfile200Response**](SelectSnapchatProfile200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Snapchat Public Profile connected successfully |  -  |
| **400** | Missing required fields |  -  |
| **401** | Unauthorized |  -  |
| **403** | No access to profile or profile limit exceeded |  -  |
| **500** | Failed to connect Snapchat account |  -  |


## updateFacebookPage

> UpdateFacebookPage200Response updateFacebookPage(accountId, updateFacebookPageRequest)

Update Facebook page

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        UpdateFacebookPageRequest updateFacebookPageRequest = new UpdateFacebookPageRequest(); // UpdateFacebookPageRequest | 
        try {
            UpdateFacebookPage200Response result = apiInstance.updateFacebookPage(accountId, updateFacebookPageRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#updateFacebookPage");
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
| **accountId** | **String**|  | |
| **updateFacebookPageRequest** | [**UpdateFacebookPageRequest**](UpdateFacebookPageRequest.md)|  | |

### Return type

[**UpdateFacebookPage200Response**](UpdateFacebookPage200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Page updated |  -  |
| **400** | Page not in available pages |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## updateFacebookPageWithHttpInfo

> ApiResponse<UpdateFacebookPage200Response> updateFacebookPage updateFacebookPageWithHttpInfo(accountId, updateFacebookPageRequest)

Update Facebook page

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        UpdateFacebookPageRequest updateFacebookPageRequest = new UpdateFacebookPageRequest(); // UpdateFacebookPageRequest | 
        try {
            ApiResponse<UpdateFacebookPage200Response> response = apiInstance.updateFacebookPageWithHttpInfo(accountId, updateFacebookPageRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#updateFacebookPage");
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
| **accountId** | **String**|  | |
| **updateFacebookPageRequest** | [**UpdateFacebookPageRequest**](UpdateFacebookPageRequest.md)|  | |

### Return type

ApiResponse<[**UpdateFacebookPage200Response**](UpdateFacebookPage200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Page updated |  -  |
| **400** | Page not in available pages |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |


## updateGmbLocation

> UpdateGmbLocation200Response updateGmbLocation(accountId, updateGmbLocationRequest)

Update Google Business location

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        UpdateGmbLocationRequest updateGmbLocationRequest = new UpdateGmbLocationRequest(); // UpdateGmbLocationRequest | 
        try {
            UpdateGmbLocation200Response result = apiInstance.updateGmbLocation(accountId, updateGmbLocationRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#updateGmbLocation");
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
| **accountId** | **String**|  | |
| **updateGmbLocationRequest** | [**UpdateGmbLocationRequest**](UpdateGmbLocationRequest.md)|  | |

### Return type

[**UpdateGmbLocation200Response**](UpdateGmbLocation200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Location updated |  -  |
| **400** | Location not in available locations |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## updateGmbLocationWithHttpInfo

> ApiResponse<UpdateGmbLocation200Response> updateGmbLocation updateGmbLocationWithHttpInfo(accountId, updateGmbLocationRequest)

Update Google Business location

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        UpdateGmbLocationRequest updateGmbLocationRequest = new UpdateGmbLocationRequest(); // UpdateGmbLocationRequest | 
        try {
            ApiResponse<UpdateGmbLocation200Response> response = apiInstance.updateGmbLocationWithHttpInfo(accountId, updateGmbLocationRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#updateGmbLocation");
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
| **accountId** | **String**|  | |
| **updateGmbLocationRequest** | [**UpdateGmbLocationRequest**](UpdateGmbLocationRequest.md)|  | |

### Return type

ApiResponse<[**UpdateGmbLocation200Response**](UpdateGmbLocation200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Location updated |  -  |
| **400** | Location not in available locations |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |


## updateLinkedInOrganization

> ConnectBlueskyCredentials200Response updateLinkedInOrganization(accountId, updateLinkedInOrganizationRequest)

Switch LinkedIn account type

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        UpdateLinkedInOrganizationRequest updateLinkedInOrganizationRequest = new UpdateLinkedInOrganizationRequest(); // UpdateLinkedInOrganizationRequest | 
        try {
            ConnectBlueskyCredentials200Response result = apiInstance.updateLinkedInOrganization(accountId, updateLinkedInOrganizationRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#updateLinkedInOrganization");
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
| **accountId** | **String**|  | |
| **updateLinkedInOrganizationRequest** | [**UpdateLinkedInOrganizationRequest**](UpdateLinkedInOrganizationRequest.md)|  | |

### Return type

[**ConnectBlueskyCredentials200Response**](ConnectBlueskyCredentials200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Account updated |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## updateLinkedInOrganizationWithHttpInfo

> ApiResponse<ConnectBlueskyCredentials200Response> updateLinkedInOrganization updateLinkedInOrganizationWithHttpInfo(accountId, updateLinkedInOrganizationRequest)

Switch LinkedIn account type

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        UpdateLinkedInOrganizationRequest updateLinkedInOrganizationRequest = new UpdateLinkedInOrganizationRequest(); // UpdateLinkedInOrganizationRequest | 
        try {
            ApiResponse<ConnectBlueskyCredentials200Response> response = apiInstance.updateLinkedInOrganizationWithHttpInfo(accountId, updateLinkedInOrganizationRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#updateLinkedInOrganization");
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
| **accountId** | **String**|  | |
| **updateLinkedInOrganizationRequest** | [**UpdateLinkedInOrganizationRequest**](UpdateLinkedInOrganizationRequest.md)|  | |

### Return type

ApiResponse<[**ConnectBlueskyCredentials200Response**](ConnectBlueskyCredentials200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Account updated |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |


## updatePinterestBoards

> ConnectBlueskyCredentials200Response updatePinterestBoards(accountId, updatePinterestBoardsRequest)

Set default Pinterest board

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        UpdatePinterestBoardsRequest updatePinterestBoardsRequest = new UpdatePinterestBoardsRequest(); // UpdatePinterestBoardsRequest | 
        try {
            ConnectBlueskyCredentials200Response result = apiInstance.updatePinterestBoards(accountId, updatePinterestBoardsRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#updatePinterestBoards");
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
| **accountId** | **String**|  | |
| **updatePinterestBoardsRequest** | [**UpdatePinterestBoardsRequest**](UpdatePinterestBoardsRequest.md)|  | |

### Return type

[**ConnectBlueskyCredentials200Response**](ConnectBlueskyCredentials200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default board set |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## updatePinterestBoardsWithHttpInfo

> ApiResponse<ConnectBlueskyCredentials200Response> updatePinterestBoards updatePinterestBoardsWithHttpInfo(accountId, updatePinterestBoardsRequest)

Set default Pinterest board

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        UpdatePinterestBoardsRequest updatePinterestBoardsRequest = new UpdatePinterestBoardsRequest(); // UpdatePinterestBoardsRequest | 
        try {
            ApiResponse<ConnectBlueskyCredentials200Response> response = apiInstance.updatePinterestBoardsWithHttpInfo(accountId, updatePinterestBoardsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#updatePinterestBoards");
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
| **accountId** | **String**|  | |
| **updatePinterestBoardsRequest** | [**UpdatePinterestBoardsRequest**](UpdatePinterestBoardsRequest.md)|  | |

### Return type

ApiResponse<[**ConnectBlueskyCredentials200Response**](ConnectBlueskyCredentials200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default board set |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |


## updateRedditSubreddits

> UpdateRedditSubreddits200Response updateRedditSubreddits(accountId, updateRedditSubredditsRequest)

Set default subreddit

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        UpdateRedditSubredditsRequest updateRedditSubredditsRequest = new UpdateRedditSubredditsRequest(); // UpdateRedditSubredditsRequest | 
        try {
            UpdateRedditSubreddits200Response result = apiInstance.updateRedditSubreddits(accountId, updateRedditSubredditsRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#updateRedditSubreddits");
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
| **accountId** | **String**|  | |
| **updateRedditSubredditsRequest** | [**UpdateRedditSubredditsRequest**](UpdateRedditSubredditsRequest.md)|  | |

### Return type

[**UpdateRedditSubreddits200Response**](UpdateRedditSubreddits200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default subreddit set |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## updateRedditSubredditsWithHttpInfo

> ApiResponse<UpdateRedditSubreddits200Response> updateRedditSubreddits updateRedditSubredditsWithHttpInfo(accountId, updateRedditSubredditsRequest)

Set default subreddit

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        UpdateRedditSubredditsRequest updateRedditSubredditsRequest = new UpdateRedditSubredditsRequest(); // UpdateRedditSubredditsRequest | 
        try {
            ApiResponse<UpdateRedditSubreddits200Response> response = apiInstance.updateRedditSubredditsWithHttpInfo(accountId, updateRedditSubredditsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#updateRedditSubreddits");
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
| **accountId** | **String**|  | |
| **updateRedditSubredditsRequest** | [**UpdateRedditSubredditsRequest**](UpdateRedditSubredditsRequest.md)|  | |

### Return type

ApiResponse<[**UpdateRedditSubreddits200Response**](UpdateRedditSubreddits200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default subreddit set |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

