# CommentsApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**deleteInboxComment**](CommentsApi.md#deleteInboxComment) | **DELETE** /v1/inbox/comments/{postId} | Delete a comment |
| [**deleteInboxCommentWithHttpInfo**](CommentsApi.md#deleteInboxCommentWithHttpInfo) | **DELETE** /v1/inbox/comments/{postId} | Delete a comment |
| [**getInboxPostComments**](CommentsApi.md#getInboxPostComments) | **GET** /v1/inbox/comments/{postId} | Get comments for a post |
| [**getInboxPostCommentsWithHttpInfo**](CommentsApi.md#getInboxPostCommentsWithHttpInfo) | **GET** /v1/inbox/comments/{postId} | Get comments for a post |
| [**hideInboxComment**](CommentsApi.md#hideInboxComment) | **POST** /v1/inbox/comments/{postId}/{commentId}/hide | Hide a comment |
| [**hideInboxCommentWithHttpInfo**](CommentsApi.md#hideInboxCommentWithHttpInfo) | **POST** /v1/inbox/comments/{postId}/{commentId}/hide | Hide a comment |
| [**likeInboxComment**](CommentsApi.md#likeInboxComment) | **POST** /v1/inbox/comments/{postId}/{commentId}/like | Like a comment |
| [**likeInboxCommentWithHttpInfo**](CommentsApi.md#likeInboxCommentWithHttpInfo) | **POST** /v1/inbox/comments/{postId}/{commentId}/like | Like a comment |
| [**listInboxComments**](CommentsApi.md#listInboxComments) | **GET** /v1/inbox/comments | List posts with comments across all accounts |
| [**listInboxCommentsWithHttpInfo**](CommentsApi.md#listInboxCommentsWithHttpInfo) | **GET** /v1/inbox/comments | List posts with comments across all accounts |
| [**replyToInboxPost**](CommentsApi.md#replyToInboxPost) | **POST** /v1/inbox/comments/{postId} | Reply to a post or comment |
| [**replyToInboxPostWithHttpInfo**](CommentsApi.md#replyToInboxPostWithHttpInfo) | **POST** /v1/inbox/comments/{postId} | Reply to a post or comment |
| [**sendPrivateReplyToComment**](CommentsApi.md#sendPrivateReplyToComment) | **POST** /v1/inbox/comments/{postId}/{commentId}/private-reply | Send private reply to comment author |
| [**sendPrivateReplyToCommentWithHttpInfo**](CommentsApi.md#sendPrivateReplyToCommentWithHttpInfo) | **POST** /v1/inbox/comments/{postId}/{commentId}/private-reply | Send private reply to comment author |
| [**unhideInboxComment**](CommentsApi.md#unhideInboxComment) | **DELETE** /v1/inbox/comments/{postId}/{commentId}/hide | Unhide a comment |
| [**unhideInboxCommentWithHttpInfo**](CommentsApi.md#unhideInboxCommentWithHttpInfo) | **DELETE** /v1/inbox/comments/{postId}/{commentId}/hide | Unhide a comment |
| [**unlikeInboxComment**](CommentsApi.md#unlikeInboxComment) | **DELETE** /v1/inbox/comments/{postId}/{commentId}/like | Unlike a comment |
| [**unlikeInboxCommentWithHttpInfo**](CommentsApi.md#unlikeInboxCommentWithHttpInfo) | **DELETE** /v1/inbox/comments/{postId}/{commentId}/like | Unlike a comment |



## deleteInboxComment

> DeleteInboxComment200Response deleteInboxComment(postId, accountId, commentId)

Delete a comment

Delete a comment on a post. Supported by Facebook, Instagram, Bluesky, Reddit, YouTube, LinkedIn, and TikTok. Requires accountId and commentId query parameters. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.CommentsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentsApi apiInstance = new CommentsApi(defaultClient);
        String postId = "postId_example"; // String | 
        String accountId = "accountId_example"; // String | 
        String commentId = "commentId_example"; // String | 
        try {
            DeleteInboxComment200Response result = apiInstance.deleteInboxComment(postId, accountId, commentId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentsApi#deleteInboxComment");
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
| **accountId** | **String**|  | |
| **commentId** | **String**|  | |

### Return type

[**DeleteInboxComment200Response**](DeleteInboxComment200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Comment deleted |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |

## deleteInboxCommentWithHttpInfo

> ApiResponse<DeleteInboxComment200Response> deleteInboxComment deleteInboxCommentWithHttpInfo(postId, accountId, commentId)

Delete a comment

Delete a comment on a post. Supported by Facebook, Instagram, Bluesky, Reddit, YouTube, LinkedIn, and TikTok. Requires accountId and commentId query parameters. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.CommentsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentsApi apiInstance = new CommentsApi(defaultClient);
        String postId = "postId_example"; // String | 
        String accountId = "accountId_example"; // String | 
        String commentId = "commentId_example"; // String | 
        try {
            ApiResponse<DeleteInboxComment200Response> response = apiInstance.deleteInboxCommentWithHttpInfo(postId, accountId, commentId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentsApi#deleteInboxComment");
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
| **accountId** | **String**|  | |
| **commentId** | **String**|  | |

### Return type

ApiResponse<[**DeleteInboxComment200Response**](DeleteInboxComment200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Comment deleted |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |


## getInboxPostComments

> GetInboxPostComments200Response getInboxPostComments(postId, accountId, subreddit, limit, cursor, commentId)

Get comments for a post

Fetch comments for a specific post. Requires accountId query parameter.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.CommentsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentsApi apiInstance = new CommentsApi(defaultClient);
        String postId = "postId_example"; // String | 
        String accountId = "accountId_example"; // String | 
        String subreddit = "subreddit_example"; // String | (Reddit only) Subreddit name
        Integer limit = 25; // Integer | Maximum number of comments to return
        String cursor = "cursor_example"; // String | Pagination cursor
        String commentId = "commentId_example"; // String | (Reddit only) Get replies to a specific comment
        try {
            GetInboxPostComments200Response result = apiInstance.getInboxPostComments(postId, accountId, subreddit, limit, cursor, commentId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentsApi#getInboxPostComments");
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
| **accountId** | **String**|  | |
| **subreddit** | **String**| (Reddit only) Subreddit name | [optional] |
| **limit** | **Integer**| Maximum number of comments to return | [optional] [default to 25] |
| **cursor** | **String**| Pagination cursor | [optional] |
| **commentId** | **String**| (Reddit only) Get replies to a specific comment | [optional] |

### Return type

[**GetInboxPostComments200Response**](GetInboxPostComments200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Comments for the post |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |

## getInboxPostCommentsWithHttpInfo

> ApiResponse<GetInboxPostComments200Response> getInboxPostComments getInboxPostCommentsWithHttpInfo(postId, accountId, subreddit, limit, cursor, commentId)

Get comments for a post

Fetch comments for a specific post. Requires accountId query parameter.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.CommentsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentsApi apiInstance = new CommentsApi(defaultClient);
        String postId = "postId_example"; // String | 
        String accountId = "accountId_example"; // String | 
        String subreddit = "subreddit_example"; // String | (Reddit only) Subreddit name
        Integer limit = 25; // Integer | Maximum number of comments to return
        String cursor = "cursor_example"; // String | Pagination cursor
        String commentId = "commentId_example"; // String | (Reddit only) Get replies to a specific comment
        try {
            ApiResponse<GetInboxPostComments200Response> response = apiInstance.getInboxPostCommentsWithHttpInfo(postId, accountId, subreddit, limit, cursor, commentId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentsApi#getInboxPostComments");
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
| **accountId** | **String**|  | |
| **subreddit** | **String**| (Reddit only) Subreddit name | [optional] |
| **limit** | **Integer**| Maximum number of comments to return | [optional] [default to 25] |
| **cursor** | **String**| Pagination cursor | [optional] |
| **commentId** | **String**| (Reddit only) Get replies to a specific comment | [optional] |

### Return type

ApiResponse<[**GetInboxPostComments200Response**](GetInboxPostComments200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Comments for the post |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |


## hideInboxComment

> HideInboxComment200Response hideInboxComment(postId, commentId, hideInboxCommentRequest)

Hide a comment

Hide a comment on a post. Supported by Facebook, Instagram, and Threads. Hidden comments are only visible to the commenter and page admin. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.CommentsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentsApi apiInstance = new CommentsApi(defaultClient);
        String postId = "postId_example"; // String | 
        String commentId = "commentId_example"; // String | 
        HideInboxCommentRequest hideInboxCommentRequest = new HideInboxCommentRequest(); // HideInboxCommentRequest | 
        try {
            HideInboxComment200Response result = apiInstance.hideInboxComment(postId, commentId, hideInboxCommentRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentsApi#hideInboxComment");
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
| **commentId** | **String**|  | |
| **hideInboxCommentRequest** | [**HideInboxCommentRequest**](HideInboxCommentRequest.md)|  | |

### Return type

[**HideInboxComment200Response**](HideInboxComment200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Comment hidden |  -  |
| **400** | Platform does not support hiding comments |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |

## hideInboxCommentWithHttpInfo

> ApiResponse<HideInboxComment200Response> hideInboxComment hideInboxCommentWithHttpInfo(postId, commentId, hideInboxCommentRequest)

Hide a comment

Hide a comment on a post. Supported by Facebook, Instagram, and Threads. Hidden comments are only visible to the commenter and page admin. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.CommentsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentsApi apiInstance = new CommentsApi(defaultClient);
        String postId = "postId_example"; // String | 
        String commentId = "commentId_example"; // String | 
        HideInboxCommentRequest hideInboxCommentRequest = new HideInboxCommentRequest(); // HideInboxCommentRequest | 
        try {
            ApiResponse<HideInboxComment200Response> response = apiInstance.hideInboxCommentWithHttpInfo(postId, commentId, hideInboxCommentRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentsApi#hideInboxComment");
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
| **commentId** | **String**|  | |
| **hideInboxCommentRequest** | [**HideInboxCommentRequest**](HideInboxCommentRequest.md)|  | |

### Return type

ApiResponse<[**HideInboxComment200Response**](HideInboxComment200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Comment hidden |  -  |
| **400** | Platform does not support hiding comments |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |


## likeInboxComment

> LikeInboxComment200Response likeInboxComment(postId, commentId, likeInboxCommentRequest)

Like a comment

Like or upvote a comment on a post.  **Supported platforms:** Facebook, Bluesky, Reddit  For Bluesky, the &#x60;cid&#x60; (content identifier) is required in the request body. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.CommentsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentsApi apiInstance = new CommentsApi(defaultClient);
        String postId = "postId_example"; // String | 
        String commentId = "commentId_example"; // String | 
        LikeInboxCommentRequest likeInboxCommentRequest = new LikeInboxCommentRequest(); // LikeInboxCommentRequest | 
        try {
            LikeInboxComment200Response result = apiInstance.likeInboxComment(postId, commentId, likeInboxCommentRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentsApi#likeInboxComment");
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
| **commentId** | **String**|  | |
| **likeInboxCommentRequest** | [**LikeInboxCommentRequest**](LikeInboxCommentRequest.md)|  | |

### Return type

[**LikeInboxComment200Response**](LikeInboxComment200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Comment liked |  -  |
| **400** | Platform does not support liking comments |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |

## likeInboxCommentWithHttpInfo

> ApiResponse<LikeInboxComment200Response> likeInboxComment likeInboxCommentWithHttpInfo(postId, commentId, likeInboxCommentRequest)

Like a comment

Like or upvote a comment on a post.  **Supported platforms:** Facebook, Bluesky, Reddit  For Bluesky, the &#x60;cid&#x60; (content identifier) is required in the request body. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.CommentsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentsApi apiInstance = new CommentsApi(defaultClient);
        String postId = "postId_example"; // String | 
        String commentId = "commentId_example"; // String | 
        LikeInboxCommentRequest likeInboxCommentRequest = new LikeInboxCommentRequest(); // LikeInboxCommentRequest | 
        try {
            ApiResponse<LikeInboxComment200Response> response = apiInstance.likeInboxCommentWithHttpInfo(postId, commentId, likeInboxCommentRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentsApi#likeInboxComment");
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
| **commentId** | **String**|  | |
| **likeInboxCommentRequest** | [**LikeInboxCommentRequest**](LikeInboxCommentRequest.md)|  | |

### Return type

ApiResponse<[**LikeInboxComment200Response**](LikeInboxComment200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Comment liked |  -  |
| **400** | Platform does not support liking comments |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |


## listInboxComments

> ListInboxComments200Response listInboxComments(profileId, platform, minComments, since, sortBy, sortOrder, limit, cursor, accountId)

List posts with comments across all accounts

Fetch posts with their comment counts from all connected accounts. Aggregates data from multiple accounts in a single API call.  **Supported platforms:** Facebook, Instagram, Bluesky, YouTube, LinkedIn, Reddit, TikTok (write-only) 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.CommentsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentsApi apiInstance = new CommentsApi(defaultClient);
        String profileId = "profileId_example"; // String | Filter by profile ID
        String platform = "facebook"; // String | Filter by platform
        Integer minComments = 56; // Integer | Minimum comment count
        OffsetDateTime since = OffsetDateTime.now(); // OffsetDateTime | Posts created after this date
        String sortBy = "date"; // String | Sort field
        String sortOrder = "asc"; // String | Sort order
        Integer limit = 50; // Integer | 
        String cursor = "cursor_example"; // String | 
        String accountId = "accountId_example"; // String | Filter by specific social account ID
        try {
            ListInboxComments200Response result = apiInstance.listInboxComments(profileId, platform, minComments, since, sortBy, sortOrder, limit, cursor, accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentsApi#listInboxComments");
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
| **profileId** | **String**| Filter by profile ID | [optional] |
| **platform** | **String**| Filter by platform | [optional] [enum: facebook, instagram, youtube, linkedin, reddit, bluesky, tiktok] |
| **minComments** | **Integer**| Minimum comment count | [optional] |
| **since** | **OffsetDateTime**| Posts created after this date | [optional] |
| **sortBy** | **String**| Sort field | [optional] [default to date] [enum: date, comments] |
| **sortOrder** | **String**| Sort order | [optional] [default to desc] [enum: asc, desc] |
| **limit** | **Integer**|  | [optional] [default to 50] |
| **cursor** | **String**|  | [optional] |
| **accountId** | **String**| Filter by specific social account ID | [optional] |

### Return type

[**ListInboxComments200Response**](ListInboxComments200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Aggregated posts with comments |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |

## listInboxCommentsWithHttpInfo

> ApiResponse<ListInboxComments200Response> listInboxComments listInboxCommentsWithHttpInfo(profileId, platform, minComments, since, sortBy, sortOrder, limit, cursor, accountId)

List posts with comments across all accounts

Fetch posts with their comment counts from all connected accounts. Aggregates data from multiple accounts in a single API call.  **Supported platforms:** Facebook, Instagram, Bluesky, YouTube, LinkedIn, Reddit, TikTok (write-only) 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.CommentsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentsApi apiInstance = new CommentsApi(defaultClient);
        String profileId = "profileId_example"; // String | Filter by profile ID
        String platform = "facebook"; // String | Filter by platform
        Integer minComments = 56; // Integer | Minimum comment count
        OffsetDateTime since = OffsetDateTime.now(); // OffsetDateTime | Posts created after this date
        String sortBy = "date"; // String | Sort field
        String sortOrder = "asc"; // String | Sort order
        Integer limit = 50; // Integer | 
        String cursor = "cursor_example"; // String | 
        String accountId = "accountId_example"; // String | Filter by specific social account ID
        try {
            ApiResponse<ListInboxComments200Response> response = apiInstance.listInboxCommentsWithHttpInfo(profileId, platform, minComments, since, sortBy, sortOrder, limit, cursor, accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentsApi#listInboxComments");
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
| **profileId** | **String**| Filter by profile ID | [optional] |
| **platform** | **String**| Filter by platform | [optional] [enum: facebook, instagram, youtube, linkedin, reddit, bluesky, tiktok] |
| **minComments** | **Integer**| Minimum comment count | [optional] |
| **since** | **OffsetDateTime**| Posts created after this date | [optional] |
| **sortBy** | **String**| Sort field | [optional] [default to date] [enum: date, comments] |
| **sortOrder** | **String**| Sort order | [optional] [default to desc] [enum: asc, desc] |
| **limit** | **Integer**|  | [optional] [default to 50] |
| **cursor** | **String**|  | [optional] |
| **accountId** | **String**| Filter by specific social account ID | [optional] |

### Return type

ApiResponse<[**ListInboxComments200Response**](ListInboxComments200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Aggregated posts with comments |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |


## replyToInboxPost

> ReplyToInboxPost200Response replyToInboxPost(postId, replyToInboxPostRequest)

Reply to a post or comment

Post a reply to a post or specific comment. Requires accountId in request body.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.CommentsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentsApi apiInstance = new CommentsApi(defaultClient);
        String postId = "postId_example"; // String | 
        ReplyToInboxPostRequest replyToInboxPostRequest = new ReplyToInboxPostRequest(); // ReplyToInboxPostRequest | 
        try {
            ReplyToInboxPost200Response result = apiInstance.replyToInboxPost(postId, replyToInboxPostRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentsApi#replyToInboxPost");
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
| **replyToInboxPostRequest** | [**ReplyToInboxPostRequest**](ReplyToInboxPostRequest.md)|  | |

### Return type

[**ReplyToInboxPost200Response**](ReplyToInboxPost200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Reply posted |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |

## replyToInboxPostWithHttpInfo

> ApiResponse<ReplyToInboxPost200Response> replyToInboxPost replyToInboxPostWithHttpInfo(postId, replyToInboxPostRequest)

Reply to a post or comment

Post a reply to a post or specific comment. Requires accountId in request body.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.CommentsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentsApi apiInstance = new CommentsApi(defaultClient);
        String postId = "postId_example"; // String | 
        ReplyToInboxPostRequest replyToInboxPostRequest = new ReplyToInboxPostRequest(); // ReplyToInboxPostRequest | 
        try {
            ApiResponse<ReplyToInboxPost200Response> response = apiInstance.replyToInboxPostWithHttpInfo(postId, replyToInboxPostRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentsApi#replyToInboxPost");
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
| **replyToInboxPostRequest** | [**ReplyToInboxPostRequest**](ReplyToInboxPostRequest.md)|  | |

### Return type

ApiResponse<[**ReplyToInboxPost200Response**](ReplyToInboxPost200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Reply posted |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |


## sendPrivateReplyToComment

> SendPrivateReplyToComment200Response sendPrivateReplyToComment(postId, commentId, sendPrivateReplyToCommentRequest)

Send private reply to comment author

Send a private direct message to the author of a comment on your post. This is useful for handling customer inquiries or sensitive matters privately.  **Supported platforms:** Instagram only  **Limitations:** - Instagram only allows ONE private reply per comment - Must be sent within 7 days of the comment being posted - Only works for comments on posts owned by the connected account - Message goes to the user&#39;s Inbox (if they follow you) or Message Requests (if they don&#39;t) - Requires &#x60;instagram_business_manage_messages&#x60; permission (already included in Late&#39;s OAuth)  **Note:** This does not create a conversation thread until the user replies back. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.CommentsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentsApi apiInstance = new CommentsApi(defaultClient);
        String postId = "postId_example"; // String | The Instagram media/post ID
        String commentId = "commentId_example"; // String | The comment ID to send a private reply to
        SendPrivateReplyToCommentRequest sendPrivateReplyToCommentRequest = new SendPrivateReplyToCommentRequest(); // SendPrivateReplyToCommentRequest | 
        try {
            SendPrivateReplyToComment200Response result = apiInstance.sendPrivateReplyToComment(postId, commentId, sendPrivateReplyToCommentRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentsApi#sendPrivateReplyToComment");
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
| **postId** | **String**| The Instagram media/post ID | |
| **commentId** | **String**| The comment ID to send a private reply to | |
| **sendPrivateReplyToCommentRequest** | [**SendPrivateReplyToCommentRequest**](SendPrivateReplyToCommentRequest.md)|  | |

### Return type

[**SendPrivateReplyToComment200Response**](SendPrivateReplyToComment200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Private reply sent successfully |  -  |
| **400** | Bad request |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |
| **404** | Account not found |  -  |

## sendPrivateReplyToCommentWithHttpInfo

> ApiResponse<SendPrivateReplyToComment200Response> sendPrivateReplyToComment sendPrivateReplyToCommentWithHttpInfo(postId, commentId, sendPrivateReplyToCommentRequest)

Send private reply to comment author

Send a private direct message to the author of a comment on your post. This is useful for handling customer inquiries or sensitive matters privately.  **Supported platforms:** Instagram only  **Limitations:** - Instagram only allows ONE private reply per comment - Must be sent within 7 days of the comment being posted - Only works for comments on posts owned by the connected account - Message goes to the user&#39;s Inbox (if they follow you) or Message Requests (if they don&#39;t) - Requires &#x60;instagram_business_manage_messages&#x60; permission (already included in Late&#39;s OAuth)  **Note:** This does not create a conversation thread until the user replies back. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.CommentsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentsApi apiInstance = new CommentsApi(defaultClient);
        String postId = "postId_example"; // String | The Instagram media/post ID
        String commentId = "commentId_example"; // String | The comment ID to send a private reply to
        SendPrivateReplyToCommentRequest sendPrivateReplyToCommentRequest = new SendPrivateReplyToCommentRequest(); // SendPrivateReplyToCommentRequest | 
        try {
            ApiResponse<SendPrivateReplyToComment200Response> response = apiInstance.sendPrivateReplyToCommentWithHttpInfo(postId, commentId, sendPrivateReplyToCommentRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentsApi#sendPrivateReplyToComment");
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
| **postId** | **String**| The Instagram media/post ID | |
| **commentId** | **String**| The comment ID to send a private reply to | |
| **sendPrivateReplyToCommentRequest** | [**SendPrivateReplyToCommentRequest**](SendPrivateReplyToCommentRequest.md)|  | |

### Return type

ApiResponse<[**SendPrivateReplyToComment200Response**](SendPrivateReplyToComment200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Private reply sent successfully |  -  |
| **400** | Bad request |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |
| **404** | Account not found |  -  |


## unhideInboxComment

> HideInboxComment200Response unhideInboxComment(postId, commentId, accountId)

Unhide a comment

Unhide a previously hidden comment. Supported by Facebook, Instagram, and Threads. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.CommentsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentsApi apiInstance = new CommentsApi(defaultClient);
        String postId = "postId_example"; // String | 
        String commentId = "commentId_example"; // String | 
        String accountId = "accountId_example"; // String | 
        try {
            HideInboxComment200Response result = apiInstance.unhideInboxComment(postId, commentId, accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentsApi#unhideInboxComment");
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
| **commentId** | **String**|  | |
| **accountId** | **String**|  | |

### Return type

[**HideInboxComment200Response**](HideInboxComment200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Comment unhidden |  -  |
| **400** | Platform does not support unhiding comments |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |

## unhideInboxCommentWithHttpInfo

> ApiResponse<HideInboxComment200Response> unhideInboxComment unhideInboxCommentWithHttpInfo(postId, commentId, accountId)

Unhide a comment

Unhide a previously hidden comment. Supported by Facebook, Instagram, and Threads. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.CommentsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentsApi apiInstance = new CommentsApi(defaultClient);
        String postId = "postId_example"; // String | 
        String commentId = "commentId_example"; // String | 
        String accountId = "accountId_example"; // String | 
        try {
            ApiResponse<HideInboxComment200Response> response = apiInstance.unhideInboxCommentWithHttpInfo(postId, commentId, accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentsApi#unhideInboxComment");
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
| **commentId** | **String**|  | |
| **accountId** | **String**|  | |

### Return type

ApiResponse<[**HideInboxComment200Response**](HideInboxComment200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Comment unhidden |  -  |
| **400** | Platform does not support unhiding comments |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |


## unlikeInboxComment

> UnlikeInboxComment200Response unlikeInboxComment(postId, commentId, accountId, likeUri)

Unlike a comment

Remove a like from a comment.  **Supported platforms:** Facebook, Bluesky, Reddit  For Bluesky, the &#x60;likeUri&#x60; query parameter is required. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.CommentsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentsApi apiInstance = new CommentsApi(defaultClient);
        String postId = "postId_example"; // String | 
        String commentId = "commentId_example"; // String | 
        String accountId = "accountId_example"; // String | 
        String likeUri = "likeUri_example"; // String | (Bluesky only) The like URI returned when liking
        try {
            UnlikeInboxComment200Response result = apiInstance.unlikeInboxComment(postId, commentId, accountId, likeUri);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentsApi#unlikeInboxComment");
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
| **commentId** | **String**|  | |
| **accountId** | **String**|  | |
| **likeUri** | **String**| (Bluesky only) The like URI returned when liking | [optional] |

### Return type

[**UnlikeInboxComment200Response**](UnlikeInboxComment200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Comment unliked |  -  |
| **400** | Platform does not support unliking comments |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |

## unlikeInboxCommentWithHttpInfo

> ApiResponse<UnlikeInboxComment200Response> unlikeInboxComment unlikeInboxCommentWithHttpInfo(postId, commentId, accountId, likeUri)

Unlike a comment

Remove a like from a comment.  **Supported platforms:** Facebook, Bluesky, Reddit  For Bluesky, the &#x60;likeUri&#x60; query parameter is required. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.CommentsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        CommentsApi apiInstance = new CommentsApi(defaultClient);
        String postId = "postId_example"; // String | 
        String commentId = "commentId_example"; // String | 
        String accountId = "accountId_example"; // String | 
        String likeUri = "likeUri_example"; // String | (Bluesky only) The like URI returned when liking
        try {
            ApiResponse<UnlikeInboxComment200Response> response = apiInstance.unlikeInboxCommentWithHttpInfo(postId, commentId, accountId, likeUri);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling CommentsApi#unlikeInboxComment");
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
| **commentId** | **String**|  | |
| **accountId** | **String**|  | |
| **likeUri** | **String**| (Bluesky only) The like URI returned when liking | [optional] |

### Return type

ApiResponse<[**UnlikeInboxComment200Response**](UnlikeInboxComment200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Comment unliked |  -  |
| **400** | Platform does not support unliking comments |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |

