# TwitterEngagementApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**bookmarkPost**](TwitterEngagementApi.md#bookmarkPost) | **POST** /v1/twitter/bookmark | Bookmark a tweet |
| [**bookmarkPostWithHttpInfo**](TwitterEngagementApi.md#bookmarkPostWithHttpInfo) | **POST** /v1/twitter/bookmark | Bookmark a tweet |
| [**followUser**](TwitterEngagementApi.md#followUser) | **POST** /v1/twitter/follow | Follow a user |
| [**followUserWithHttpInfo**](TwitterEngagementApi.md#followUserWithHttpInfo) | **POST** /v1/twitter/follow | Follow a user |
| [**removeBookmark**](TwitterEngagementApi.md#removeBookmark) | **DELETE** /v1/twitter/bookmark | Remove bookmark |
| [**removeBookmarkWithHttpInfo**](TwitterEngagementApi.md#removeBookmarkWithHttpInfo) | **DELETE** /v1/twitter/bookmark | Remove bookmark |
| [**retweetPost**](TwitterEngagementApi.md#retweetPost) | **POST** /v1/twitter/retweet | Retweet a post |
| [**retweetPostWithHttpInfo**](TwitterEngagementApi.md#retweetPostWithHttpInfo) | **POST** /v1/twitter/retweet | Retweet a post |
| [**undoRetweet**](TwitterEngagementApi.md#undoRetweet) | **DELETE** /v1/twitter/retweet | Undo retweet |
| [**undoRetweetWithHttpInfo**](TwitterEngagementApi.md#undoRetweetWithHttpInfo) | **DELETE** /v1/twitter/retweet | Undo retweet |
| [**unfollowUser**](TwitterEngagementApi.md#unfollowUser) | **DELETE** /v1/twitter/follow | Unfollow a user |
| [**unfollowUserWithHttpInfo**](TwitterEngagementApi.md#unfollowUserWithHttpInfo) | **DELETE** /v1/twitter/follow | Unfollow a user |



## bookmarkPost

> BookmarkPost200Response bookmarkPost(bookmarkPostRequest)

Bookmark a tweet

Bookmark a tweet by ID. Requires the bookmark.write OAuth scope. Rate limit: 50 requests per 15-min window. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.TwitterEngagementApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        TwitterEngagementApi apiInstance = new TwitterEngagementApi(defaultClient);
        BookmarkPostRequest bookmarkPostRequest = new BookmarkPostRequest(); // BookmarkPostRequest | 
        try {
            BookmarkPost200Response result = apiInstance.bookmarkPost(bookmarkPostRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling TwitterEngagementApi#bookmarkPost");
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
| **bookmarkPostRequest** | [**BookmarkPostRequest**](BookmarkPostRequest.md)|  | |

### Return type

[**BookmarkPost200Response**](BookmarkPost200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Tweet bookmarked |  -  |
| **400** | Bad request or platform limitation |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## bookmarkPostWithHttpInfo

> ApiResponse<BookmarkPost200Response> bookmarkPost bookmarkPostWithHttpInfo(bookmarkPostRequest)

Bookmark a tweet

Bookmark a tweet by ID. Requires the bookmark.write OAuth scope. Rate limit: 50 requests per 15-min window. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.TwitterEngagementApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        TwitterEngagementApi apiInstance = new TwitterEngagementApi(defaultClient);
        BookmarkPostRequest bookmarkPostRequest = new BookmarkPostRequest(); // BookmarkPostRequest | 
        try {
            ApiResponse<BookmarkPost200Response> response = apiInstance.bookmarkPostWithHttpInfo(bookmarkPostRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling TwitterEngagementApi#bookmarkPost");
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
| **bookmarkPostRequest** | [**BookmarkPostRequest**](BookmarkPostRequest.md)|  | |

### Return type

ApiResponse<[**BookmarkPost200Response**](BookmarkPost200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Tweet bookmarked |  -  |
| **400** | Bad request or platform limitation |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |


## followUser

> FollowUser200Response followUser(followUserRequest)

Follow a user

Follow a user on X/Twitter. Requires the follows.write OAuth scope. For protected accounts, a follow request is sent instead (pending_follow will be true). 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.TwitterEngagementApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        TwitterEngagementApi apiInstance = new TwitterEngagementApi(defaultClient);
        FollowUserRequest followUserRequest = new FollowUserRequest(); // FollowUserRequest | 
        try {
            FollowUser200Response result = apiInstance.followUser(followUserRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling TwitterEngagementApi#followUser");
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
| **followUserRequest** | [**FollowUserRequest**](FollowUserRequest.md)|  | |

### Return type

[**FollowUser200Response**](FollowUser200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User followed or follow request sent |  -  |
| **400** | Bad request or platform limitation |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## followUserWithHttpInfo

> ApiResponse<FollowUser200Response> followUser followUserWithHttpInfo(followUserRequest)

Follow a user

Follow a user on X/Twitter. Requires the follows.write OAuth scope. For protected accounts, a follow request is sent instead (pending_follow will be true). 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.TwitterEngagementApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        TwitterEngagementApi apiInstance = new TwitterEngagementApi(defaultClient);
        FollowUserRequest followUserRequest = new FollowUserRequest(); // FollowUserRequest | 
        try {
            ApiResponse<FollowUser200Response> response = apiInstance.followUserWithHttpInfo(followUserRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling TwitterEngagementApi#followUser");
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
| **followUserRequest** | [**FollowUserRequest**](FollowUserRequest.md)|  | |

### Return type

ApiResponse<[**FollowUser200Response**](FollowUser200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User followed or follow request sent |  -  |
| **400** | Bad request or platform limitation |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |


## removeBookmark

> RemoveBookmark200Response removeBookmark(accountId, tweetId)

Remove bookmark

Remove a bookmark from a tweet. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.TwitterEngagementApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        TwitterEngagementApi apiInstance = new TwitterEngagementApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        String tweetId = "tweetId_example"; // String | The ID of the tweet to unbookmark
        try {
            RemoveBookmark200Response result = apiInstance.removeBookmark(accountId, tweetId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling TwitterEngagementApi#removeBookmark");
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
| **tweetId** | **String**| The ID of the tweet to unbookmark | |

### Return type

[**RemoveBookmark200Response**](RemoveBookmark200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Bookmark removed |  -  |
| **400** | Bad request |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## removeBookmarkWithHttpInfo

> ApiResponse<RemoveBookmark200Response> removeBookmark removeBookmarkWithHttpInfo(accountId, tweetId)

Remove bookmark

Remove a bookmark from a tweet. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.TwitterEngagementApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        TwitterEngagementApi apiInstance = new TwitterEngagementApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        String tweetId = "tweetId_example"; // String | The ID of the tweet to unbookmark
        try {
            ApiResponse<RemoveBookmark200Response> response = apiInstance.removeBookmarkWithHttpInfo(accountId, tweetId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling TwitterEngagementApi#removeBookmark");
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
| **tweetId** | **String**| The ID of the tweet to unbookmark | |

### Return type

ApiResponse<[**RemoveBookmark200Response**](RemoveBookmark200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Bookmark removed |  -  |
| **400** | Bad request |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |


## retweetPost

> RetweetPost200Response retweetPost(retweetPostRequest)

Retweet a post

Retweet (repost) a tweet by ID. Rate limit: 50 requests per 15-min window. Shares the 300/3hr creation limit with tweet creation. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.TwitterEngagementApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        TwitterEngagementApi apiInstance = new TwitterEngagementApi(defaultClient);
        RetweetPostRequest retweetPostRequest = new RetweetPostRequest(); // RetweetPostRequest | 
        try {
            RetweetPost200Response result = apiInstance.retweetPost(retweetPostRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling TwitterEngagementApi#retweetPost");
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
| **retweetPostRequest** | [**RetweetPostRequest**](RetweetPostRequest.md)|  | |

### Return type

[**RetweetPost200Response**](RetweetPost200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Tweet retweeted |  -  |
| **400** | Bad request or platform limitation |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## retweetPostWithHttpInfo

> ApiResponse<RetweetPost200Response> retweetPost retweetPostWithHttpInfo(retweetPostRequest)

Retweet a post

Retweet (repost) a tweet by ID. Rate limit: 50 requests per 15-min window. Shares the 300/3hr creation limit with tweet creation. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.TwitterEngagementApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        TwitterEngagementApi apiInstance = new TwitterEngagementApi(defaultClient);
        RetweetPostRequest retweetPostRequest = new RetweetPostRequest(); // RetweetPostRequest | 
        try {
            ApiResponse<RetweetPost200Response> response = apiInstance.retweetPostWithHttpInfo(retweetPostRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling TwitterEngagementApi#retweetPost");
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
| **retweetPostRequest** | [**RetweetPostRequest**](RetweetPostRequest.md)|  | |

### Return type

ApiResponse<[**RetweetPost200Response**](RetweetPost200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Tweet retweeted |  -  |
| **400** | Bad request or platform limitation |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |


## undoRetweet

> UndoRetweet200Response undoRetweet(accountId, tweetId)

Undo retweet

Undo a retweet (un-repost a tweet). 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.TwitterEngagementApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        TwitterEngagementApi apiInstance = new TwitterEngagementApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        String tweetId = "tweetId_example"; // String | The ID of the original tweet to un-retweet
        try {
            UndoRetweet200Response result = apiInstance.undoRetweet(accountId, tweetId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling TwitterEngagementApi#undoRetweet");
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
| **tweetId** | **String**| The ID of the original tweet to un-retweet | |

### Return type

[**UndoRetweet200Response**](UndoRetweet200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Retweet undone |  -  |
| **400** | Bad request |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## undoRetweetWithHttpInfo

> ApiResponse<UndoRetweet200Response> undoRetweet undoRetweetWithHttpInfo(accountId, tweetId)

Undo retweet

Undo a retweet (un-repost a tweet). 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.TwitterEngagementApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        TwitterEngagementApi apiInstance = new TwitterEngagementApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        String tweetId = "tweetId_example"; // String | The ID of the original tweet to un-retweet
        try {
            ApiResponse<UndoRetweet200Response> response = apiInstance.undoRetweetWithHttpInfo(accountId, tweetId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling TwitterEngagementApi#undoRetweet");
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
| **tweetId** | **String**| The ID of the original tweet to un-retweet | |

### Return type

ApiResponse<[**UndoRetweet200Response**](UndoRetweet200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Retweet undone |  -  |
| **400** | Bad request |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |


## unfollowUser

> UnfollowUser200Response unfollowUser(accountId, targetUserId)

Unfollow a user

Unfollow a user on X/Twitter. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.TwitterEngagementApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        TwitterEngagementApi apiInstance = new TwitterEngagementApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        String targetUserId = "targetUserId_example"; // String | The Twitter ID of the user to unfollow
        try {
            UnfollowUser200Response result = apiInstance.unfollowUser(accountId, targetUserId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling TwitterEngagementApi#unfollowUser");
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
| **targetUserId** | **String**| The Twitter ID of the user to unfollow | |

### Return type

[**UnfollowUser200Response**](UnfollowUser200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User unfollowed |  -  |
| **400** | Bad request |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## unfollowUserWithHttpInfo

> ApiResponse<UnfollowUser200Response> unfollowUser unfollowUserWithHttpInfo(accountId, targetUserId)

Unfollow a user

Unfollow a user on X/Twitter. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.TwitterEngagementApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        TwitterEngagementApi apiInstance = new TwitterEngagementApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        String targetUserId = "targetUserId_example"; // String | The Twitter ID of the user to unfollow
        try {
            ApiResponse<UnfollowUser200Response> response = apiInstance.unfollowUserWithHttpInfo(accountId, targetUserId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling TwitterEngagementApi#unfollowUser");
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
| **targetUserId** | **String**| The Twitter ID of the user to unfollow | |

### Return type

ApiResponse<[**UnfollowUser200Response**](UnfollowUser200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User unfollowed |  -  |
| **400** | Bad request |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

