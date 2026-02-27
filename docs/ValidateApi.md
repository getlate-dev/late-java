# ValidateApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**validateMedia**](ValidateApi.md#validateMedia) | **POST** /v1/tools/validate/media | Validate media URL |
| [**validateMediaWithHttpInfo**](ValidateApi.md#validateMediaWithHttpInfo) | **POST** /v1/tools/validate/media | Validate media URL |
| [**validatePost**](ValidateApi.md#validatePost) | **POST** /v1/tools/validate/post | Validate post content |
| [**validatePostWithHttpInfo**](ValidateApi.md#validatePostWithHttpInfo) | **POST** /v1/tools/validate/post | Validate post content |
| [**validatePostLength**](ValidateApi.md#validatePostLength) | **POST** /v1/tools/validate/post-length | Validate post character count |
| [**validatePostLengthWithHttpInfo**](ValidateApi.md#validatePostLengthWithHttpInfo) | **POST** /v1/tools/validate/post-length | Validate post character count |
| [**validateSubreddit**](ValidateApi.md#validateSubreddit) | **GET** /v1/tools/validate/subreddit | Check subreddit existence |
| [**validateSubredditWithHttpInfo**](ValidateApi.md#validateSubredditWithHttpInfo) | **GET** /v1/tools/validate/subreddit | Check subreddit existence |



## validateMedia

> ValidateMedia200Response validateMedia(validateMediaRequest)

Validate media URL

Check if a media URL is accessible and return metadata (content type, file size) plus per-platform size limit comparisons.  Performs a HEAD request (with GET fallback) to detect content type and size. Rejects private/localhost URLs for SSRF protection.  Platform limits are sourced from each platform&#39;s actual upload constraints. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ValidateApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ValidateApi apiInstance = new ValidateApi(defaultClient);
        ValidateMediaRequest validateMediaRequest = new ValidateMediaRequest(); // ValidateMediaRequest | 
        try {
            ValidateMedia200Response result = apiInstance.validateMedia(validateMediaRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ValidateApi#validateMedia");
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
| **validateMediaRequest** | [**ValidateMediaRequest**](ValidateMediaRequest.md)|  | |

### Return type

[**ValidateMedia200Response**](ValidateMedia200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Media validation result |  -  |

## validateMediaWithHttpInfo

> ApiResponse<ValidateMedia200Response> validateMedia validateMediaWithHttpInfo(validateMediaRequest)

Validate media URL

Check if a media URL is accessible and return metadata (content type, file size) plus per-platform size limit comparisons.  Performs a HEAD request (with GET fallback) to detect content type and size. Rejects private/localhost URLs for SSRF protection.  Platform limits are sourced from each platform&#39;s actual upload constraints. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ValidateApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ValidateApi apiInstance = new ValidateApi(defaultClient);
        ValidateMediaRequest validateMediaRequest = new ValidateMediaRequest(); // ValidateMediaRequest | 
        try {
            ApiResponse<ValidateMedia200Response> response = apiInstance.validateMediaWithHttpInfo(validateMediaRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ValidateApi#validateMedia");
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
| **validateMediaRequest** | [**ValidateMediaRequest**](ValidateMediaRequest.md)|  | |

### Return type

ApiResponse<[**ValidateMedia200Response**](ValidateMedia200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Media validation result |  -  |


## validatePost

> ValidatePost200Response validatePost(validatePostRequest)

Validate post content

Dry-run the full post validation pipeline without publishing. Catches issues like missing media for Instagram/TikTok/YouTube, hashtag limits, invalid thread formats, Facebook Reel requirements, and character limit violations.  Accepts the same body as &#x60;POST /v1/posts&#x60;. Does NOT validate accounts, process media, or track usage. This is content-only validation.  Returns errors for failures and warnings for near-limit content (&gt;90% of character limit). 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ValidateApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ValidateApi apiInstance = new ValidateApi(defaultClient);
        ValidatePostRequest validatePostRequest = new ValidatePostRequest(); // ValidatePostRequest | 
        try {
            ValidatePost200Response result = apiInstance.validatePost(validatePostRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ValidateApi#validatePost");
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
| **validatePostRequest** | [**ValidatePostRequest**](ValidatePostRequest.md)|  | |

### Return type

[**ValidatePost200Response**](ValidatePost200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Validation result |  -  |

## validatePostWithHttpInfo

> ApiResponse<ValidatePost200Response> validatePost validatePostWithHttpInfo(validatePostRequest)

Validate post content

Dry-run the full post validation pipeline without publishing. Catches issues like missing media for Instagram/TikTok/YouTube, hashtag limits, invalid thread formats, Facebook Reel requirements, and character limit violations.  Accepts the same body as &#x60;POST /v1/posts&#x60;. Does NOT validate accounts, process media, or track usage. This is content-only validation.  Returns errors for failures and warnings for near-limit content (&gt;90% of character limit). 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ValidateApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ValidateApi apiInstance = new ValidateApi(defaultClient);
        ValidatePostRequest validatePostRequest = new ValidatePostRequest(); // ValidatePostRequest | 
        try {
            ApiResponse<ValidatePost200Response> response = apiInstance.validatePostWithHttpInfo(validatePostRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ValidateApi#validatePost");
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
| **validatePostRequest** | [**ValidatePostRequest**](ValidatePostRequest.md)|  | |

### Return type

ApiResponse<[**ValidatePost200Response**](ValidatePost200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Validation result |  -  |


## validatePostLength

> ValidatePostLength200Response validatePostLength(validatePostLengthRequest)

Validate post character count

Check weighted character count per platform and whether the text is within each platform&#39;s limit.  Twitter/X uses weighted counting (URLs &#x3D; 23 chars via t.co, emojis &#x3D; 2 chars). All other platforms use plain character length.  Returns counts and limits for all 15 supported platform variants. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ValidateApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ValidateApi apiInstance = new ValidateApi(defaultClient);
        ValidatePostLengthRequest validatePostLengthRequest = new ValidatePostLengthRequest(); // ValidatePostLengthRequest | 
        try {
            ValidatePostLength200Response result = apiInstance.validatePostLength(validatePostLengthRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ValidateApi#validatePostLength");
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
| **validatePostLengthRequest** | [**ValidatePostLengthRequest**](ValidatePostLengthRequest.md)|  | |

### Return type

[**ValidatePostLength200Response**](ValidatePostLength200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Character counts per platform |  -  |

## validatePostLengthWithHttpInfo

> ApiResponse<ValidatePostLength200Response> validatePostLength validatePostLengthWithHttpInfo(validatePostLengthRequest)

Validate post character count

Check weighted character count per platform and whether the text is within each platform&#39;s limit.  Twitter/X uses weighted counting (URLs &#x3D; 23 chars via t.co, emojis &#x3D; 2 chars). All other platforms use plain character length.  Returns counts and limits for all 15 supported platform variants. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ValidateApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ValidateApi apiInstance = new ValidateApi(defaultClient);
        ValidatePostLengthRequest validatePostLengthRequest = new ValidatePostLengthRequest(); // ValidatePostLengthRequest | 
        try {
            ApiResponse<ValidatePostLength200Response> response = apiInstance.validatePostLengthWithHttpInfo(validatePostLengthRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ValidateApi#validatePostLength");
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
| **validatePostLengthRequest** | [**ValidatePostLengthRequest**](ValidatePostLengthRequest.md)|  | |

### Return type

ApiResponse<[**ValidatePostLength200Response**](ValidatePostLength200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Character counts per platform |  -  |


## validateSubreddit

> ValidateSubreddit200Response validateSubreddit(name)

Check subreddit existence

Check if a subreddit exists and return basic info (title, subscriber count, NSFW status, post types allowed).  Uses Reddit&#39;s public JSON API (no Reddit auth needed). Returns &#x60;exists: false&#x60; for private, banned, or nonexistent subreddits. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ValidateApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ValidateApi apiInstance = new ValidateApi(defaultClient);
        String name = "programming"; // String | Subreddit name (with or without \"r/\" prefix)
        try {
            ValidateSubreddit200Response result = apiInstance.validateSubreddit(name);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ValidateApi#validateSubreddit");
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
| **name** | **String**| Subreddit name (with or without \&quot;r/\&quot; prefix) | |

### Return type

[**ValidateSubreddit200Response**](ValidateSubreddit200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Subreddit lookup result |  -  |

## validateSubredditWithHttpInfo

> ApiResponse<ValidateSubreddit200Response> validateSubreddit validateSubredditWithHttpInfo(name)

Check subreddit existence

Check if a subreddit exists and return basic info (title, subscriber count, NSFW status, post types allowed).  Uses Reddit&#39;s public JSON API (no Reddit auth needed). Returns &#x60;exists: false&#x60; for private, banned, or nonexistent subreddits. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ValidateApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ValidateApi apiInstance = new ValidateApi(defaultClient);
        String name = "programming"; // String | Subreddit name (with or without \"r/\" prefix)
        try {
            ApiResponse<ValidateSubreddit200Response> response = apiInstance.validateSubredditWithHttpInfo(name);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ValidateApi#validateSubreddit");
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
| **name** | **String**| Subreddit name (with or without \&quot;r/\&quot; prefix) | |

### Return type

ApiResponse<[**ValidateSubreddit200Response**](ValidateSubreddit200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Subreddit lookup result |  -  |

