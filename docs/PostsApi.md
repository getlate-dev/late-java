# PostsApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**bulkUploadPosts**](PostsApi.md#bulkUploadPosts) | **POST** /v1/posts/bulk-upload | Bulk upload from CSV |
| [**bulkUploadPostsWithHttpInfo**](PostsApi.md#bulkUploadPostsWithHttpInfo) | **POST** /v1/posts/bulk-upload | Bulk upload from CSV |
| [**createPost**](PostsApi.md#createPost) | **POST** /v1/posts | Create post |
| [**createPostWithHttpInfo**](PostsApi.md#createPostWithHttpInfo) | **POST** /v1/posts | Create post |
| [**deletePost**](PostsApi.md#deletePost) | **DELETE** /v1/posts/{postId} | Delete post |
| [**deletePostWithHttpInfo**](PostsApi.md#deletePostWithHttpInfo) | **DELETE** /v1/posts/{postId} | Delete post |
| [**getPost**](PostsApi.md#getPost) | **GET** /v1/posts/{postId} | Get post |
| [**getPostWithHttpInfo**](PostsApi.md#getPostWithHttpInfo) | **GET** /v1/posts/{postId} | Get post |
| [**listPosts**](PostsApi.md#listPosts) | **GET** /v1/posts | List posts |
| [**listPostsWithHttpInfo**](PostsApi.md#listPostsWithHttpInfo) | **GET** /v1/posts | List posts |
| [**retryPost**](PostsApi.md#retryPost) | **POST** /v1/posts/{postId}/retry | Retry failed post |
| [**retryPostWithHttpInfo**](PostsApi.md#retryPostWithHttpInfo) | **POST** /v1/posts/{postId}/retry | Retry failed post |
| [**unpublishPost**](PostsApi.md#unpublishPost) | **POST** /v1/posts/{postId}/unpublish | Unpublish post |
| [**unpublishPostWithHttpInfo**](PostsApi.md#unpublishPostWithHttpInfo) | **POST** /v1/posts/{postId}/unpublish | Unpublish post |
| [**updatePost**](PostsApi.md#updatePost) | **PUT** /v1/posts/{postId} | Update post |
| [**updatePostWithHttpInfo**](PostsApi.md#updatePostWithHttpInfo) | **PUT** /v1/posts/{postId} | Update post |



## bulkUploadPosts

> BulkUploadPosts200Response bulkUploadPosts(dryRun, _file)

Bulk upload from CSV

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.PostsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        PostsApi apiInstance = new PostsApi(defaultClient);
        Boolean dryRun = false; // Boolean | 
        File _file = new File("/path/to/file"); // File | 
        try {
            BulkUploadPosts200Response result = apiInstance.bulkUploadPosts(dryRun, _file);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling PostsApi#bulkUploadPosts");
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
| **dryRun** | **Boolean**|  | [optional] [default to false] |
| **_file** | **File**|  | [optional] |

### Return type

[**BulkUploadPosts200Response**](BulkUploadPosts200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Bulk upload results |  -  |
| **207** | Partial success |  -  |
| **400** | Invalid CSV or validation errors |  -  |
| **401** | Unauthorized |  -  |
| **429** | Rate limit exceeded. Can be triggered by: - **API rate limit**: Requests per minute exceeded - **Account cooldown**: One or more accounts are temporarily rate-limited  |  -  |

## bulkUploadPostsWithHttpInfo

> ApiResponse<BulkUploadPosts200Response> bulkUploadPosts bulkUploadPostsWithHttpInfo(dryRun, _file)

Bulk upload from CSV

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.PostsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        PostsApi apiInstance = new PostsApi(defaultClient);
        Boolean dryRun = false; // Boolean | 
        File _file = new File("/path/to/file"); // File | 
        try {
            ApiResponse<BulkUploadPosts200Response> response = apiInstance.bulkUploadPostsWithHttpInfo(dryRun, _file);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling PostsApi#bulkUploadPosts");
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
| **dryRun** | **Boolean**|  | [optional] [default to false] |
| **_file** | **File**|  | [optional] |

### Return type

ApiResponse<[**BulkUploadPosts200Response**](BulkUploadPosts200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Bulk upload results |  -  |
| **207** | Partial success |  -  |
| **400** | Invalid CSV or validation errors |  -  |
| **401** | Unauthorized |  -  |
| **429** | Rate limit exceeded. Can be triggered by: - **API rate limit**: Requests per minute exceeded - **Account cooldown**: One or more accounts are temporarily rate-limited  |  -  |


## createPost

> PostCreateResponse createPost(createPostRequest)

Create post

**Getting Post URLs:** - Immediate posts (&#x60;publishNow: true&#x60;): response includes &#x60;platformPostUrl&#x60; in &#x60;post.platforms[]&#x60;. - Scheduled posts: fetch via &#x60;GET /v1/posts/{postId}&#x60; after publish time for &#x60;platformPostUrl&#x60;.  **Content requirements:** - &#x60;content&#x60; is optional when media is attached, all platforms have &#x60;customContent&#x60;, or posting to YouTube only. - Text-only posts require &#x60;content&#x60;. Stories ignore captions.  **Platform constraints:** - YouTube: video required, optional thumbnail via &#x60;MediaItem.thumbnail&#x60; - Instagram/TikTok: media required; TikTok cannot mix videos and images - Instagram carousels: up to 10 items; Threads carousels: up to 10 images only - Facebook Stories: single image or video, set &#x60;contentType: &#39;story&#39;&#x60; - LinkedIn: up to 20 images or a single PDF (max 100MB) - Pinterest: single image or video, &#x60;boardId&#x60; required - Bluesky: up to 4 images, auto-recompressed to ~1MB - Snapchat: single image or video, set &#x60;contentType&#x60; in platformSpecificData 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.PostsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        PostsApi apiInstance = new PostsApi(defaultClient);
        CreatePostRequest createPostRequest = new CreatePostRequest(); // CreatePostRequest | 
        try {
            PostCreateResponse result = apiInstance.createPost(createPostRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling PostsApi#createPost");
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
| **createPostRequest** | [**CreatePostRequest**](CreatePostRequest.md)|  | |

### Return type

[**PostCreateResponse**](PostCreateResponse.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Post created |  -  |
| **400** | Validation error |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **409** | Duplicate content detected |  -  |
| **429** | Rate limit exceeded. Can be triggered by: - **API rate limit**: Requests per minute exceeded (Free: 60, Build: 120, Accelerate: 600, Unlimited: 1,200) - **Velocity limit**: 15 posts per hour per account exceeded - **Account cooldown**: Account temporarily rate-limited due to repeated errors (escalating: 10min, 20min, 40min, up to 24h) - **Daily post limit**: Platform daily limits exceeded (X: 20, Pinterest: 25, Instagram/Facebook: 100, Threads: 250, others: 50)  |  * Retry-After - Seconds until the rate limit resets (for API rate limits) <br>  * X-RateLimit-Limit - The rate limit ceiling <br>  * X-RateLimit-Remaining - Requests remaining in current window <br>  |

## createPostWithHttpInfo

> ApiResponse<PostCreateResponse> createPost createPostWithHttpInfo(createPostRequest)

Create post

**Getting Post URLs:** - Immediate posts (&#x60;publishNow: true&#x60;): response includes &#x60;platformPostUrl&#x60; in &#x60;post.platforms[]&#x60;. - Scheduled posts: fetch via &#x60;GET /v1/posts/{postId}&#x60; after publish time for &#x60;platformPostUrl&#x60;.  **Content requirements:** - &#x60;content&#x60; is optional when media is attached, all platforms have &#x60;customContent&#x60;, or posting to YouTube only. - Text-only posts require &#x60;content&#x60;. Stories ignore captions.  **Platform constraints:** - YouTube: video required, optional thumbnail via &#x60;MediaItem.thumbnail&#x60; - Instagram/TikTok: media required; TikTok cannot mix videos and images - Instagram carousels: up to 10 items; Threads carousels: up to 10 images only - Facebook Stories: single image or video, set &#x60;contentType: &#39;story&#39;&#x60; - LinkedIn: up to 20 images or a single PDF (max 100MB) - Pinterest: single image or video, &#x60;boardId&#x60; required - Bluesky: up to 4 images, auto-recompressed to ~1MB - Snapchat: single image or video, set &#x60;contentType&#x60; in platformSpecificData 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.PostsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        PostsApi apiInstance = new PostsApi(defaultClient);
        CreatePostRequest createPostRequest = new CreatePostRequest(); // CreatePostRequest | 
        try {
            ApiResponse<PostCreateResponse> response = apiInstance.createPostWithHttpInfo(createPostRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling PostsApi#createPost");
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
| **createPostRequest** | [**CreatePostRequest**](CreatePostRequest.md)|  | |

### Return type

ApiResponse<[**PostCreateResponse**](PostCreateResponse.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Post created |  -  |
| **400** | Validation error |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **409** | Duplicate content detected |  -  |
| **429** | Rate limit exceeded. Can be triggered by: - **API rate limit**: Requests per minute exceeded (Free: 60, Build: 120, Accelerate: 600, Unlimited: 1,200) - **Velocity limit**: 15 posts per hour per account exceeded - **Account cooldown**: Account temporarily rate-limited due to repeated errors (escalating: 10min, 20min, 40min, up to 24h) - **Daily post limit**: Platform daily limits exceeded (X: 20, Pinterest: 25, Instagram/Facebook: 100, Threads: 250, others: 50)  |  * Retry-After - Seconds until the rate limit resets (for API rate limits) <br>  * X-RateLimit-Limit - The rate limit ceiling <br>  * X-RateLimit-Remaining - Requests remaining in current window <br>  |


## deletePost

> PostDeleteResponse deletePost(postId)

Delete post

Delete a draft or scheduled post from Late. Only posts that have not been published can be deleted. To remove a published post from a social media platform, use the [Unpublish endpoint](#tag/Posts/operation/unpublishPost) instead. When deleting a scheduled or draft post that consumed upload quota, the quota will be automatically refunded. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.PostsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        PostsApi apiInstance = new PostsApi(defaultClient);
        String postId = "postId_example"; // String | 
        try {
            PostDeleteResponse result = apiInstance.deletePost(postId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling PostsApi#deletePost");
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
| **postId** | **String**|  | |

### Return type

[**PostDeleteResponse**](PostDeleteResponse.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Deleted |  -  |
| **400** | Cannot delete published posts |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Resource not found |  -  |

## deletePostWithHttpInfo

> ApiResponse<PostDeleteResponse> deletePost deletePostWithHttpInfo(postId)

Delete post

Delete a draft or scheduled post from Late. Only posts that have not been published can be deleted. To remove a published post from a social media platform, use the [Unpublish endpoint](#tag/Posts/operation/unpublishPost) instead. When deleting a scheduled or draft post that consumed upload quota, the quota will be automatically refunded. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.PostsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        PostsApi apiInstance = new PostsApi(defaultClient);
        String postId = "postId_example"; // String | 
        try {
            ApiResponse<PostDeleteResponse> response = apiInstance.deletePostWithHttpInfo(postId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling PostsApi#deletePost");
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
| **postId** | **String**|  | |

### Return type

ApiResponse<[**PostDeleteResponse**](PostDeleteResponse.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Deleted |  -  |
| **400** | Cannot delete published posts |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Resource not found |  -  |


## getPost

> PostGetResponse getPost(postId)

Get post

Fetch a single post by ID. For published posts, this returns &#x60;platformPostUrl&#x60;  for each platform - useful for retrieving post URLs after scheduled posts publish. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.PostsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        PostsApi apiInstance = new PostsApi(defaultClient);
        String postId = "postId_example"; // String | 
        try {
            PostGetResponse result = apiInstance.getPost(postId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling PostsApi#getPost");
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
| **postId** | **String**|  | |

### Return type

[**PostGetResponse**](PostGetResponse.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Post |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Resource not found |  -  |

## getPostWithHttpInfo

> ApiResponse<PostGetResponse> getPost getPostWithHttpInfo(postId)

Get post

Fetch a single post by ID. For published posts, this returns &#x60;platformPostUrl&#x60;  for each platform - useful for retrieving post URLs after scheduled posts publish. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.PostsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        PostsApi apiInstance = new PostsApi(defaultClient);
        String postId = "postId_example"; // String | 
        try {
            ApiResponse<PostGetResponse> response = apiInstance.getPostWithHttpInfo(postId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling PostsApi#getPost");
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
| **postId** | **String**|  | |

### Return type

ApiResponse<[**PostGetResponse**](PostGetResponse.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Post |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Resource not found |  -  |


## listPosts

> PostsListResponse listPosts(page, limit, status, platform, profileId, createdBy, dateFrom, dateTo, includeHidden)

List posts

**Getting Post URLs:** For published posts, each platform entry includes &#x60;platformPostUrl&#x60; with the public URL. Use &#x60;status&#x3D;published&#x60; filter to fetch only published posts with their URLs.  Notes and constraints by platform when interpreting the response: - YouTube: posts always include at least one video in mediaItems. - Instagram/TikTok: posts always include media; drafts may omit media until finalized in client. - TikTok: mediaItems will not mix photos and videos in the same post. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.PostsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        PostsApi apiInstance = new PostsApi(defaultClient);
        Integer page = 1; // Integer | Page number (1-based)
        Integer limit = 10; // Integer | Page size
        String status = "draft"; // String | 
        String platform = "twitter"; // String | 
        String profileId = "profileId_example"; // String | 
        String createdBy = "createdBy_example"; // String | 
        LocalDate dateFrom = LocalDate.now(); // LocalDate | 
        LocalDate dateTo = LocalDate.now(); // LocalDate | 
        Boolean includeHidden = false; // Boolean | 
        try {
            PostsListResponse result = apiInstance.listPosts(page, limit, status, platform, profileId, createdBy, dateFrom, dateTo, includeHidden);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling PostsApi#listPosts");
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
| **page** | **Integer**| Page number (1-based) | [optional] [default to 1] |
| **limit** | **Integer**| Page size | [optional] [default to 10] |
| **status** | **String**|  | [optional] [enum: draft, scheduled, published, failed] |
| **platform** | **String**|  | [optional] |
| **profileId** | **String**|  | [optional] |
| **createdBy** | **String**|  | [optional] |
| **dateFrom** | **LocalDate**|  | [optional] |
| **dateTo** | **LocalDate**|  | [optional] |
| **includeHidden** | **Boolean**|  | [optional] [default to false] |

### Return type

[**PostsListResponse**](PostsListResponse.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated posts |  -  |
| **401** | Unauthorized |  -  |

## listPostsWithHttpInfo

> ApiResponse<PostsListResponse> listPosts listPostsWithHttpInfo(page, limit, status, platform, profileId, createdBy, dateFrom, dateTo, includeHidden)

List posts

**Getting Post URLs:** For published posts, each platform entry includes &#x60;platformPostUrl&#x60; with the public URL. Use &#x60;status&#x3D;published&#x60; filter to fetch only published posts with their URLs.  Notes and constraints by platform when interpreting the response: - YouTube: posts always include at least one video in mediaItems. - Instagram/TikTok: posts always include media; drafts may omit media until finalized in client. - TikTok: mediaItems will not mix photos and videos in the same post. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.PostsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        PostsApi apiInstance = new PostsApi(defaultClient);
        Integer page = 1; // Integer | Page number (1-based)
        Integer limit = 10; // Integer | Page size
        String status = "draft"; // String | 
        String platform = "twitter"; // String | 
        String profileId = "profileId_example"; // String | 
        String createdBy = "createdBy_example"; // String | 
        LocalDate dateFrom = LocalDate.now(); // LocalDate | 
        LocalDate dateTo = LocalDate.now(); // LocalDate | 
        Boolean includeHidden = false; // Boolean | 
        try {
            ApiResponse<PostsListResponse> response = apiInstance.listPostsWithHttpInfo(page, limit, status, platform, profileId, createdBy, dateFrom, dateTo, includeHidden);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling PostsApi#listPosts");
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
| **page** | **Integer**| Page number (1-based) | [optional] [default to 1] |
| **limit** | **Integer**| Page size | [optional] [default to 10] |
| **status** | **String**|  | [optional] [enum: draft, scheduled, published, failed] |
| **platform** | **String**|  | [optional] |
| **profileId** | **String**|  | [optional] |
| **createdBy** | **String**|  | [optional] |
| **dateFrom** | **LocalDate**|  | [optional] |
| **dateTo** | **LocalDate**|  | [optional] |
| **includeHidden** | **Boolean**|  | [optional] [default to false] |

### Return type

ApiResponse<[**PostsListResponse**](PostsListResponse.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated posts |  -  |
| **401** | Unauthorized |  -  |


## retryPost

> PostRetryResponse retryPost(postId)

Retry failed post

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.PostsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        PostsApi apiInstance = new PostsApi(defaultClient);
        String postId = "postId_example"; // String | 
        try {
            PostRetryResponse result = apiInstance.retryPost(postId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling PostsApi#retryPost");
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
| **postId** | **String**|  | |

### Return type

[**PostRetryResponse**](PostRetryResponse.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Retry successful |  -  |
| **207** | Partial success |  -  |
| **400** | Invalid state |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Resource not found |  -  |
| **409** | Post is currently publishing |  -  |
| **429** | Rate limit exceeded. Can be triggered by: - **API rate limit**: Requests per minute exceeded - **Velocity limit**: 15 posts per hour per account exceeded - **Account cooldown**: Account temporarily rate-limited due to repeated errors  |  -  |

## retryPostWithHttpInfo

> ApiResponse<PostRetryResponse> retryPost retryPostWithHttpInfo(postId)

Retry failed post

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.PostsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        PostsApi apiInstance = new PostsApi(defaultClient);
        String postId = "postId_example"; // String | 
        try {
            ApiResponse<PostRetryResponse> response = apiInstance.retryPostWithHttpInfo(postId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling PostsApi#retryPost");
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
| **postId** | **String**|  | |

### Return type

ApiResponse<[**PostRetryResponse**](PostRetryResponse.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Retry successful |  -  |
| **207** | Partial success |  -  |
| **400** | Invalid state |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Resource not found |  -  |
| **409** | Post is currently publishing |  -  |
| **429** | Rate limit exceeded. Can be triggered by: - **API rate limit**: Requests per minute exceeded - **Velocity limit**: 15 posts per hour per account exceeded - **Account cooldown**: Account temporarily rate-limited due to repeated errors  |  -  |


## unpublishPost

> UnpublishPost200Response unpublishPost(postId, unpublishPostRequest)

Unpublish post

Permanently deletes a published post from the specified social media platform. The post record in Late is kept but its platform status is updated to \&quot;cancelled\&quot;. This does not delete the post from Late, only from the platform.  **Supported platforms:** Threads, Facebook, Twitter/X, LinkedIn, YouTube, Pinterest, Reddit, Bluesky, Google Business, Telegram.  **Not supported:** - **Instagram:** No deletion API available. Posts must be deleted manually. - **TikTok:** No deletion API available. Posts must be deleted manually. - **Snapchat:** No deletion API available. Posts must be deleted manually.  **Platform notes:** - **Threaded posts (Twitter, Threads, Bluesky):** If the post was published as a thread, all items in the thread are deleted (not just the first one). Posts published before this feature was added will only have the first item deleted. - **Telegram:** Messages older than 48 hours may fail to delete (Telegram Bot API limitation). - **YouTube:** This permanently deletes the video from YouTube. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.PostsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        PostsApi apiInstance = new PostsApi(defaultClient);
        String postId = "postId_example"; // String | 
        UnpublishPostRequest unpublishPostRequest = new UnpublishPostRequest(); // UnpublishPostRequest | 
        try {
            UnpublishPost200Response result = apiInstance.unpublishPost(postId, unpublishPostRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling PostsApi#unpublishPost");
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
| **postId** | **String**|  | |
| **unpublishPostRequest** | [**UnpublishPostRequest**](UnpublishPostRequest.md)|  | |

### Return type

[**UnpublishPost200Response**](UnpublishPost200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Post deleted from platform |  -  |
| **400** | Invalid request. Possible reasons: - Platform not recognized or not supported for deletion - Post does not have the specified platform - Post is not in \&quot;published\&quot; status on that platform - No platform post ID found (post may not have been published correctly) - No access token (account needs to be reconnected)  |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Resource not found |  -  |
| **500** | Platform API deletion failed |  -  |

## unpublishPostWithHttpInfo

> ApiResponse<UnpublishPost200Response> unpublishPost unpublishPostWithHttpInfo(postId, unpublishPostRequest)

Unpublish post

Permanently deletes a published post from the specified social media platform. The post record in Late is kept but its platform status is updated to \&quot;cancelled\&quot;. This does not delete the post from Late, only from the platform.  **Supported platforms:** Threads, Facebook, Twitter/X, LinkedIn, YouTube, Pinterest, Reddit, Bluesky, Google Business, Telegram.  **Not supported:** - **Instagram:** No deletion API available. Posts must be deleted manually. - **TikTok:** No deletion API available. Posts must be deleted manually. - **Snapchat:** No deletion API available. Posts must be deleted manually.  **Platform notes:** - **Threaded posts (Twitter, Threads, Bluesky):** If the post was published as a thread, all items in the thread are deleted (not just the first one). Posts published before this feature was added will only have the first item deleted. - **Telegram:** Messages older than 48 hours may fail to delete (Telegram Bot API limitation). - **YouTube:** This permanently deletes the video from YouTube. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.PostsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        PostsApi apiInstance = new PostsApi(defaultClient);
        String postId = "postId_example"; // String | 
        UnpublishPostRequest unpublishPostRequest = new UnpublishPostRequest(); // UnpublishPostRequest | 
        try {
            ApiResponse<UnpublishPost200Response> response = apiInstance.unpublishPostWithHttpInfo(postId, unpublishPostRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling PostsApi#unpublishPost");
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
| **postId** | **String**|  | |
| **unpublishPostRequest** | [**UnpublishPostRequest**](UnpublishPostRequest.md)|  | |

### Return type

ApiResponse<[**UnpublishPost200Response**](UnpublishPost200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Post deleted from platform |  -  |
| **400** | Invalid request. Possible reasons: - Platform not recognized or not supported for deletion - Post does not have the specified platform - Post is not in \&quot;published\&quot; status on that platform - No platform post ID found (post may not have been published correctly) - No access token (account needs to be reconnected)  |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Resource not found |  -  |
| **500** | Platform API deletion failed |  -  |


## updatePost

> PostUpdateResponse updatePost(postId, updatePostRequest)

Update post

Update an existing post. Only draft, scheduled, failed, and partial posts can be edited. Published, publishing, and cancelled posts cannot be modified. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.PostsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        PostsApi apiInstance = new PostsApi(defaultClient);
        String postId = "postId_example"; // String | 
        UpdatePostRequest updatePostRequest = new UpdatePostRequest(); // UpdatePostRequest | 
        try {
            PostUpdateResponse result = apiInstance.updatePost(postId, updatePostRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling PostsApi#updatePost");
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
| **postId** | **String**|  | |
| **updatePostRequest** | [**UpdatePostRequest**](UpdatePostRequest.md)|  | |

### Return type

[**PostUpdateResponse**](PostUpdateResponse.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Post updated |  -  |
| **207** | Partial publish success |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Resource not found |  -  |

## updatePostWithHttpInfo

> ApiResponse<PostUpdateResponse> updatePost updatePostWithHttpInfo(postId, updatePostRequest)

Update post

Update an existing post. Only draft, scheduled, failed, and partial posts can be edited. Published, publishing, and cancelled posts cannot be modified. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.PostsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        PostsApi apiInstance = new PostsApi(defaultClient);
        String postId = "postId_example"; // String | 
        UpdatePostRequest updatePostRequest = new UpdatePostRequest(); // UpdatePostRequest | 
        try {
            ApiResponse<PostUpdateResponse> response = apiInstance.updatePostWithHttpInfo(postId, updatePostRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling PostsApi#updatePost");
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
| **postId** | **String**|  | |
| **updatePostRequest** | [**UpdatePostRequest**](UpdatePostRequest.md)|  | |

### Return type

ApiResponse<[**PostUpdateResponse**](PostUpdateResponse.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Post updated |  -  |
| **207** | Partial publish success |  -  |
| **400** | Invalid request |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Resource not found |  -  |

