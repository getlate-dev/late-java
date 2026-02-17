# ToolsApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**checkInstagramHashtags**](ToolsApi.md#checkInstagramHashtags) | **POST** /v1/tools/instagram/hashtag-checker | Check Instagram hashtag bans |
| [**checkInstagramHashtagsWithHttpInfo**](ToolsApi.md#checkInstagramHashtagsWithHttpInfo) | **POST** /v1/tools/instagram/hashtag-checker | Check Instagram hashtag bans |
| [**downloadBlueskyMedia**](ToolsApi.md#downloadBlueskyMedia) | **GET** /v1/tools/bluesky/download | Download Bluesky media |
| [**downloadBlueskyMediaWithHttpInfo**](ToolsApi.md#downloadBlueskyMediaWithHttpInfo) | **GET** /v1/tools/bluesky/download | Download Bluesky media |
| [**downloadFacebookVideo**](ToolsApi.md#downloadFacebookVideo) | **GET** /v1/tools/facebook/download | Download Facebook video |
| [**downloadFacebookVideoWithHttpInfo**](ToolsApi.md#downloadFacebookVideoWithHttpInfo) | **GET** /v1/tools/facebook/download | Download Facebook video |
| [**downloadInstagramMedia**](ToolsApi.md#downloadInstagramMedia) | **GET** /v1/tools/instagram/download | Download Instagram media |
| [**downloadInstagramMediaWithHttpInfo**](ToolsApi.md#downloadInstagramMediaWithHttpInfo) | **GET** /v1/tools/instagram/download | Download Instagram media |
| [**downloadLinkedInVideo**](ToolsApi.md#downloadLinkedInVideo) | **GET** /v1/tools/linkedin/download | Download LinkedIn video |
| [**downloadLinkedInVideoWithHttpInfo**](ToolsApi.md#downloadLinkedInVideoWithHttpInfo) | **GET** /v1/tools/linkedin/download | Download LinkedIn video |
| [**downloadTikTokVideo**](ToolsApi.md#downloadTikTokVideo) | **GET** /v1/tools/tiktok/download | Download TikTok video |
| [**downloadTikTokVideoWithHttpInfo**](ToolsApi.md#downloadTikTokVideoWithHttpInfo) | **GET** /v1/tools/tiktok/download | Download TikTok video |
| [**downloadTwitterMedia**](ToolsApi.md#downloadTwitterMedia) | **GET** /v1/tools/twitter/download | Download Twitter/X media |
| [**downloadTwitterMediaWithHttpInfo**](ToolsApi.md#downloadTwitterMediaWithHttpInfo) | **GET** /v1/tools/twitter/download | Download Twitter/X media |
| [**downloadYouTubeVideo**](ToolsApi.md#downloadYouTubeVideo) | **GET** /v1/tools/youtube/download | Download YouTube video |
| [**downloadYouTubeVideoWithHttpInfo**](ToolsApi.md#downloadYouTubeVideoWithHttpInfo) | **GET** /v1/tools/youtube/download | Download YouTube video |
| [**getYouTubeTranscript**](ToolsApi.md#getYouTubeTranscript) | **GET** /v1/tools/youtube/transcript | Get YouTube transcript |
| [**getYouTubeTranscriptWithHttpInfo**](ToolsApi.md#getYouTubeTranscriptWithHttpInfo) | **GET** /v1/tools/youtube/transcript | Get YouTube transcript |



## checkInstagramHashtags

> CheckInstagramHashtags200Response checkInstagramHashtags(checkInstagramHashtagsRequest)

Check Instagram hashtag bans

Check if Instagram hashtags are banned, restricted, or safe to use.  **Rate Limits:** Build (50/day), Accelerate (500/day), Unlimited (unlimited) 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ToolsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ToolsApi apiInstance = new ToolsApi(defaultClient);
        CheckInstagramHashtagsRequest checkInstagramHashtagsRequest = new CheckInstagramHashtagsRequest(); // CheckInstagramHashtagsRequest | 
        try {
            CheckInstagramHashtags200Response result = apiInstance.checkInstagramHashtags(checkInstagramHashtagsRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ToolsApi#checkInstagramHashtags");
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
| **checkInstagramHashtagsRequest** | [**CheckInstagramHashtagsRequest**](CheckInstagramHashtagsRequest.md)|  | |

### Return type

[**CheckInstagramHashtags200Response**](CheckInstagramHashtags200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |

## checkInstagramHashtagsWithHttpInfo

> ApiResponse<CheckInstagramHashtags200Response> checkInstagramHashtags checkInstagramHashtagsWithHttpInfo(checkInstagramHashtagsRequest)

Check Instagram hashtag bans

Check if Instagram hashtags are banned, restricted, or safe to use.  **Rate Limits:** Build (50/day), Accelerate (500/day), Unlimited (unlimited) 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ToolsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ToolsApi apiInstance = new ToolsApi(defaultClient);
        CheckInstagramHashtagsRequest checkInstagramHashtagsRequest = new CheckInstagramHashtagsRequest(); // CheckInstagramHashtagsRequest | 
        try {
            ApiResponse<CheckInstagramHashtags200Response> response = apiInstance.checkInstagramHashtagsWithHttpInfo(checkInstagramHashtagsRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ToolsApi#checkInstagramHashtags");
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
| **checkInstagramHashtagsRequest** | [**CheckInstagramHashtagsRequest**](CheckInstagramHashtagsRequest.md)|  | |

### Return type

ApiResponse<[**CheckInstagramHashtags200Response**](CheckInstagramHashtags200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |


## downloadBlueskyMedia

> DownloadBlueskyMedia200Response downloadBlueskyMedia(url)

Download Bluesky media

Download videos from Bluesky posts.  **Rate Limits:** Build (50/day), Accelerate (500/day), Unlimited (unlimited) 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ToolsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ToolsApi apiInstance = new ToolsApi(defaultClient);
        String url = "https://bsky.app/profile/user.bsky.social/post/abc123"; // String | Bluesky post URL
        try {
            DownloadBlueskyMedia200Response result = apiInstance.downloadBlueskyMedia(url);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ToolsApi#downloadBlueskyMedia");
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
| **url** | **String**| Bluesky post URL | |

### Return type

[**DownloadBlueskyMedia200Response**](DownloadBlueskyMedia200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |

## downloadBlueskyMediaWithHttpInfo

> ApiResponse<DownloadBlueskyMedia200Response> downloadBlueskyMedia downloadBlueskyMediaWithHttpInfo(url)

Download Bluesky media

Download videos from Bluesky posts.  **Rate Limits:** Build (50/day), Accelerate (500/day), Unlimited (unlimited) 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ToolsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ToolsApi apiInstance = new ToolsApi(defaultClient);
        String url = "https://bsky.app/profile/user.bsky.social/post/abc123"; // String | Bluesky post URL
        try {
            ApiResponse<DownloadBlueskyMedia200Response> response = apiInstance.downloadBlueskyMediaWithHttpInfo(url);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ToolsApi#downloadBlueskyMedia");
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
| **url** | **String**| Bluesky post URL | |

### Return type

ApiResponse<[**DownloadBlueskyMedia200Response**](DownloadBlueskyMedia200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |


## downloadFacebookVideo

> DownloadFacebookVideo200Response downloadFacebookVideo(url)

Download Facebook video

Download videos and reels from Facebook.  **Rate Limits:** Build (50/day), Accelerate (500/day), Unlimited (unlimited) 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ToolsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ToolsApi apiInstance = new ToolsApi(defaultClient);
        String url = "url_example"; // String | Facebook video or reel URL
        try {
            DownloadFacebookVideo200Response result = apiInstance.downloadFacebookVideo(url);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ToolsApi#downloadFacebookVideo");
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
| **url** | **String**| Facebook video or reel URL | |

### Return type

[**DownloadFacebookVideo200Response**](DownloadFacebookVideo200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |

## downloadFacebookVideoWithHttpInfo

> ApiResponse<DownloadFacebookVideo200Response> downloadFacebookVideo downloadFacebookVideoWithHttpInfo(url)

Download Facebook video

Download videos and reels from Facebook.  **Rate Limits:** Build (50/day), Accelerate (500/day), Unlimited (unlimited) 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ToolsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ToolsApi apiInstance = new ToolsApi(defaultClient);
        String url = "url_example"; // String | Facebook video or reel URL
        try {
            ApiResponse<DownloadFacebookVideo200Response> response = apiInstance.downloadFacebookVideoWithHttpInfo(url);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ToolsApi#downloadFacebookVideo");
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
| **url** | **String**| Facebook video or reel URL | |

### Return type

ApiResponse<[**DownloadFacebookVideo200Response**](DownloadFacebookVideo200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |


## downloadInstagramMedia

> DownloadInstagramMedia200Response downloadInstagramMedia(url)

Download Instagram media

Download Instagram reels, posts, or photos.  **Rate Limits:** Build (50/day), Accelerate (500/day), Unlimited (unlimited) 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ToolsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ToolsApi apiInstance = new ToolsApi(defaultClient);
        String url = "https://www.instagram.com/reel/ABC123/"; // String | Instagram reel or post URL
        try {
            DownloadInstagramMedia200Response result = apiInstance.downloadInstagramMedia(url);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ToolsApi#downloadInstagramMedia");
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
| **url** | **String**| Instagram reel or post URL | |

### Return type

[**DownloadInstagramMedia200Response**](DownloadInstagramMedia200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |

## downloadInstagramMediaWithHttpInfo

> ApiResponse<DownloadInstagramMedia200Response> downloadInstagramMedia downloadInstagramMediaWithHttpInfo(url)

Download Instagram media

Download Instagram reels, posts, or photos.  **Rate Limits:** Build (50/day), Accelerate (500/day), Unlimited (unlimited) 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ToolsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ToolsApi apiInstance = new ToolsApi(defaultClient);
        String url = "https://www.instagram.com/reel/ABC123/"; // String | Instagram reel or post URL
        try {
            ApiResponse<DownloadInstagramMedia200Response> response = apiInstance.downloadInstagramMediaWithHttpInfo(url);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ToolsApi#downloadInstagramMedia");
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
| **url** | **String**| Instagram reel or post URL | |

### Return type

ApiResponse<[**DownloadInstagramMedia200Response**](DownloadInstagramMedia200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |


## downloadLinkedInVideo

> DownloadInstagramMedia200Response downloadLinkedInVideo(url)

Download LinkedIn video

Download videos from LinkedIn posts.  **Rate Limits:** Build (50/day), Accelerate (500/day), Unlimited (unlimited) 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ToolsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ToolsApi apiInstance = new ToolsApi(defaultClient);
        String url = "url_example"; // String | LinkedIn post URL
        try {
            DownloadInstagramMedia200Response result = apiInstance.downloadLinkedInVideo(url);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ToolsApi#downloadLinkedInVideo");
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
| **url** | **String**| LinkedIn post URL | |

### Return type

[**DownloadInstagramMedia200Response**](DownloadInstagramMedia200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |

## downloadLinkedInVideoWithHttpInfo

> ApiResponse<DownloadInstagramMedia200Response> downloadLinkedInVideo downloadLinkedInVideoWithHttpInfo(url)

Download LinkedIn video

Download videos from LinkedIn posts.  **Rate Limits:** Build (50/day), Accelerate (500/day), Unlimited (unlimited) 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ToolsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ToolsApi apiInstance = new ToolsApi(defaultClient);
        String url = "url_example"; // String | LinkedIn post URL
        try {
            ApiResponse<DownloadInstagramMedia200Response> response = apiInstance.downloadLinkedInVideoWithHttpInfo(url);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ToolsApi#downloadLinkedInVideo");
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
| **url** | **String**| LinkedIn post URL | |

### Return type

ApiResponse<[**DownloadInstagramMedia200Response**](DownloadInstagramMedia200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |


## downloadTikTokVideo

> DownloadTikTokVideo200Response downloadTikTokVideo(url, action, formatId)

Download TikTok video

Download TikTok videos with or without watermark.  **Rate Limits:** Build (50/day), Accelerate (500/day), Unlimited (unlimited) 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ToolsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ToolsApi apiInstance = new ToolsApi(defaultClient);
        String url = "url_example"; // String | TikTok video URL or ID
        String action = "download"; // String | 'formats' to list available formats
        String formatId = "formatId_example"; // String | Specific format ID (0 = no watermark, etc.)
        try {
            DownloadTikTokVideo200Response result = apiInstance.downloadTikTokVideo(url, action, formatId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ToolsApi#downloadTikTokVideo");
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
| **url** | **String**| TikTok video URL or ID | |
| **action** | **String**| &#39;formats&#39; to list available formats | [optional] [default to download] [enum: download, formats] |
| **formatId** | **String**| Specific format ID (0 &#x3D; no watermark, etc.) | [optional] |

### Return type

[**DownloadTikTokVideo200Response**](DownloadTikTokVideo200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |

## downloadTikTokVideoWithHttpInfo

> ApiResponse<DownloadTikTokVideo200Response> downloadTikTokVideo downloadTikTokVideoWithHttpInfo(url, action, formatId)

Download TikTok video

Download TikTok videos with or without watermark.  **Rate Limits:** Build (50/day), Accelerate (500/day), Unlimited (unlimited) 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ToolsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ToolsApi apiInstance = new ToolsApi(defaultClient);
        String url = "url_example"; // String | TikTok video URL or ID
        String action = "download"; // String | 'formats' to list available formats
        String formatId = "formatId_example"; // String | Specific format ID (0 = no watermark, etc.)
        try {
            ApiResponse<DownloadTikTokVideo200Response> response = apiInstance.downloadTikTokVideoWithHttpInfo(url, action, formatId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ToolsApi#downloadTikTokVideo");
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
| **url** | **String**| TikTok video URL or ID | |
| **action** | **String**| &#39;formats&#39; to list available formats | [optional] [default to download] [enum: download, formats] |
| **formatId** | **String**| Specific format ID (0 &#x3D; no watermark, etc.) | [optional] |

### Return type

ApiResponse<[**DownloadTikTokVideo200Response**](DownloadTikTokVideo200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |


## downloadTwitterMedia

> DownloadInstagramMedia200Response downloadTwitterMedia(url, action, formatId)

Download Twitter/X media

Download videos from Twitter/X posts.  **Rate Limits:** Build (50/day), Accelerate (500/day), Unlimited (unlimited) 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ToolsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ToolsApi apiInstance = new ToolsApi(defaultClient);
        String url = "https://x.com/user/status/123456789"; // String | Twitter/X post URL
        String action = "download"; // String | 
        String formatId = "formatId_example"; // String | 
        try {
            DownloadInstagramMedia200Response result = apiInstance.downloadTwitterMedia(url, action, formatId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ToolsApi#downloadTwitterMedia");
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
| **url** | **String**| Twitter/X post URL | |
| **action** | **String**|  | [optional] [default to download] [enum: download, formats] |
| **formatId** | **String**|  | [optional] |

### Return type

[**DownloadInstagramMedia200Response**](DownloadInstagramMedia200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |

## downloadTwitterMediaWithHttpInfo

> ApiResponse<DownloadInstagramMedia200Response> downloadTwitterMedia downloadTwitterMediaWithHttpInfo(url, action, formatId)

Download Twitter/X media

Download videos from Twitter/X posts.  **Rate Limits:** Build (50/day), Accelerate (500/day), Unlimited (unlimited) 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ToolsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ToolsApi apiInstance = new ToolsApi(defaultClient);
        String url = "https://x.com/user/status/123456789"; // String | Twitter/X post URL
        String action = "download"; // String | 
        String formatId = "formatId_example"; // String | 
        try {
            ApiResponse<DownloadInstagramMedia200Response> response = apiInstance.downloadTwitterMediaWithHttpInfo(url, action, formatId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ToolsApi#downloadTwitterMedia");
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
| **url** | **String**| Twitter/X post URL | |
| **action** | **String**|  | [optional] [default to download] [enum: download, formats] |
| **formatId** | **String**|  | [optional] |

### Return type

ApiResponse<[**DownloadInstagramMedia200Response**](DownloadInstagramMedia200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |


## downloadYouTubeVideo

> DownloadYouTubeVideo200Response downloadYouTubeVideo(url, action, format, quality, formatId)

Download YouTube video

Download YouTube videos or audio. Returns available formats or direct download URL.  **Rate Limits:** Build (50/day), Accelerate (500/day), Unlimited (unlimited) 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ToolsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ToolsApi apiInstance = new ToolsApi(defaultClient);
        String url = "https://www.youtube.com/watch?v=dQw4w9WgXcQ"; // String | YouTube video URL or video ID
        String action = "download"; // String | Action to perform: 'download' returns download URL, 'formats' lists available formats
        String format = "video"; // String | Desired format (when action=download)
        String quality = "hd"; // String | Desired quality (when action=download)
        String formatId = "formatId_example"; // String | Specific format ID from formats list
        try {
            DownloadYouTubeVideo200Response result = apiInstance.downloadYouTubeVideo(url, action, format, quality, formatId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ToolsApi#downloadYouTubeVideo");
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
| **url** | **String**| YouTube video URL or video ID | |
| **action** | **String**| Action to perform: &#39;download&#39; returns download URL, &#39;formats&#39; lists available formats | [optional] [default to download] [enum: download, formats] |
| **format** | **String**| Desired format (when action&#x3D;download) | [optional] [default to video] [enum: video, audio] |
| **quality** | **String**| Desired quality (when action&#x3D;download) | [optional] [default to hd] [enum: hd, sd] |
| **formatId** | **String**| Specific format ID from formats list | [optional] |

### Return type

[**DownloadYouTubeVideo200Response**](DownloadYouTubeVideo200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  * X-RateLimit-Limit - Daily rate limit <br>  * X-RateLimit-Remaining - Remaining calls today <br>  * X-RateLimit-Reset - Unix timestamp when limit resets <br>  |
| **401** | Unauthorized |  -  |
| **403** | Tools API not available on free plan |  -  |
| **429** | Daily rate limit exceeded |  -  |

## downloadYouTubeVideoWithHttpInfo

> ApiResponse<DownloadYouTubeVideo200Response> downloadYouTubeVideo downloadYouTubeVideoWithHttpInfo(url, action, format, quality, formatId)

Download YouTube video

Download YouTube videos or audio. Returns available formats or direct download URL.  **Rate Limits:** Build (50/day), Accelerate (500/day), Unlimited (unlimited) 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ToolsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ToolsApi apiInstance = new ToolsApi(defaultClient);
        String url = "https://www.youtube.com/watch?v=dQw4w9WgXcQ"; // String | YouTube video URL or video ID
        String action = "download"; // String | Action to perform: 'download' returns download URL, 'formats' lists available formats
        String format = "video"; // String | Desired format (when action=download)
        String quality = "hd"; // String | Desired quality (when action=download)
        String formatId = "formatId_example"; // String | Specific format ID from formats list
        try {
            ApiResponse<DownloadYouTubeVideo200Response> response = apiInstance.downloadYouTubeVideoWithHttpInfo(url, action, format, quality, formatId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ToolsApi#downloadYouTubeVideo");
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
| **url** | **String**| YouTube video URL or video ID | |
| **action** | **String**| Action to perform: &#39;download&#39; returns download URL, &#39;formats&#39; lists available formats | [optional] [default to download] [enum: download, formats] |
| **format** | **String**| Desired format (when action&#x3D;download) | [optional] [default to video] [enum: video, audio] |
| **quality** | **String**| Desired quality (when action&#x3D;download) | [optional] [default to hd] [enum: hd, sd] |
| **formatId** | **String**| Specific format ID from formats list | [optional] |

### Return type

ApiResponse<[**DownloadYouTubeVideo200Response**](DownloadYouTubeVideo200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  * X-RateLimit-Limit - Daily rate limit <br>  * X-RateLimit-Remaining - Remaining calls today <br>  * X-RateLimit-Reset - Unix timestamp when limit resets <br>  |
| **401** | Unauthorized |  -  |
| **403** | Tools API not available on free plan |  -  |
| **429** | Daily rate limit exceeded |  -  |


## getYouTubeTranscript

> GetYouTubeTranscript200Response getYouTubeTranscript(url, lang)

Get YouTube transcript

Extract transcript/captions from a YouTube video.  **Rate Limits:** Build (50/day), Accelerate (500/day), Unlimited (unlimited) 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ToolsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ToolsApi apiInstance = new ToolsApi(defaultClient);
        String url = "url_example"; // String | YouTube video URL or video ID
        String lang = "en"; // String | Language code for transcript
        try {
            GetYouTubeTranscript200Response result = apiInstance.getYouTubeTranscript(url, lang);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ToolsApi#getYouTubeTranscript");
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
| **url** | **String**| YouTube video URL or video ID | |
| **lang** | **String**| Language code for transcript | [optional] [default to en] |

### Return type

[**GetYouTubeTranscript200Response**](GetYouTubeTranscript200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |
| **404** | No transcript available |  -  |

## getYouTubeTranscriptWithHttpInfo

> ApiResponse<GetYouTubeTranscript200Response> getYouTubeTranscript getYouTubeTranscriptWithHttpInfo(url, lang)

Get YouTube transcript

Extract transcript/captions from a YouTube video.  **Rate Limits:** Build (50/day), Accelerate (500/day), Unlimited (unlimited) 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ToolsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ToolsApi apiInstance = new ToolsApi(defaultClient);
        String url = "url_example"; // String | YouTube video URL or video ID
        String lang = "en"; // String | Language code for transcript
        try {
            ApiResponse<GetYouTubeTranscript200Response> response = apiInstance.getYouTubeTranscriptWithHttpInfo(url, lang);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ToolsApi#getYouTubeTranscript");
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
| **url** | **String**| YouTube video URL or video ID | |
| **lang** | **String**| Language code for transcript | [optional] [default to en] |

### Return type

ApiResponse<[**GetYouTubeTranscript200Response**](GetYouTubeTranscript200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |
| **404** | No transcript available |  -  |

