# ConnectApi

All URIs are relative to *https://zernio.com/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**completeTelegramConnect**](ConnectApi.md#completeTelegramConnect) | **PATCH** /v1/connect/telegram | Check Telegram status |
| [**completeTelegramConnectWithHttpInfo**](ConnectApi.md#completeTelegramConnectWithHttpInfo) | **PATCH** /v1/connect/telegram | Check Telegram status |
| [**completeWhatsAppPhoneSelection**](ConnectApi.md#completeWhatsAppPhoneSelection) | **POST** /v1/connect/whatsapp/select-phone-number | Complete WhatsApp phone number selection |
| [**completeWhatsAppPhoneSelectionWithHttpInfo**](ConnectApi.md#completeWhatsAppPhoneSelectionWithHttpInfo) | **POST** /v1/connect/whatsapp/select-phone-number | Complete WhatsApp phone number selection |
| [**configureTikTokAdsBrandIdentity**](ConnectApi.md#configureTikTokAdsBrandIdentity) | **PATCH** /v1/connect/tiktok-ads | Configure TikTok Ads Brand Identity |
| [**configureTikTokAdsBrandIdentityWithHttpInfo**](ConnectApi.md#configureTikTokAdsBrandIdentityWithHttpInfo) | **PATCH** /v1/connect/tiktok-ads | Configure TikTok Ads Brand Identity |
| [**connectAds**](ConnectApi.md#connectAds) | **GET** /v1/connect/{platform}/ads | Connect ads for a platform |
| [**connectAdsWithHttpInfo**](ConnectApi.md#connectAdsWithHttpInfo) | **GET** /v1/connect/{platform}/ads | Connect ads for a platform |
| [**connectBlueskyCredentials**](ConnectApi.md#connectBlueskyCredentials) | **POST** /v1/connect/bluesky/credentials | Connect Bluesky account |
| [**connectBlueskyCredentialsWithHttpInfo**](ConnectApi.md#connectBlueskyCredentialsWithHttpInfo) | **POST** /v1/connect/bluesky/credentials | Connect Bluesky account |
| [**connectWhatsAppCredentials**](ConnectApi.md#connectWhatsAppCredentials) | **POST** /v1/connect/whatsapp/credentials | Connect WhatsApp via credentials |
| [**connectWhatsAppCredentialsWithHttpInfo**](ConnectApi.md#connectWhatsAppCredentialsWithHttpInfo) | **POST** /v1/connect/whatsapp/credentials | Connect WhatsApp via credentials |
| [**getConnectUrl**](ConnectApi.md#getConnectUrl) | **GET** /v1/connect/{platform} | Get OAuth connect URL |
| [**getConnectUrlWithHttpInfo**](ConnectApi.md#getConnectUrlWithHttpInfo) | **GET** /v1/connect/{platform} | Get OAuth connect URL |
| [**getFacebookPages**](ConnectApi.md#getFacebookPages) | **GET** /v1/accounts/{accountId}/facebook-page | List Facebook pages |
| [**getFacebookPagesWithHttpInfo**](ConnectApi.md#getFacebookPagesWithHttpInfo) | **GET** /v1/accounts/{accountId}/facebook-page | List Facebook pages |
| [**getGmbLocations**](ConnectApi.md#getGmbLocations) | **GET** /v1/accounts/{accountId}/gmb-locations | List GBP locations |
| [**getGmbLocationsWithHttpInfo**](ConnectApi.md#getGmbLocationsWithHttpInfo) | **GET** /v1/accounts/{accountId}/gmb-locations | List GBP locations |
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
| [**getYoutubePlaylists**](ConnectApi.md#getYoutubePlaylists) | **GET** /v1/accounts/{accountId}/youtube-playlists | List YouTube playlists |
| [**getYoutubePlaylistsWithHttpInfo**](ConnectApi.md#getYoutubePlaylistsWithHttpInfo) | **GET** /v1/accounts/{accountId}/youtube-playlists | List YouTube playlists |
| [**handleOAuthCallback**](ConnectApi.md#handleOAuthCallback) | **POST** /v1/connect/{platform} | Complete OAuth callback |
| [**handleOAuthCallbackWithHttpInfo**](ConnectApi.md#handleOAuthCallbackWithHttpInfo) | **POST** /v1/connect/{platform} | Complete OAuth callback |
| [**initiateTelegramConnect**](ConnectApi.md#initiateTelegramConnect) | **POST** /v1/connect/telegram | Connect Telegram directly |
| [**initiateTelegramConnectWithHttpInfo**](ConnectApi.md#initiateTelegramConnectWithHttpInfo) | **POST** /v1/connect/telegram | Connect Telegram directly |
| [**listFacebookPages**](ConnectApi.md#listFacebookPages) | **GET** /v1/connect/facebook/select-page | List Facebook pages |
| [**listFacebookPagesWithHttpInfo**](ConnectApi.md#listFacebookPagesWithHttpInfo) | **GET** /v1/connect/facebook/select-page | List Facebook pages |
| [**listGoogleBusinessLocations**](ConnectApi.md#listGoogleBusinessLocations) | **GET** /v1/connect/googlebusiness/locations | List GBP locations |
| [**listGoogleBusinessLocationsWithHttpInfo**](ConnectApi.md#listGoogleBusinessLocationsWithHttpInfo) | **GET** /v1/connect/googlebusiness/locations | List GBP locations |
| [**listLinkedInOrganizations**](ConnectApi.md#listLinkedInOrganizations) | **GET** /v1/connect/linkedin/organizations | List LinkedIn orgs |
| [**listLinkedInOrganizationsWithHttpInfo**](ConnectApi.md#listLinkedInOrganizationsWithHttpInfo) | **GET** /v1/connect/linkedin/organizations | List LinkedIn orgs |
| [**listPinterestBoardsForSelection**](ConnectApi.md#listPinterestBoardsForSelection) | **GET** /v1/connect/pinterest/select-board | List Pinterest boards |
| [**listPinterestBoardsForSelectionWithHttpInfo**](ConnectApi.md#listPinterestBoardsForSelectionWithHttpInfo) | **GET** /v1/connect/pinterest/select-board | List Pinterest boards |
| [**listSnapchatProfiles**](ConnectApi.md#listSnapchatProfiles) | **GET** /v1/connect/snapchat/select-profile | List Snapchat profiles |
| [**listSnapchatProfilesWithHttpInfo**](ConnectApi.md#listSnapchatProfilesWithHttpInfo) | **GET** /v1/connect/snapchat/select-profile | List Snapchat profiles |
| [**listWhatsAppPhoneNumbers**](ConnectApi.md#listWhatsAppPhoneNumbers) | **GET** /v1/connect/whatsapp/select-phone-number | List WhatsApp phone numbers for selection |
| [**listWhatsAppPhoneNumbersWithHttpInfo**](ConnectApi.md#listWhatsAppPhoneNumbersWithHttpInfo) | **GET** /v1/connect/whatsapp/select-phone-number | List WhatsApp phone numbers for selection |
| [**selectFacebookPage**](ConnectApi.md#selectFacebookPage) | **POST** /v1/connect/facebook/select-page | Select Facebook page |
| [**selectFacebookPageWithHttpInfo**](ConnectApi.md#selectFacebookPageWithHttpInfo) | **POST** /v1/connect/facebook/select-page | Select Facebook page |
| [**selectGoogleBusinessLocation**](ConnectApi.md#selectGoogleBusinessLocation) | **POST** /v1/connect/googlebusiness/select-location | Select GBP location |
| [**selectGoogleBusinessLocationWithHttpInfo**](ConnectApi.md#selectGoogleBusinessLocationWithHttpInfo) | **POST** /v1/connect/googlebusiness/select-location | Select GBP location |
| [**selectLinkedInOrganization**](ConnectApi.md#selectLinkedInOrganization) | **POST** /v1/connect/linkedin/select-organization | Select LinkedIn org |
| [**selectLinkedInOrganizationWithHttpInfo**](ConnectApi.md#selectLinkedInOrganizationWithHttpInfo) | **POST** /v1/connect/linkedin/select-organization | Select LinkedIn org |
| [**selectPinterestBoard**](ConnectApi.md#selectPinterestBoard) | **POST** /v1/connect/pinterest/select-board | Select Pinterest board |
| [**selectPinterestBoardWithHttpInfo**](ConnectApi.md#selectPinterestBoardWithHttpInfo) | **POST** /v1/connect/pinterest/select-board | Select Pinterest board |
| [**selectSnapchatProfile**](ConnectApi.md#selectSnapchatProfile) | **POST** /v1/connect/snapchat/select-profile | Select Snapchat profile |
| [**selectSnapchatProfileWithHttpInfo**](ConnectApi.md#selectSnapchatProfileWithHttpInfo) | **POST** /v1/connect/snapchat/select-profile | Select Snapchat profile |
| [**updateFacebookPage**](ConnectApi.md#updateFacebookPage) | **PUT** /v1/accounts/{accountId}/facebook-page | Update Facebook page |
| [**updateFacebookPageWithHttpInfo**](ConnectApi.md#updateFacebookPageWithHttpInfo) | **PUT** /v1/accounts/{accountId}/facebook-page | Update Facebook page |
| [**updateGmbLocation**](ConnectApi.md#updateGmbLocation) | **PUT** /v1/accounts/{accountId}/gmb-locations | Update GBP location |
| [**updateGmbLocationWithHttpInfo**](ConnectApi.md#updateGmbLocationWithHttpInfo) | **PUT** /v1/accounts/{accountId}/gmb-locations | Update GBP location |
| [**updateLinkedInOrganization**](ConnectApi.md#updateLinkedInOrganization) | **PUT** /v1/accounts/{accountId}/linkedin-organization | Switch LinkedIn account type |
| [**updateLinkedInOrganizationWithHttpInfo**](ConnectApi.md#updateLinkedInOrganizationWithHttpInfo) | **PUT** /v1/accounts/{accountId}/linkedin-organization | Switch LinkedIn account type |
| [**updatePinterestBoards**](ConnectApi.md#updatePinterestBoards) | **PUT** /v1/accounts/{accountId}/pinterest-boards | Set default Pinterest board |
| [**updatePinterestBoardsWithHttpInfo**](ConnectApi.md#updatePinterestBoardsWithHttpInfo) | **PUT** /v1/accounts/{accountId}/pinterest-boards | Set default Pinterest board |
| [**updateRedditSubreddits**](ConnectApi.md#updateRedditSubreddits) | **PUT** /v1/accounts/{accountId}/reddit-subreddits | Set default subreddit |
| [**updateRedditSubredditsWithHttpInfo**](ConnectApi.md#updateRedditSubredditsWithHttpInfo) | **PUT** /v1/accounts/{accountId}/reddit-subreddits | Set default subreddit |
| [**updateYoutubeDefaultPlaylist**](ConnectApi.md#updateYoutubeDefaultPlaylist) | **PUT** /v1/accounts/{accountId}/youtube-playlists | Set default YouTube playlist |
| [**updateYoutubeDefaultPlaylistWithHttpInfo**](ConnectApi.md#updateYoutubeDefaultPlaylistWithHttpInfo) | **PUT** /v1/accounts/{accountId}/youtube-playlists | Set default YouTube playlist |



## completeTelegramConnect

> CompleteTelegramConnect200Response completeTelegramConnect(code)

Check Telegram status

Poll this endpoint to check if a Telegram access code has been used to connect a channel/group. Recommended polling interval: 3 seconds. Status values: pending (waiting for user), connected (channel/group linked), expired (generate a new code). 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String code = "ZRN-ABC123"; // String | The access code to check status for
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

Poll this endpoint to check if a Telegram access code has been used to connect a channel/group. Recommended polling interval: 3 seconds. Status values: pending (waiting for user), connected (channel/group linked), expired (generate a new code). 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String code = "ZRN-ABC123"; // String | The access code to check status for
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


## completeWhatsAppPhoneSelection

> CompleteWhatsAppPhoneSelection200Response completeWhatsAppPhoneSelection(completeWhatsAppPhoneSelectionRequest, xConnectToken)

Complete WhatsApp phone number selection

Bind a specific WhatsApp phone number to the Zernio profile after the user picks one from &#x60;listWhatsAppPhoneNumbers&#x60;. Exchanges the short-lived OAuth token for a long-lived token, subscribes the WABA to webhooks, and creates the SocialAccount. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        CompleteWhatsAppPhoneSelectionRequest completeWhatsAppPhoneSelectionRequest = new CompleteWhatsAppPhoneSelectionRequest(); // CompleteWhatsAppPhoneSelectionRequest | 
        String xConnectToken = "xConnectToken_example"; // String | Alternative auth for API users' end customers
        try {
            CompleteWhatsAppPhoneSelection200Response result = apiInstance.completeWhatsAppPhoneSelection(completeWhatsAppPhoneSelectionRequest, xConnectToken);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#completeWhatsAppPhoneSelection");
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
| **completeWhatsAppPhoneSelectionRequest** | [**CompleteWhatsAppPhoneSelectionRequest**](CompleteWhatsAppPhoneSelectionRequest.md)|  | |
| **xConnectToken** | **String**| Alternative auth for API users&#39; end customers | [optional] |

### Return type

[**CompleteWhatsAppPhoneSelection200Response**](CompleteWhatsAppPhoneSelection200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Phone number connected successfully |  -  |
| **400** | Missing required fields (profileId, phoneNumberId, wabaId, or tempToken) |  -  |
| **401** | Unauthorized |  -  |
| **403** | Profile limit exceeded for the user&#39;s plan (PROFILE_LIMIT_EXCEEDED) |  -  |
| **404** | Selected phone number not found in the specified WABA |  -  |
| **500** | Failed to bind phone number |  -  |

## completeWhatsAppPhoneSelectionWithHttpInfo

> ApiResponse<CompleteWhatsAppPhoneSelection200Response> completeWhatsAppPhoneSelection completeWhatsAppPhoneSelectionWithHttpInfo(completeWhatsAppPhoneSelectionRequest, xConnectToken)

Complete WhatsApp phone number selection

Bind a specific WhatsApp phone number to the Zernio profile after the user picks one from &#x60;listWhatsAppPhoneNumbers&#x60;. Exchanges the short-lived OAuth token for a long-lived token, subscribes the WABA to webhooks, and creates the SocialAccount. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        CompleteWhatsAppPhoneSelectionRequest completeWhatsAppPhoneSelectionRequest = new CompleteWhatsAppPhoneSelectionRequest(); // CompleteWhatsAppPhoneSelectionRequest | 
        String xConnectToken = "xConnectToken_example"; // String | Alternative auth for API users' end customers
        try {
            ApiResponse<CompleteWhatsAppPhoneSelection200Response> response = apiInstance.completeWhatsAppPhoneSelectionWithHttpInfo(completeWhatsAppPhoneSelectionRequest, xConnectToken);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#completeWhatsAppPhoneSelection");
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
| **completeWhatsAppPhoneSelectionRequest** | [**CompleteWhatsAppPhoneSelectionRequest**](CompleteWhatsAppPhoneSelectionRequest.md)|  | |
| **xConnectToken** | **String**| Alternative auth for API users&#39; end customers | [optional] |

### Return type

ApiResponse<[**CompleteWhatsAppPhoneSelection200Response**](CompleteWhatsAppPhoneSelection200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Phone number connected successfully |  -  |
| **400** | Missing required fields (profileId, phoneNumberId, wabaId, or tempToken) |  -  |
| **401** | Unauthorized |  -  |
| **403** | Profile limit exceeded for the user&#39;s plan (PROFILE_LIMIT_EXCEEDED) |  -  |
| **404** | Selected phone number not found in the specified WABA |  -  |
| **500** | Failed to bind phone number |  -  |


## configureTikTokAdsBrandIdentity

> ConfigureTikTokAdsBrandIdentity200Response configureTikTokAdsBrandIdentity(configureTikTokAdsBrandIdentityRequest)

Configure TikTok Ads Brand Identity

Set or update the Brand Identity (display name + avatar) for a &#x60;tiktokads&#x60; SocialAccount. TikTok requires every ad to carry an &#x60;identity_id + identity_type&#x60; pair. The Brand Identity is the CUSTOMIZED_USER alternative to attributing ads to a real @username (TT_USER). This route uploads the supplied image to TikTok, creates the identity via &#x60;/v2/identity/create/&#x60;, and caches the resulting &#x60;identity_id&#x60; on the account so subsequent &#x60;POST /v1/ads/create&#x60; calls can opt into it via &#x60;identityType: &#39;CUSTOMIZED_USER&#39;&#x60;.  Configurable on every &#x60;tiktokads&#x60; account, including linked-mode ones (those with a posting account on the same profile). Configuration is idempotent and harmless when posting is also connected: the default ad-create path still prefers TT_USER, and CUSTOMIZED_USER is only used per-ad when the caller explicitly opts in.  TikTok identities are immutable post-creation. Re-saving creates a new identity on TikTok and swaps the cached id; the old identity stays orphaned on TikTok&#39;s side (harmless, no billing impact).  Alternative: pass &#x60;brandIdentity&#x60; directly on &#x60;POST /v1/ads/create&#x60; to configure on first ad creation in a single round-trip. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        ConfigureTikTokAdsBrandIdentityRequest configureTikTokAdsBrandIdentityRequest = new ConfigureTikTokAdsBrandIdentityRequest(); // ConfigureTikTokAdsBrandIdentityRequest | 
        try {
            ConfigureTikTokAdsBrandIdentity200Response result = apiInstance.configureTikTokAdsBrandIdentity(configureTikTokAdsBrandIdentityRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#configureTikTokAdsBrandIdentity");
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
| **configureTikTokAdsBrandIdentityRequest** | [**ConfigureTikTokAdsBrandIdentityRequest**](ConfigureTikTokAdsBrandIdentityRequest.md)|  | |

### Return type

[**ConfigureTikTokAdsBrandIdentity200Response**](ConfigureTikTokAdsBrandIdentity200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Brand identity configured (or updated) |  -  |
| **400** | Missing fields, invalid lengths, account is in linked mode, or no advertiser found on the account |  -  |
| **401** | Unauthorized |  -  |
| **404** | TikTok Ads account not found |  -  |
| **500** | Failed to create the TikTok identity (TikTok API error) |  -  |

## configureTikTokAdsBrandIdentityWithHttpInfo

> ApiResponse<ConfigureTikTokAdsBrandIdentity200Response> configureTikTokAdsBrandIdentity configureTikTokAdsBrandIdentityWithHttpInfo(configureTikTokAdsBrandIdentityRequest)

Configure TikTok Ads Brand Identity

Set or update the Brand Identity (display name + avatar) for a &#x60;tiktokads&#x60; SocialAccount. TikTok requires every ad to carry an &#x60;identity_id + identity_type&#x60; pair. The Brand Identity is the CUSTOMIZED_USER alternative to attributing ads to a real @username (TT_USER). This route uploads the supplied image to TikTok, creates the identity via &#x60;/v2/identity/create/&#x60;, and caches the resulting &#x60;identity_id&#x60; on the account so subsequent &#x60;POST /v1/ads/create&#x60; calls can opt into it via &#x60;identityType: &#39;CUSTOMIZED_USER&#39;&#x60;.  Configurable on every &#x60;tiktokads&#x60; account, including linked-mode ones (those with a posting account on the same profile). Configuration is idempotent and harmless when posting is also connected: the default ad-create path still prefers TT_USER, and CUSTOMIZED_USER is only used per-ad when the caller explicitly opts in.  TikTok identities are immutable post-creation. Re-saving creates a new identity on TikTok and swaps the cached id; the old identity stays orphaned on TikTok&#39;s side (harmless, no billing impact).  Alternative: pass &#x60;brandIdentity&#x60; directly on &#x60;POST /v1/ads/create&#x60; to configure on first ad creation in a single round-trip. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        ConfigureTikTokAdsBrandIdentityRequest configureTikTokAdsBrandIdentityRequest = new ConfigureTikTokAdsBrandIdentityRequest(); // ConfigureTikTokAdsBrandIdentityRequest | 
        try {
            ApiResponse<ConfigureTikTokAdsBrandIdentity200Response> response = apiInstance.configureTikTokAdsBrandIdentityWithHttpInfo(configureTikTokAdsBrandIdentityRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#configureTikTokAdsBrandIdentity");
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
| **configureTikTokAdsBrandIdentityRequest** | [**ConfigureTikTokAdsBrandIdentityRequest**](ConfigureTikTokAdsBrandIdentityRequest.md)|  | |

### Return type

ApiResponse<[**ConfigureTikTokAdsBrandIdentity200Response**](ConfigureTikTokAdsBrandIdentity200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Brand identity configured (or updated) |  -  |
| **400** | Missing fields, invalid lengths, account is in linked mode, or no advertiser found on the account |  -  |
| **401** | Unauthorized |  -  |
| **404** | TikTok Ads account not found |  -  |
| **500** | Failed to create the TikTok identity (TikTok API error) |  -  |


## connectAds

> ConnectAds200Response connectAds(platform, profileId, accountId, redirectUrl, headless, adAccountId, adAccountIds)

Connect ads for a platform

Unified ads connection endpoint. Creates a dedicated ads SocialAccount for the specified platform.  Same-token platforms (facebook, instagram, linkedin, pinterest): Creates an ads SocialAccount (metaads, linkedinads, pinterestads) with a copied OAuth token from the parent posting account. If the ads account already exists, returns alreadyConnected: true. No extra OAuth needed.  Separate-token platforms (tiktok, twitter): Starts the platform-specific marketing API OAuth flow and creates an ads SocialAccount (tiktokads, xads) with its own token. If the ads account already exists, returns alreadyConnected: true.   - tiktok: accountId is OPTIONAL. With accountId, the new tiktokads account links to that posting account (parentAccountId set) — Spark Ads + standalone ads using the posting TT_USER identity become available. Without accountId, ads-only mode kicks in: the new tiktokads account has parentAccountId&#x3D;null and standalone ads use a synthetic CUSTOMIZED_USER (\&quot;Brand Identity\&quot;); Spark Ads are unavailable because TikTok requires a posting account for them. The Brand Identity is configured separately via PATCH /v1/connect/tiktok-ads (or inline on POST /v1/ads/create via the brandIdentity field).   - twitter (X Ads): accountId is REQUIRED. There&#39;s no ads-only mode — tweets need to be authored by a real X user.  Standalone platforms (googleads): Starts the Google Ads OAuth flow and creates a standalone ads SocialAccount (googleads) with no parent. If the account already exists, returns alreadyConnected: true.  Ads accounts appear as regular SocialAccount documents with ads platform values (e.g., metaads, tiktokads) in GET /v1/accounts. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String platform = "facebook"; // String | Platform to connect ads for. Only platforms with ads support are accepted.
        String profileId = "profileId_example"; // String | Your Zernio profile ID
        String accountId = "accountId_example"; // String | Existing SocialAccount ID. Required for `twitter` (X Ads). Optional for `tiktok` — omit to enter ads-only mode (no TikTok posting account linked; ad creation uses a Brand Identity instead of a TT_USER). Ignored for same-token (`facebook`, `instagram`, `linkedin`, `pinterest`) and standalone (`googleads`) platforms. 
        URI redirectUrl = new URI(); // URI | Custom redirect URL after OAuth completes (same-token platforms only)
        Boolean headless = false; // Boolean | Enable headless mode (same-token platforms only)
        String adAccountId = "act_1330190928038136"; // String | (metaads only) Scope ad sync to a single Meta ad account. Without this param, sync covers every `act_*` the connected token can see. Pass this to limit `sync.totalAds` / `synced` and the resulting ads to one ad account. Format: `act_<digits>` (matches what `/me/adaccounts` returns). Validated against the connected token; unreachable IDs return 400. For multiple accounts use `adAccountIds` instead. 
        List<String> adAccountIds = Arrays.asList(); // List<String> | (metaads only) Scope ad sync to multiple Meta ad accounts. Repeat the param (`?adAccountIds=act_1&adAccountIds=act_2`) or comma-separate (`?adAccountIds=act_1,act_2`). Validated against the connected token. Persisted server-side; latest call wins. Omitting both `adAccountId` and `adAccountIds` keeps any previously persisted scope unchanged. 
        try {
            ConnectAds200Response result = apiInstance.connectAds(platform, profileId, accountId, redirectUrl, headless, adAccountId, adAccountIds);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#connectAds");
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
| **platform** | **String**| Platform to connect ads for. Only platforms with ads support are accepted. | [enum: facebook, instagram, linkedin, tiktok, twitter, pinterest, googleads] |
| **profileId** | **String**| Your Zernio profile ID | |
| **accountId** | **String**| Existing SocialAccount ID. Required for &#x60;twitter&#x60; (X Ads). Optional for &#x60;tiktok&#x60; — omit to enter ads-only mode (no TikTok posting account linked; ad creation uses a Brand Identity instead of a TT_USER). Ignored for same-token (&#x60;facebook&#x60;, &#x60;instagram&#x60;, &#x60;linkedin&#x60;, &#x60;pinterest&#x60;) and standalone (&#x60;googleads&#x60;) platforms.  | [optional] |
| **redirectUrl** | **URI**| Custom redirect URL after OAuth completes (same-token platforms only) | [optional] |
| **headless** | **Boolean**| Enable headless mode (same-token platforms only) | [optional] [default to false] |
| **adAccountId** | **String**| (metaads only) Scope ad sync to a single Meta ad account. Without this param, sync covers every &#x60;act_*&#x60; the connected token can see. Pass this to limit &#x60;sync.totalAds&#x60; / &#x60;synced&#x60; and the resulting ads to one ad account. Format: &#x60;act_&lt;digits&gt;&#x60; (matches what &#x60;/me/adaccounts&#x60; returns). Validated against the connected token; unreachable IDs return 400. For multiple accounts use &#x60;adAccountIds&#x60; instead.  | [optional] |
| **adAccountIds** | [**List&lt;String&gt;**](String.md)| (metaads only) Scope ad sync to multiple Meta ad accounts. Repeat the param (&#x60;?adAccountIds&#x3D;act_1&amp;adAccountIds&#x3D;act_2&#x60;) or comma-separate (&#x60;?adAccountIds&#x3D;act_1,act_2&#x60;). Validated against the connected token. Persisted server-side; latest call wins. Omitting both &#x60;adAccountId&#x60; and &#x60;adAccountIds&#x60; keeps any previously persisted scope unchanged.  | [optional] |

### Return type

[**ConnectAds200Response**](ConnectAds200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Either an OAuth URL to redirect to, or confirmation that ads are already connected |  -  |
| **400** | Platform doesn&#39;t support ads, or missing accountId for X Ads |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required, or no access to profile |  -  |
| **404** | Profile or posting account not found |  -  |

## connectAdsWithHttpInfo

> ApiResponse<ConnectAds200Response> connectAds connectAdsWithHttpInfo(platform, profileId, accountId, redirectUrl, headless, adAccountId, adAccountIds)

Connect ads for a platform

Unified ads connection endpoint. Creates a dedicated ads SocialAccount for the specified platform.  Same-token platforms (facebook, instagram, linkedin, pinterest): Creates an ads SocialAccount (metaads, linkedinads, pinterestads) with a copied OAuth token from the parent posting account. If the ads account already exists, returns alreadyConnected: true. No extra OAuth needed.  Separate-token platforms (tiktok, twitter): Starts the platform-specific marketing API OAuth flow and creates an ads SocialAccount (tiktokads, xads) with its own token. If the ads account already exists, returns alreadyConnected: true.   - tiktok: accountId is OPTIONAL. With accountId, the new tiktokads account links to that posting account (parentAccountId set) — Spark Ads + standalone ads using the posting TT_USER identity become available. Without accountId, ads-only mode kicks in: the new tiktokads account has parentAccountId&#x3D;null and standalone ads use a synthetic CUSTOMIZED_USER (\&quot;Brand Identity\&quot;); Spark Ads are unavailable because TikTok requires a posting account for them. The Brand Identity is configured separately via PATCH /v1/connect/tiktok-ads (or inline on POST /v1/ads/create via the brandIdentity field).   - twitter (X Ads): accountId is REQUIRED. There&#39;s no ads-only mode — tweets need to be authored by a real X user.  Standalone platforms (googleads): Starts the Google Ads OAuth flow and creates a standalone ads SocialAccount (googleads) with no parent. If the account already exists, returns alreadyConnected: true.  Ads accounts appear as regular SocialAccount documents with ads platform values (e.g., metaads, tiktokads) in GET /v1/accounts. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String platform = "facebook"; // String | Platform to connect ads for. Only platforms with ads support are accepted.
        String profileId = "profileId_example"; // String | Your Zernio profile ID
        String accountId = "accountId_example"; // String | Existing SocialAccount ID. Required for `twitter` (X Ads). Optional for `tiktok` — omit to enter ads-only mode (no TikTok posting account linked; ad creation uses a Brand Identity instead of a TT_USER). Ignored for same-token (`facebook`, `instagram`, `linkedin`, `pinterest`) and standalone (`googleads`) platforms. 
        URI redirectUrl = new URI(); // URI | Custom redirect URL after OAuth completes (same-token platforms only)
        Boolean headless = false; // Boolean | Enable headless mode (same-token platforms only)
        String adAccountId = "act_1330190928038136"; // String | (metaads only) Scope ad sync to a single Meta ad account. Without this param, sync covers every `act_*` the connected token can see. Pass this to limit `sync.totalAds` / `synced` and the resulting ads to one ad account. Format: `act_<digits>` (matches what `/me/adaccounts` returns). Validated against the connected token; unreachable IDs return 400. For multiple accounts use `adAccountIds` instead. 
        List<String> adAccountIds = Arrays.asList(); // List<String> | (metaads only) Scope ad sync to multiple Meta ad accounts. Repeat the param (`?adAccountIds=act_1&adAccountIds=act_2`) or comma-separate (`?adAccountIds=act_1,act_2`). Validated against the connected token. Persisted server-side; latest call wins. Omitting both `adAccountId` and `adAccountIds` keeps any previously persisted scope unchanged. 
        try {
            ApiResponse<ConnectAds200Response> response = apiInstance.connectAdsWithHttpInfo(platform, profileId, accountId, redirectUrl, headless, adAccountId, adAccountIds);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#connectAds");
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
| **platform** | **String**| Platform to connect ads for. Only platforms with ads support are accepted. | [enum: facebook, instagram, linkedin, tiktok, twitter, pinterest, googleads] |
| **profileId** | **String**| Your Zernio profile ID | |
| **accountId** | **String**| Existing SocialAccount ID. Required for &#x60;twitter&#x60; (X Ads). Optional for &#x60;tiktok&#x60; — omit to enter ads-only mode (no TikTok posting account linked; ad creation uses a Brand Identity instead of a TT_USER). Ignored for same-token (&#x60;facebook&#x60;, &#x60;instagram&#x60;, &#x60;linkedin&#x60;, &#x60;pinterest&#x60;) and standalone (&#x60;googleads&#x60;) platforms.  | [optional] |
| **redirectUrl** | **URI**| Custom redirect URL after OAuth completes (same-token platforms only) | [optional] |
| **headless** | **Boolean**| Enable headless mode (same-token platforms only) | [optional] [default to false] |
| **adAccountId** | **String**| (metaads only) Scope ad sync to a single Meta ad account. Without this param, sync covers every &#x60;act_*&#x60; the connected token can see. Pass this to limit &#x60;sync.totalAds&#x60; / &#x60;synced&#x60; and the resulting ads to one ad account. Format: &#x60;act_&lt;digits&gt;&#x60; (matches what &#x60;/me/adaccounts&#x60; returns). Validated against the connected token; unreachable IDs return 400. For multiple accounts use &#x60;adAccountIds&#x60; instead.  | [optional] |
| **adAccountIds** | [**List&lt;String&gt;**](String.md)| (metaads only) Scope ad sync to multiple Meta ad accounts. Repeat the param (&#x60;?adAccountIds&#x3D;act_1&amp;adAccountIds&#x3D;act_2&#x60;) or comma-separate (&#x60;?adAccountIds&#x3D;act_1,act_2&#x60;). Validated against the connected token. Persisted server-side; latest call wins. Omitting both &#x60;adAccountId&#x60; and &#x60;adAccountIds&#x60; keeps any previously persisted scope unchanged.  | [optional] |

### Return type

ApiResponse<[**ConnectAds200Response**](ConnectAds200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Either an OAuth URL to redirect to, or confirmation that ads are already connected |  -  |
| **400** | Platform doesn&#39;t support ads, or missing accountId for X Ads |  -  |
| **401** | Unauthorized |  -  |
| **403** | Ads add-on required, or no access to profile |  -  |
| **404** | Profile or posting account not found |  -  |


## connectBlueskyCredentials

> ConnectBlueskyCredentials200Response connectBlueskyCredentials(connectBlueskyCredentialsRequest)

Connect Bluesky account

Connect a Bluesky account using identifier (handle or email) and an app password. To get your userId for the state parameter, call GET /v1/users which includes a currentUserId field. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Connect a Bluesky account using identifier (handle or email) and an app password. To get your userId for the state parameter, call GET /v1/users which includes a currentUserId field. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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


## connectWhatsAppCredentials

> ConnectWhatsAppCredentials200Response connectWhatsAppCredentials(connectWhatsAppCredentialsRequest)

Connect WhatsApp via credentials

Connect a WhatsApp Business Account by providing Meta credentials directly. This is the headless alternative to the Embedded Signup browser flow.  To get the required credentials: 1. Go to Meta Business Suite (business.facebook.com) 2. Create or select a WhatsApp Business Account 3. In Business Settings &gt; System Users, create a System User 4. Assign it the whatsapp_business_management and whatsapp_business_messaging permissions 5. Generate a permanent access token 6. Get the WABA ID from WhatsApp Manager &gt; Account Tools &gt; Phone Numbers 7. Get the Phone Number ID from the same page (click on the number) 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        ConnectWhatsAppCredentialsRequest connectWhatsAppCredentialsRequest = new ConnectWhatsAppCredentialsRequest(); // ConnectWhatsAppCredentialsRequest | 
        try {
            ConnectWhatsAppCredentials200Response result = apiInstance.connectWhatsAppCredentials(connectWhatsAppCredentialsRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#connectWhatsAppCredentials");
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
| **connectWhatsAppCredentialsRequest** | [**ConnectWhatsAppCredentialsRequest**](ConnectWhatsAppCredentialsRequest.md)|  | |

### Return type

[**ConnectWhatsAppCredentials200Response**](ConnectWhatsAppCredentials200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | WhatsApp connected successfully |  -  |
| **400** | Invalid request. Either missing fields or the phoneNumberId was not found in the specified WABA. If the phone was not found, the response includes availablePhoneNumbers to help identify the correct ID.  |  -  |
| **401** | Invalid or expired access token |  -  |
| **403** | Profile limit exceeded for this plan |  -  |

## connectWhatsAppCredentialsWithHttpInfo

> ApiResponse<ConnectWhatsAppCredentials200Response> connectWhatsAppCredentials connectWhatsAppCredentialsWithHttpInfo(connectWhatsAppCredentialsRequest)

Connect WhatsApp via credentials

Connect a WhatsApp Business Account by providing Meta credentials directly. This is the headless alternative to the Embedded Signup browser flow.  To get the required credentials: 1. Go to Meta Business Suite (business.facebook.com) 2. Create or select a WhatsApp Business Account 3. In Business Settings &gt; System Users, create a System User 4. Assign it the whatsapp_business_management and whatsapp_business_messaging permissions 5. Generate a permanent access token 6. Get the WABA ID from WhatsApp Manager &gt; Account Tools &gt; Phone Numbers 7. Get the Phone Number ID from the same page (click on the number) 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        ConnectWhatsAppCredentialsRequest connectWhatsAppCredentialsRequest = new ConnectWhatsAppCredentialsRequest(); // ConnectWhatsAppCredentialsRequest | 
        try {
            ApiResponse<ConnectWhatsAppCredentials200Response> response = apiInstance.connectWhatsAppCredentialsWithHttpInfo(connectWhatsAppCredentialsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#connectWhatsAppCredentials");
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
| **connectWhatsAppCredentialsRequest** | [**ConnectWhatsAppCredentialsRequest**](ConnectWhatsAppCredentialsRequest.md)|  | |

### Return type

ApiResponse<[**ConnectWhatsAppCredentials200Response**](ConnectWhatsAppCredentials200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | WhatsApp connected successfully |  -  |
| **400** | Invalid request. Either missing fields or the phoneNumberId was not found in the specified WABA. If the phone was not found, the response includes availablePhoneNumbers to help identify the correct ID.  |  -  |
| **401** | Invalid or expired access token |  -  |
| **403** | Profile limit exceeded for this plan |  -  |


## getConnectUrl

> GetConnectUrl200Response getConnectUrl(platform, profileId, redirectUrl, headless)

Get OAuth connect URL

Initiate an OAuth connection flow. Returns an authUrl to redirect the user to. Standard flow: Zernio hosts the selection UI, then redirects to your redirect_url. Headless mode (headless&#x3D;true): user is redirected to your redirect_url with OAuth data for custom UI. Use the platform-specific selection endpoints to complete. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String platform = "facebook"; // String | Social media platform to connect
        String profileId = "profileId_example"; // String | Your Zernio profile ID (get from /v1/profiles)
        URI redirectUrl = new URI(); // URI | Your custom redirect URL after connection completes. Standard mode appends ?connected={platform}&profileId=X&accountId=Y&username=Z. Headless mode appends OAuth data params for platforms requiring selection (e.g. LinkedIn orgs, Facebook pages). If no selection is needed, the account is created directly and the redirect includes accountId.
        Boolean headless = false; // Boolean | When true, the user is redirected to your redirect_url with raw OAuth data (code, state) instead of Zernio's default account selection UI. Use this to build a custom connect experience.
        try {
            GetConnectUrl200Response result = apiInstance.getConnectUrl(platform, profileId, redirectUrl, headless);
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
| **platform** | **String**| Social media platform to connect | [enum: facebook, instagram, linkedin, twitter, tiktok, youtube, threads, reddit, pinterest, bluesky, googlebusiness, telegram, snapchat, discord] |
| **profileId** | **String**| Your Zernio profile ID (get from /v1/profiles) | |
| **redirectUrl** | **URI**| Your custom redirect URL after connection completes. Standard mode appends ?connected&#x3D;{platform}&amp;profileId&#x3D;X&amp;accountId&#x3D;Y&amp;username&#x3D;Z. Headless mode appends OAuth data params for platforms requiring selection (e.g. LinkedIn orgs, Facebook pages). If no selection is needed, the account is created directly and the redirect includes accountId. | [optional] |
| **headless** | **Boolean**| When true, the user is redirected to your redirect_url with raw OAuth data (code, state) instead of Zernio&#39;s default account selection UI. Use this to build a custom connect experience. | [optional] [default to false] |

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
| **402** | Payment method or enterprise contract required. The authenticated account hit a billing gate before the connection could proceed. Three reasons:    - &#x60;free_tier_exceeded&#x60;: the team has connected more accounts     than the free tier allows. Add a payment method on the     dashboard to continue (the user will be billed per     additional connected account).    - &#x60;twitter_passthrough&#x60;: connecting an X (Twitter) account     requires a card on file from day one because X API calls     incur real per-call pass-through costs. Applies to the 1st     X account, not just the 3rd+.    - &#x60;enterprise_required&#x60;: the team has reached the public     pricing ceiling (2,000 connected accounts). Beyond that     requires a custom enterprise contract negotiated directly.     &#x60;dashboard_url&#x60; deep-links to the enterprise contact page     rather than the billing tab. The end-user already has a     card on file; this gate is about contract terms, not card     collection.  SDK consumers should switch on &#x60;reason&#x60; to render the right prompt. For &#x60;free_tier_exceeded&#x60; and &#x60;twitter_passthrough&#x60;, redirect the end-user to &#x60;dashboard_url&#x60; to add a payment method via Zernio&#39;s hosted Stripe Setup Checkout. For &#x60;enterprise_required&#x60;, redirect to &#x60;dashboard_url&#x60; (the enterprise contact form) so they can talk to sales.  |  -  |
| **403** | No access to profile, or BYOK required for AppSumo Twitter |  -  |
| **404** | Profile not found |  -  |

## getConnectUrlWithHttpInfo

> ApiResponse<GetConnectUrl200Response> getConnectUrl getConnectUrlWithHttpInfo(platform, profileId, redirectUrl, headless)

Get OAuth connect URL

Initiate an OAuth connection flow. Returns an authUrl to redirect the user to. Standard flow: Zernio hosts the selection UI, then redirects to your redirect_url. Headless mode (headless&#x3D;true): user is redirected to your redirect_url with OAuth data for custom UI. Use the platform-specific selection endpoints to complete. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String platform = "facebook"; // String | Social media platform to connect
        String profileId = "profileId_example"; // String | Your Zernio profile ID (get from /v1/profiles)
        URI redirectUrl = new URI(); // URI | Your custom redirect URL after connection completes. Standard mode appends ?connected={platform}&profileId=X&accountId=Y&username=Z. Headless mode appends OAuth data params for platforms requiring selection (e.g. LinkedIn orgs, Facebook pages). If no selection is needed, the account is created directly and the redirect includes accountId.
        Boolean headless = false; // Boolean | When true, the user is redirected to your redirect_url with raw OAuth data (code, state) instead of Zernio's default account selection UI. Use this to build a custom connect experience.
        try {
            ApiResponse<GetConnectUrl200Response> response = apiInstance.getConnectUrlWithHttpInfo(platform, profileId, redirectUrl, headless);
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
| **platform** | **String**| Social media platform to connect | [enum: facebook, instagram, linkedin, twitter, tiktok, youtube, threads, reddit, pinterest, bluesky, googlebusiness, telegram, snapchat, discord] |
| **profileId** | **String**| Your Zernio profile ID (get from /v1/profiles) | |
| **redirectUrl** | **URI**| Your custom redirect URL after connection completes. Standard mode appends ?connected&#x3D;{platform}&amp;profileId&#x3D;X&amp;accountId&#x3D;Y&amp;username&#x3D;Z. Headless mode appends OAuth data params for platforms requiring selection (e.g. LinkedIn orgs, Facebook pages). If no selection is needed, the account is created directly and the redirect includes accountId. | [optional] |
| **headless** | **Boolean**| When true, the user is redirected to your redirect_url with raw OAuth data (code, state) instead of Zernio&#39;s default account selection UI. Use this to build a custom connect experience. | [optional] [default to false] |

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
| **402** | Payment method or enterprise contract required. The authenticated account hit a billing gate before the connection could proceed. Three reasons:    - &#x60;free_tier_exceeded&#x60;: the team has connected more accounts     than the free tier allows. Add a payment method on the     dashboard to continue (the user will be billed per     additional connected account).    - &#x60;twitter_passthrough&#x60;: connecting an X (Twitter) account     requires a card on file from day one because X API calls     incur real per-call pass-through costs. Applies to the 1st     X account, not just the 3rd+.    - &#x60;enterprise_required&#x60;: the team has reached the public     pricing ceiling (2,000 connected accounts). Beyond that     requires a custom enterprise contract negotiated directly.     &#x60;dashboard_url&#x60; deep-links to the enterprise contact page     rather than the billing tab. The end-user already has a     card on file; this gate is about contract terms, not card     collection.  SDK consumers should switch on &#x60;reason&#x60; to render the right prompt. For &#x60;free_tier_exceeded&#x60; and &#x60;twitter_passthrough&#x60;, redirect the end-user to &#x60;dashboard_url&#x60; to add a payment method via Zernio&#39;s hosted Stripe Setup Checkout. For &#x60;enterprise_required&#x60;, redirect to &#x60;dashboard_url&#x60; (the enterprise contact form) so they can talk to sales.  |  -  |
| **403** | No access to profile, or BYOK required for AppSumo Twitter |  -  |
| **404** | Profile not found |  -  |


## getFacebookPages

> GetFacebookPages200Response getFacebookPages(accountId)

List Facebook pages

Returns all Facebook pages the connected account has access to, including the currently selected page.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

List GBP locations

Returns all Google Business Profile locations the connected account has access to, including the currently selected location.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

List GBP locations

Returns all Google Business Profile locations the connected account has access to, including the currently selected location.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Returns LinkedIn organizations (company pages) the connected account has admin access to.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Returns LinkedIn organizations (company pages) the connected account has admin access to.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Fetch pending OAuth data for headless mode using the pendingDataToken from the redirect URL.  **Scope**: This endpoint is used only for LinkedIn organizations and Snapchat profiles, where the selection list is too large to fit in URL params. WhatsApp, Facebook, Pinterest, Google Business and other platforms pass selection state directly via URL query params on the redirect (&#x60;profileId&#x60;, &#x60;tempToken&#x60;, &#x60;step&#x60;), no pending record is created, so this endpoint will return 404 for those flows. Use the platform-specific selection endpoint instead (e.g. &#x60;/v1/connect/whatsapp/select-phone-number&#x60;).  Token is one-time use and expires after 10 minutes. No authentication required. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String token = "token_example"; // String | The pending data token from the OAuth redirect URL (pendingDataToken parameter)
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
| **token** | **String**| The pending data token from the OAuth redirect URL (pendingDataToken parameter) | |

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

Fetch pending OAuth data for headless mode using the pendingDataToken from the redirect URL.  **Scope**: This endpoint is used only for LinkedIn organizations and Snapchat profiles, where the selection list is too large to fit in URL params. WhatsApp, Facebook, Pinterest, Google Business and other platforms pass selection state directly via URL query params on the redirect (&#x60;profileId&#x60;, &#x60;tempToken&#x60;, &#x60;step&#x60;), no pending record is created, so this endpoint will return 404 for those flows. Use the platform-specific selection endpoint instead (e.g. &#x60;/v1/connect/whatsapp/select-phone-number&#x60;).  Token is one-time use and expires after 10 minutes. No authentication required. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String token = "token_example"; // String | The pending data token from the OAuth redirect URL (pendingDataToken parameter)
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
| **token** | **String**| The pending data token from the OAuth redirect URL (pendingDataToken parameter) | |

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

Returns the boards available for a connected Pinterest account. Use this to get a board ID when creating a Pinterest post.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Returns the boards available for a connected Pinterest account. Use this to get a board ID when creating a Pinterest post.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Returns available post flairs for a subreddit. Some subreddits require a flair when posting.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Returns available post flairs for a subreddit. Some subreddits require a flair when posting.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Returns the subreddits the connected Reddit account can post to. Use this to get a subreddit name when creating a Reddit post.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Returns the subreddits the connected Reddit account can post to. Use this to get a subreddit name when creating a Reddit post.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Generate an access code (valid 15 minutes) for connecting a Telegram channel or group. Add the bot as admin, then send the code + @yourchannel to the bot. Poll PATCH /v1/connect/telegram to check status.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Generate an access code (valid 15 minutes) for connecting a Telegram channel or group. Add the bot as admin, then send the code + @yourchannel to the bot. Poll PATCH /v1/connect/telegram to check status.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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


## getYoutubePlaylists

> GetYoutubePlaylists200Response getYoutubePlaylists(accountId)

List YouTube playlists

Returns the playlists available for a connected YouTube account. Use this to get a playlist ID when creating a YouTube post with the playlistId field.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        try {
            GetYoutubePlaylists200Response result = apiInstance.getYoutubePlaylists(accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#getYoutubePlaylists");
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

[**GetYoutubePlaylists200Response**](GetYoutubePlaylists200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Playlists list |  -  |
| **400** | Not a YouTube account |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## getYoutubePlaylistsWithHttpInfo

> ApiResponse<GetYoutubePlaylists200Response> getYoutubePlaylists getYoutubePlaylistsWithHttpInfo(accountId)

List YouTube playlists

Returns the playlists available for a connected YouTube account. Use this to get a playlist ID when creating a YouTube post with the playlistId field.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        try {
            ApiResponse<GetYoutubePlaylists200Response> response = apiInstance.getYoutubePlaylistsWithHttpInfo(accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#getYoutubePlaylists");
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

ApiResponse<[**GetYoutubePlaylists200Response**](GetYoutubePlaylists200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Playlists list |  -  |
| **400** | Not a YouTube account |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |


## handleOAuthCallback

> void handleOAuthCallback(platform, handleOAuthCallbackRequest)

Complete OAuth callback

Exchange the OAuth authorization code for tokens and connect the account to the specified profile.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Exchange the OAuth authorization code for tokens and connect the account to the specified profile.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Connect a Telegram channel/group directly using the chat ID. Alternative to the access code flow. The bot must already be an admin in the channel/group.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Connect a Telegram channel/group directly using the chat ID. Alternative to the access code flow. The bot must already be an admin in the channel/group.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Returns the list of Facebook Pages the user can manage after OAuth. Extract tempToken and userProfile from the OAuth redirect params and pass them here. Use the X-Connect-Token header if connecting via API key.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Returns the list of Facebook Pages the user can manage after OAuth. Extract tempToken and userProfile from the OAuth redirect params and pass them here. Use the X-Connect-Token header if connecting via API key.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

> ListGoogleBusinessLocations200Response listGoogleBusinessLocations(profileId, pendingDataToken, tempToken)

List GBP locations

For headless flows. Returns the list of GBP locations the user can manage. Use pendingDataToken (from the OAuth callback redirect) to list locations without consuming the token, so it remains available for select-location. Use X-Connect-Token header if connecting via API key. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure API key authorization: connectToken
        ApiKeyAuth connectToken = (ApiKeyAuth) defaultClient.getAuthentication("connectToken");
        connectToken.setApiKey("YOUR API KEY");
        // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
        //connectToken.setApiKeyPrefix("Token");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String profileId = "profileId_example"; // String | Profile ID from your connection flow. Required for auth validation when provided.
        String pendingDataToken = "pendingDataToken_example"; // String | Token from the OAuth callback redirect. Preferred over tempToken because it preserves server-side token storage. One of pendingDataToken or tempToken is required.
        String tempToken = "tempToken_example"; // String | Legacy. Direct Google access token. Use pendingDataToken instead when available.
        try {
            ListGoogleBusinessLocations200Response result = apiInstance.listGoogleBusinessLocations(profileId, pendingDataToken, tempToken);
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
| **profileId** | **String**| Profile ID from your connection flow. Required for auth validation when provided. | [optional] |
| **pendingDataToken** | **String**| Token from the OAuth callback redirect. Preferred over tempToken because it preserves server-side token storage. One of pendingDataToken or tempToken is required. | [optional] |
| **tempToken** | **String**| Legacy. Direct Google access token. Use pendingDataToken instead when available. | [optional] |

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

> ApiResponse<ListGoogleBusinessLocations200Response> listGoogleBusinessLocations listGoogleBusinessLocationsWithHttpInfo(profileId, pendingDataToken, tempToken)

List GBP locations

For headless flows. Returns the list of GBP locations the user can manage. Use pendingDataToken (from the OAuth callback redirect) to list locations without consuming the token, so it remains available for select-location. Use X-Connect-Token header if connecting via API key. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure API key authorization: connectToken
        ApiKeyAuth connectToken = (ApiKeyAuth) defaultClient.getAuthentication("connectToken");
        connectToken.setApiKey("YOUR API KEY");
        // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
        //connectToken.setApiKeyPrefix("Token");

        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String profileId = "profileId_example"; // String | Profile ID from your connection flow. Required for auth validation when provided.
        String pendingDataToken = "pendingDataToken_example"; // String | Token from the OAuth callback redirect. Preferred over tempToken because it preserves server-side token storage. One of pendingDataToken or tempToken is required.
        String tempToken = "tempToken_example"; // String | Legacy. Direct Google access token. Use pendingDataToken instead when available.
        try {
            ApiResponse<ListGoogleBusinessLocations200Response> response = apiInstance.listGoogleBusinessLocationsWithHttpInfo(profileId, pendingDataToken, tempToken);
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
| **profileId** | **String**| Profile ID from your connection flow. Required for auth validation when provided. | [optional] |
| **pendingDataToken** | **String**| Token from the OAuth callback redirect. Preferred over tempToken because it preserves server-side token storage. One of pendingDataToken or tempToken is required. | [optional] |
| **tempToken** | **String**| Legacy. Direct Google access token. Use pendingDataToken instead when available. | [optional] |

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

Fetch full LinkedIn organization details (logos, vanity names, websites) for custom UI. No authentication required, just the tempToken from OAuth.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Fetch full LinkedIn organization details (logos, vanity names, websites) for custom UI. No authentication required, just the tempToken from OAuth.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

For headless flows. Returns Pinterest boards the user can post to. Use X-Connect-Token from the redirect URL.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String xConnectToken = "xConnectToken_example"; // String | Short-lived connect token from the OAuth redirect
        String profileId = "profileId_example"; // String | Your Zernio profile ID
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
| **profileId** | **String**| Your Zernio profile ID | |
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

For headless flows. Returns Pinterest boards the user can post to. Use X-Connect-Token from the redirect URL.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String xConnectToken = "xConnectToken_example"; // String | Short-lived connect token from the OAuth redirect
        String profileId = "profileId_example"; // String | Your Zernio profile ID
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
| **profileId** | **String**| Your Zernio profile ID | |
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

For headless flows. Returns Snapchat Public Profiles the user can post to. Use X-Connect-Token from the redirect URL.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String xConnectToken = "xConnectToken_example"; // String | Short-lived connect token from the OAuth redirect
        String profileId = "profileId_example"; // String | Your Zernio profile ID
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
| **profileId** | **String**| Your Zernio profile ID | |
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

For headless flows. Returns Snapchat Public Profiles the user can post to. Use X-Connect-Token from the redirect URL.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String xConnectToken = "xConnectToken_example"; // String | Short-lived connect token from the OAuth redirect
        String profileId = "profileId_example"; // String | Your Zernio profile ID
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
| **profileId** | **String**| Your Zernio profile ID | |
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


## listWhatsAppPhoneNumbers

> ListWhatsAppPhoneNumbers200Response listWhatsAppPhoneNumbers(profileId, tempToken, xConnectToken)

List WhatsApp phone numbers for selection

Fetch the WhatsApp phone numbers available across the user&#39;s WhatsApp Business Accounts (WABAs) after a headless OAuth flow.  WhatsApp OAuth grants access at the WABA level. When a connected WABA has 2 or more phone numbers, you must call this endpoint to list them and then &#x60;POST /v1/connect/whatsapp/select-phone-number&#x60; to bind one to the Zernio profile. Single-phone WABAs auto-complete during the OAuth callback and never reach this endpoint.  Use the &#x60;profileId&#x60; and &#x60;tempToken&#x60; returned in the headless redirect (&#x60;step&#x3D;select_phone_number&#x60;).  Alternative: if you already know &#x60;wabaId&#x60; and &#x60;phoneNumberId&#x60; (e.g. from Meta Business Suite), use &#x60;connectWhatsAppCredentials&#x60; instead, which skips this two-step flow. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String profileId = "profileId_example"; // String | The Zernio profile ID from the headless redirect
        String tempToken = "tempToken_example"; // String | The temporary access token from the headless redirect
        String xConnectToken = "xConnectToken_example"; // String | Alternative auth for API users' end customers (used when the bearer token is scoped to a different user)
        try {
            ListWhatsAppPhoneNumbers200Response result = apiInstance.listWhatsAppPhoneNumbers(profileId, tempToken, xConnectToken);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#listWhatsAppPhoneNumbers");
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
| **profileId** | **String**| The Zernio profile ID from the headless redirect | |
| **tempToken** | **String**| The temporary access token from the headless redirect | |
| **xConnectToken** | **String**| Alternative auth for API users&#39; end customers (used when the bearer token is scoped to a different user) | [optional] |

### Return type

[**ListWhatsAppPhoneNumbers200Response**](ListWhatsAppPhoneNumbers200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Phone numbers fetched successfully |  -  |
| **400** | Missing profileId or tempToken |  -  |
| **401** | Unauthorized |  -  |
| **500** | Failed to fetch phone numbers (Meta API error, expired token, or insufficient permissions) |  -  |

## listWhatsAppPhoneNumbersWithHttpInfo

> ApiResponse<ListWhatsAppPhoneNumbers200Response> listWhatsAppPhoneNumbers listWhatsAppPhoneNumbersWithHttpInfo(profileId, tempToken, xConnectToken)

List WhatsApp phone numbers for selection

Fetch the WhatsApp phone numbers available across the user&#39;s WhatsApp Business Accounts (WABAs) after a headless OAuth flow.  WhatsApp OAuth grants access at the WABA level. When a connected WABA has 2 or more phone numbers, you must call this endpoint to list them and then &#x60;POST /v1/connect/whatsapp/select-phone-number&#x60; to bind one to the Zernio profile. Single-phone WABAs auto-complete during the OAuth callback and never reach this endpoint.  Use the &#x60;profileId&#x60; and &#x60;tempToken&#x60; returned in the headless redirect (&#x60;step&#x3D;select_phone_number&#x60;).  Alternative: if you already know &#x60;wabaId&#x60; and &#x60;phoneNumberId&#x60; (e.g. from Meta Business Suite), use &#x60;connectWhatsAppCredentials&#x60; instead, which skips this two-step flow. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String profileId = "profileId_example"; // String | The Zernio profile ID from the headless redirect
        String tempToken = "tempToken_example"; // String | The temporary access token from the headless redirect
        String xConnectToken = "xConnectToken_example"; // String | Alternative auth for API users' end customers (used when the bearer token is scoped to a different user)
        try {
            ApiResponse<ListWhatsAppPhoneNumbers200Response> response = apiInstance.listWhatsAppPhoneNumbersWithHttpInfo(profileId, tempToken, xConnectToken);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#listWhatsAppPhoneNumbers");
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
| **profileId** | **String**| The Zernio profile ID from the headless redirect | |
| **tempToken** | **String**| The temporary access token from the headless redirect | |
| **xConnectToken** | **String**| Alternative auth for API users&#39; end customers (used when the bearer token is scoped to a different user) | [optional] |

### Return type

ApiResponse<[**ListWhatsAppPhoneNumbers200Response**](ListWhatsAppPhoneNumbers200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Phone numbers fetched successfully |  -  |
| **400** | Missing profileId or tempToken |  -  |
| **401** | Unauthorized |  -  |
| **500** | Failed to fetch phone numbers (Meta API error, expired token, or insufficient permissions) |  -  |


## selectFacebookPage

> SelectFacebookPage200Response selectFacebookPage(selectFacebookPageRequest)

Select Facebook page

Complete the headless flow by saving the user&#39;s selected Facebook page. Pass the userProfile from the OAuth redirect and use X-Connect-Token if connecting via API key.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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
| **400** | Missing required fields (profileId, pageId, tempToken, or userProfile) |  -  |
| **401** | Unauthorized |  -  |
| **403** | User does not have access to the specified profile |  -  |
| **404** | Selected page not found in available pages |  -  |
| **500** | Failed to save Facebook connection |  -  |

## selectFacebookPageWithHttpInfo

> ApiResponse<SelectFacebookPage200Response> selectFacebookPage selectFacebookPageWithHttpInfo(selectFacebookPageRequest)

Select Facebook page

Complete the headless flow by saving the user&#39;s selected Facebook page. Pass the userProfile from the OAuth redirect and use X-Connect-Token if connecting via API key.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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
| **400** | Missing required fields (profileId, pageId, tempToken, or userProfile) |  -  |
| **401** | Unauthorized |  -  |
| **403** | User does not have access to the specified profile |  -  |
| **404** | Selected page not found in available pages |  -  |
| **500** | Failed to save Facebook connection |  -  |


## selectGoogleBusinessLocation

> SelectGoogleBusinessLocation200Response selectGoogleBusinessLocation(selectGoogleBusinessLocationRequest)

Select GBP location

Complete the headless GBP flow by saving the user&#39;s selected location. The pendingDataToken is returned in your redirect URL after OAuth completes (step&#x3D;select_location). Tokens and profile data are stored server-side, so only the pendingDataToken is needed here. Use X-Connect-Token header if connecting via API key. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Select GBP location

Complete the headless GBP flow by saving the user&#39;s selected location. The pendingDataToken is returned in your redirect URL after OAuth completes (step&#x3D;select_location). Tokens and profile data are stored server-side, so only the pendingDataToken is needed here. Use X-Connect-Token header if connecting via API key. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Complete the LinkedIn connection flow. Set accountType to \&quot;personal\&quot; or \&quot;organization\&quot; to connect as a company page. Use X-Connect-Token if connecting via API key.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Complete the LinkedIn connection flow. Set accountType to \&quot;personal\&quot; or \&quot;organization\&quot; to connect as a company page. Use X-Connect-Token if connecting via API key.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Complete the Pinterest connection flow. After OAuth, use this endpoint to save the selected board and complete the account connection. Use the X-Connect-Token header if you initiated the connection via API key. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Complete the Pinterest connection flow. After OAuth, use this endpoint to save the selected board and complete the account connection. Use the X-Connect-Token header if you initiated the connection via API key. 

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Complete the Snapchat connection flow by saving the selected Public Profile. Snapchat requires a Public Profile to publish content. Use X-Connect-Token if connecting via API key.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Complete the Snapchat connection flow by saving the selected Public Profile. Snapchat requires a Public Profile to publish content. Use X-Connect-Token if connecting via API key.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Switch which Facebook Page is active for a connected account.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Switch which Facebook Page is active for a connected account.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Update GBP location

Switch which GBP location is active for a connected account.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Update GBP location

Switch which GBP location is active for a connected account.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Switch a LinkedIn account between personal profile and organization (company page) posting.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Switch a LinkedIn account between personal profile and organization (company page) posting.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Sets the default board used when publishing pins for this account.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

Sets the default board used when publishing pins for this account.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
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

> UpdateYoutubeDefaultPlaylist200Response updateRedditSubreddits(accountId, updateRedditSubredditsRequest)

Set default subreddit

Sets the default subreddit used when publishing posts for this Reddit account.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        UpdateRedditSubredditsRequest updateRedditSubredditsRequest = new UpdateRedditSubredditsRequest(); // UpdateRedditSubredditsRequest | 
        try {
            UpdateYoutubeDefaultPlaylist200Response result = apiInstance.updateRedditSubreddits(accountId, updateRedditSubredditsRequest);
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

[**UpdateYoutubeDefaultPlaylist200Response**](UpdateYoutubeDefaultPlaylist200Response.md)


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

> ApiResponse<UpdateYoutubeDefaultPlaylist200Response> updateRedditSubreddits updateRedditSubredditsWithHttpInfo(accountId, updateRedditSubredditsRequest)

Set default subreddit

Sets the default subreddit used when publishing posts for this Reddit account.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        UpdateRedditSubredditsRequest updateRedditSubredditsRequest = new UpdateRedditSubredditsRequest(); // UpdateRedditSubredditsRequest | 
        try {
            ApiResponse<UpdateYoutubeDefaultPlaylist200Response> response = apiInstance.updateRedditSubredditsWithHttpInfo(accountId, updateRedditSubredditsRequest);
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

ApiResponse<[**UpdateYoutubeDefaultPlaylist200Response**](UpdateYoutubeDefaultPlaylist200Response.md)>


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


## updateYoutubeDefaultPlaylist

> UpdateYoutubeDefaultPlaylist200Response updateYoutubeDefaultPlaylist(accountId, updateYoutubeDefaultPlaylistRequest)

Set default YouTube playlist

Sets the default playlist used when publishing videos for this account. When a post does not specify a playlistId, the default playlist is not automatically used (it is stored for client-side convenience).

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        UpdateYoutubeDefaultPlaylistRequest updateYoutubeDefaultPlaylistRequest = new UpdateYoutubeDefaultPlaylistRequest(); // UpdateYoutubeDefaultPlaylistRequest | 
        try {
            UpdateYoutubeDefaultPlaylist200Response result = apiInstance.updateYoutubeDefaultPlaylist(accountId, updateYoutubeDefaultPlaylistRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#updateYoutubeDefaultPlaylist");
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
| **updateYoutubeDefaultPlaylistRequest** | [**UpdateYoutubeDefaultPlaylistRequest**](UpdateYoutubeDefaultPlaylistRequest.md)|  | |

### Return type

[**UpdateYoutubeDefaultPlaylist200Response**](UpdateYoutubeDefaultPlaylist200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default playlist set |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## updateYoutubeDefaultPlaylistWithHttpInfo

> ApiResponse<UpdateYoutubeDefaultPlaylist200Response> updateYoutubeDefaultPlaylist updateYoutubeDefaultPlaylistWithHttpInfo(accountId, updateYoutubeDefaultPlaylistRequest)

Set default YouTube playlist

Sets the default playlist used when publishing videos for this account. When a post does not specify a playlistId, the default playlist is not automatically used (it is stored for client-side convenience).

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.ConnectApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ConnectApi apiInstance = new ConnectApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        UpdateYoutubeDefaultPlaylistRequest updateYoutubeDefaultPlaylistRequest = new UpdateYoutubeDefaultPlaylistRequest(); // UpdateYoutubeDefaultPlaylistRequest | 
        try {
            ApiResponse<UpdateYoutubeDefaultPlaylist200Response> response = apiInstance.updateYoutubeDefaultPlaylistWithHttpInfo(accountId, updateYoutubeDefaultPlaylistRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ConnectApi#updateYoutubeDefaultPlaylist");
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
| **updateYoutubeDefaultPlaylistRequest** | [**UpdateYoutubeDefaultPlaylistRequest**](UpdateYoutubeDefaultPlaylistRequest.md)|  | |

### Return type

ApiResponse<[**UpdateYoutubeDefaultPlaylist200Response**](UpdateYoutubeDefaultPlaylist200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Default playlist set |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

