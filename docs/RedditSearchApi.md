# RedditSearchApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getRedditFeed**](RedditSearchApi.md#getRedditFeed) | **GET** /v1/reddit/feed | Get subreddit feed |
| [**getRedditFeedWithHttpInfo**](RedditSearchApi.md#getRedditFeedWithHttpInfo) | **GET** /v1/reddit/feed | Get subreddit feed |
| [**searchReddit**](RedditSearchApi.md#searchReddit) | **GET** /v1/reddit/search | Search posts |
| [**searchRedditWithHttpInfo**](RedditSearchApi.md#searchRedditWithHttpInfo) | **GET** /v1/reddit/search | Search posts |



## getRedditFeed

> GetRedditFeed200Response getRedditFeed(accountId, subreddit, sort, limit, after, t)

Get subreddit feed

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.RedditSearchApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        RedditSearchApi apiInstance = new RedditSearchApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        String subreddit = "subreddit_example"; // String | 
        String sort = "hot"; // String | 
        Integer limit = 25; // Integer | 
        String after = "after_example"; // String | 
        String t = "hour"; // String | 
        try {
            GetRedditFeed200Response result = apiInstance.getRedditFeed(accountId, subreddit, sort, limit, after, t);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling RedditSearchApi#getRedditFeed");
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
| **subreddit** | **String**|  | [optional] |
| **sort** | **String**|  | [optional] [default to hot] [enum: hot, new, top, rising] |
| **limit** | **Integer**|  | [optional] [default to 25] |
| **after** | **String**|  | [optional] |
| **t** | **String**|  | [optional] [enum: hour, day, week, month, year, all] |

### Return type

[**GetRedditFeed200Response**](GetRedditFeed200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Feed items |  -  |
| **400** | Missing params |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## getRedditFeedWithHttpInfo

> ApiResponse<GetRedditFeed200Response> getRedditFeed getRedditFeedWithHttpInfo(accountId, subreddit, sort, limit, after, t)

Get subreddit feed

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.RedditSearchApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        RedditSearchApi apiInstance = new RedditSearchApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        String subreddit = "subreddit_example"; // String | 
        String sort = "hot"; // String | 
        Integer limit = 25; // Integer | 
        String after = "after_example"; // String | 
        String t = "hour"; // String | 
        try {
            ApiResponse<GetRedditFeed200Response> response = apiInstance.getRedditFeedWithHttpInfo(accountId, subreddit, sort, limit, after, t);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling RedditSearchApi#getRedditFeed");
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
| **subreddit** | **String**|  | [optional] |
| **sort** | **String**|  | [optional] [default to hot] [enum: hot, new, top, rising] |
| **limit** | **Integer**|  | [optional] [default to 25] |
| **after** | **String**|  | [optional] |
| **t** | **String**|  | [optional] [enum: hour, day, week, month, year, all] |

### Return type

ApiResponse<[**GetRedditFeed200Response**](GetRedditFeed200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Feed items |  -  |
| **400** | Missing params |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |


## searchReddit

> SearchReddit200Response searchReddit(accountId, q, subreddit, restrictSr, sort, limit, after)

Search posts

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.RedditSearchApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        RedditSearchApi apiInstance = new RedditSearchApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        String q = "q_example"; // String | 
        String subreddit = "subreddit_example"; // String | 
        String restrictSr = "0"; // String | 
        String sort = "relevance"; // String | 
        Integer limit = 25; // Integer | 
        String after = "after_example"; // String | 
        try {
            SearchReddit200Response result = apiInstance.searchReddit(accountId, q, subreddit, restrictSr, sort, limit, after);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling RedditSearchApi#searchReddit");
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
| **q** | **String**|  | |
| **subreddit** | **String**|  | [optional] |
| **restrictSr** | **String**|  | [optional] [enum: 0, 1] |
| **sort** | **String**|  | [optional] [default to new] [enum: relevance, hot, top, new, comments] |
| **limit** | **Integer**|  | [optional] [default to 25] |
| **after** | **String**|  | [optional] |

### Return type

[**SearchReddit200Response**](SearchReddit200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Search results |  -  |
| **400** | Missing params |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

## searchRedditWithHttpInfo

> ApiResponse<SearchReddit200Response> searchReddit searchRedditWithHttpInfo(accountId, q, subreddit, restrictSr, sort, limit, after)

Search posts

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.RedditSearchApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        RedditSearchApi apiInstance = new RedditSearchApi(defaultClient);
        String accountId = "accountId_example"; // String | 
        String q = "q_example"; // String | 
        String subreddit = "subreddit_example"; // String | 
        String restrictSr = "0"; // String | 
        String sort = "relevance"; // String | 
        Integer limit = 25; // Integer | 
        String after = "after_example"; // String | 
        try {
            ApiResponse<SearchReddit200Response> response = apiInstance.searchRedditWithHttpInfo(accountId, q, subreddit, restrictSr, sort, limit, after);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling RedditSearchApi#searchReddit");
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
| **q** | **String**|  | |
| **subreddit** | **String**|  | [optional] |
| **restrictSr** | **String**|  | [optional] [enum: 0, 1] |
| **sort** | **String**|  | [optional] [default to new] [enum: relevance, hot, top, new, comments] |
| **limit** | **Integer**|  | [optional] [default to 25] |
| **after** | **String**|  | [optional] |

### Return type

ApiResponse<[**SearchReddit200Response**](SearchReddit200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Search results |  -  |
| **400** | Missing params |  -  |
| **401** | Unauthorized |  -  |
| **404** | Account not found |  -  |

