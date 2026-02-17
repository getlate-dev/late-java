# ReviewsApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**deleteInboxReviewReply**](ReviewsApi.md#deleteInboxReviewReply) | **DELETE** /v1/inbox/reviews/{reviewId}/reply | Delete review reply |
| [**deleteInboxReviewReplyWithHttpInfo**](ReviewsApi.md#deleteInboxReviewReplyWithHttpInfo) | **DELETE** /v1/inbox/reviews/{reviewId}/reply | Delete review reply |
| [**listInboxReviews**](ReviewsApi.md#listInboxReviews) | **GET** /v1/inbox/reviews | List reviews |
| [**listInboxReviewsWithHttpInfo**](ReviewsApi.md#listInboxReviewsWithHttpInfo) | **GET** /v1/inbox/reviews | List reviews |
| [**replyToInboxReview**](ReviewsApi.md#replyToInboxReview) | **POST** /v1/inbox/reviews/{reviewId}/reply | Reply to review |
| [**replyToInboxReviewWithHttpInfo**](ReviewsApi.md#replyToInboxReviewWithHttpInfo) | **POST** /v1/inbox/reviews/{reviewId}/reply | Reply to review |



## deleteInboxReviewReply

> DeleteInboxReviewReply200Response deleteInboxReviewReply(reviewId, deleteInboxReviewReplyRequest)

Delete review reply

Delete a reply to a review (Google Business only). Requires accountId in request body.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ReviewsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ReviewsApi apiInstance = new ReviewsApi(defaultClient);
        String reviewId = "reviewId_example"; // String | 
        DeleteInboxReviewReplyRequest deleteInboxReviewReplyRequest = new DeleteInboxReviewReplyRequest(); // DeleteInboxReviewReplyRequest | 
        try {
            DeleteInboxReviewReply200Response result = apiInstance.deleteInboxReviewReply(reviewId, deleteInboxReviewReplyRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReviewsApi#deleteInboxReviewReply");
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
| **reviewId** | **String**|  | |
| **deleteInboxReviewReplyRequest** | [**DeleteInboxReviewReplyRequest**](DeleteInboxReviewReplyRequest.md)|  | |

### Return type

[**DeleteInboxReviewReply200Response**](DeleteInboxReviewReply200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Reply deleted |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |

## deleteInboxReviewReplyWithHttpInfo

> ApiResponse<DeleteInboxReviewReply200Response> deleteInboxReviewReply deleteInboxReviewReplyWithHttpInfo(reviewId, deleteInboxReviewReplyRequest)

Delete review reply

Delete a reply to a review (Google Business only). Requires accountId in request body.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ReviewsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ReviewsApi apiInstance = new ReviewsApi(defaultClient);
        String reviewId = "reviewId_example"; // String | 
        DeleteInboxReviewReplyRequest deleteInboxReviewReplyRequest = new DeleteInboxReviewReplyRequest(); // DeleteInboxReviewReplyRequest | 
        try {
            ApiResponse<DeleteInboxReviewReply200Response> response = apiInstance.deleteInboxReviewReplyWithHttpInfo(reviewId, deleteInboxReviewReplyRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ReviewsApi#deleteInboxReviewReply");
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
| **reviewId** | **String**|  | |
| **deleteInboxReviewReplyRequest** | [**DeleteInboxReviewReplyRequest**](DeleteInboxReviewReplyRequest.md)|  | |

### Return type

ApiResponse<[**DeleteInboxReviewReply200Response**](DeleteInboxReviewReply200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Reply deleted |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |


## listInboxReviews

> ListInboxReviews200Response listInboxReviews(profileId, platform, minRating, maxRating, hasReply, sortBy, sortOrder, limit, cursor, accountId)

List reviews

Fetch reviews from all connected Facebook Pages and Google Business accounts. Aggregates data with filtering and sorting options. Supported platforms: Facebook, Google Business. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ReviewsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ReviewsApi apiInstance = new ReviewsApi(defaultClient);
        String profileId = "profileId_example"; // String | 
        String platform = "facebook"; // String | 
        Integer minRating = 56; // Integer | 
        Integer maxRating = 56; // Integer | 
        Boolean hasReply = true; // Boolean | Filter by reply status
        String sortBy = "date"; // String | 
        String sortOrder = "asc"; // String | 
        Integer limit = 25; // Integer | 
        String cursor = "cursor_example"; // String | 
        String accountId = "accountId_example"; // String | Filter by specific social account ID
        try {
            ListInboxReviews200Response result = apiInstance.listInboxReviews(profileId, platform, minRating, maxRating, hasReply, sortBy, sortOrder, limit, cursor, accountId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReviewsApi#listInboxReviews");
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
| **profileId** | **String**|  | [optional] |
| **platform** | **String**|  | [optional] [enum: facebook, googlebusiness] |
| **minRating** | **Integer**|  | [optional] |
| **maxRating** | **Integer**|  | [optional] |
| **hasReply** | **Boolean**| Filter by reply status | [optional] |
| **sortBy** | **String**|  | [optional] [default to date] [enum: date, rating] |
| **sortOrder** | **String**|  | [optional] [default to desc] [enum: asc, desc] |
| **limit** | **Integer**|  | [optional] [default to 25] |
| **cursor** | **String**|  | [optional] |
| **accountId** | **String**| Filter by specific social account ID | [optional] |

### Return type

[**ListInboxReviews200Response**](ListInboxReviews200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Aggregated reviews |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |

## listInboxReviewsWithHttpInfo

> ApiResponse<ListInboxReviews200Response> listInboxReviews listInboxReviewsWithHttpInfo(profileId, platform, minRating, maxRating, hasReply, sortBy, sortOrder, limit, cursor, accountId)

List reviews

Fetch reviews from all connected Facebook Pages and Google Business accounts. Aggregates data with filtering and sorting options. Supported platforms: Facebook, Google Business. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ReviewsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ReviewsApi apiInstance = new ReviewsApi(defaultClient);
        String profileId = "profileId_example"; // String | 
        String platform = "facebook"; // String | 
        Integer minRating = 56; // Integer | 
        Integer maxRating = 56; // Integer | 
        Boolean hasReply = true; // Boolean | Filter by reply status
        String sortBy = "date"; // String | 
        String sortOrder = "asc"; // String | 
        Integer limit = 25; // Integer | 
        String cursor = "cursor_example"; // String | 
        String accountId = "accountId_example"; // String | Filter by specific social account ID
        try {
            ApiResponse<ListInboxReviews200Response> response = apiInstance.listInboxReviewsWithHttpInfo(profileId, platform, minRating, maxRating, hasReply, sortBy, sortOrder, limit, cursor, accountId);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ReviewsApi#listInboxReviews");
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
| **profileId** | **String**|  | [optional] |
| **platform** | **String**|  | [optional] [enum: facebook, googlebusiness] |
| **minRating** | **Integer**|  | [optional] |
| **maxRating** | **Integer**|  | [optional] |
| **hasReply** | **Boolean**| Filter by reply status | [optional] |
| **sortBy** | **String**|  | [optional] [default to date] [enum: date, rating] |
| **sortOrder** | **String**|  | [optional] [default to desc] [enum: asc, desc] |
| **limit** | **Integer**|  | [optional] [default to 25] |
| **cursor** | **String**|  | [optional] |
| **accountId** | **String**| Filter by specific social account ID | [optional] |

### Return type

ApiResponse<[**ListInboxReviews200Response**](ListInboxReviews200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Aggregated reviews |  -  |
| **401** | Unauthorized |  -  |
| **403** | Inbox addon required |  -  |


## replyToInboxReview

> ReplyToInboxReview200Response replyToInboxReview(reviewId, replyToInboxReviewRequest)

Reply to review

Post a reply to a review. Requires accountId in request body.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ReviewsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ReviewsApi apiInstance = new ReviewsApi(defaultClient);
        String reviewId = "reviewId_example"; // String | Review ID (URL-encoded for Google Business)
        ReplyToInboxReviewRequest replyToInboxReviewRequest = new ReplyToInboxReviewRequest(); // ReplyToInboxReviewRequest | 
        try {
            ReplyToInboxReview200Response result = apiInstance.replyToInboxReview(reviewId, replyToInboxReviewRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling ReviewsApi#replyToInboxReview");
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
| **reviewId** | **String**| Review ID (URL-encoded for Google Business) | |
| **replyToInboxReviewRequest** | [**ReplyToInboxReviewRequest**](ReplyToInboxReviewRequest.md)|  | |

### Return type

[**ReplyToInboxReview200Response**](ReplyToInboxReview200Response.md)


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

## replyToInboxReviewWithHttpInfo

> ApiResponse<ReplyToInboxReview200Response> replyToInboxReview replyToInboxReviewWithHttpInfo(reviewId, replyToInboxReviewRequest)

Reply to review

Post a reply to a review. Requires accountId in request body.

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.ReviewsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        ReviewsApi apiInstance = new ReviewsApi(defaultClient);
        String reviewId = "reviewId_example"; // String | Review ID (URL-encoded for Google Business)
        ReplyToInboxReviewRequest replyToInboxReviewRequest = new ReplyToInboxReviewRequest(); // ReplyToInboxReviewRequest | 
        try {
            ApiResponse<ReplyToInboxReview200Response> response = apiInstance.replyToInboxReviewWithHttpInfo(reviewId, replyToInboxReviewRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling ReviewsApi#replyToInboxReview");
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
| **reviewId** | **String**| Review ID (URL-encoded for Google Business) | |
| **replyToInboxReviewRequest** | [**ReplyToInboxReviewRequest**](ReplyToInboxReviewRequest.md)|  | |

### Return type

ApiResponse<[**ReplyToInboxReview200Response**](ReplyToInboxReview200Response.md)>


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

