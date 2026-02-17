# GmbReviewsApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getGoogleBusinessReviews**](GmbReviewsApi.md#getGoogleBusinessReviews) | **GET** /v1/accounts/{accountId}/gmb-reviews | Get reviews |
| [**getGoogleBusinessReviewsWithHttpInfo**](GmbReviewsApi.md#getGoogleBusinessReviewsWithHttpInfo) | **GET** /v1/accounts/{accountId}/gmb-reviews | Get reviews |



## getGoogleBusinessReviews

> GetGoogleBusinessReviews200Response getGoogleBusinessReviews(accountId, pageSize, pageToken)

Get reviews

Fetches reviews for a connected Google Business Profile account. Returns all reviews including reviewer info, star rating, comment text, owner reply, and timestamps. Use pagination via nextPageToken for locations with many reviews. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbReviewsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbReviewsApi apiInstance = new GmbReviewsApi(defaultClient);
        String accountId = "accountId_example"; // String | The Late account ID (from /v1/accounts)
        Integer pageSize = 50; // Integer | Number of reviews to fetch per page (max 50)
        String pageToken = "pageToken_example"; // String | Pagination token from previous response
        try {
            GetGoogleBusinessReviews200Response result = apiInstance.getGoogleBusinessReviews(accountId, pageSize, pageToken);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbReviewsApi#getGoogleBusinessReviews");
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
| **accountId** | **String**| The Late account ID (from /v1/accounts) | |
| **pageSize** | **Integer**| Number of reviews to fetch per page (max 50) | [optional] [default to 50] |
| **pageToken** | **String**| Pagination token from previous response | [optional] |

### Return type

[**GetGoogleBusinessReviews200Response**](GetGoogleBusinessReviews200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Reviews fetched successfully |  -  |
| **400** | Invalid request - not a Google Business account or missing location |  -  |
| **401** | Unauthorized or token expired |  -  |
| **403** | Permission denied for this location |  -  |
| **404** | Resource not found |  -  |
| **500** | Failed to fetch reviews |  -  |

## getGoogleBusinessReviewsWithHttpInfo

> ApiResponse<GetGoogleBusinessReviews200Response> getGoogleBusinessReviews getGoogleBusinessReviewsWithHttpInfo(accountId, pageSize, pageToken)

Get reviews

Fetches reviews for a connected Google Business Profile account. Returns all reviews including reviewer info, star rating, comment text, owner reply, and timestamps. Use pagination via nextPageToken for locations with many reviews. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.GmbReviewsApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        GmbReviewsApi apiInstance = new GmbReviewsApi(defaultClient);
        String accountId = "accountId_example"; // String | The Late account ID (from /v1/accounts)
        Integer pageSize = 50; // Integer | Number of reviews to fetch per page (max 50)
        String pageToken = "pageToken_example"; // String | Pagination token from previous response
        try {
            ApiResponse<GetGoogleBusinessReviews200Response> response = apiInstance.getGoogleBusinessReviewsWithHttpInfo(accountId, pageSize, pageToken);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling GmbReviewsApi#getGoogleBusinessReviews");
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
| **accountId** | **String**| The Late account ID (from /v1/accounts) | |
| **pageSize** | **Integer**| Number of reviews to fetch per page (max 50) | [optional] [default to 50] |
| **pageToken** | **String**| Pagination token from previous response | [optional] |

### Return type

ApiResponse<[**GetGoogleBusinessReviews200Response**](GetGoogleBusinessReviews200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Reviews fetched successfully |  -  |
| **400** | Invalid request - not a Google Business account or missing location |  -  |
| **401** | Unauthorized or token expired |  -  |
| **403** | Permission denied for this location |  -  |
| **404** | Resource not found |  -  |
| **500** | Failed to fetch reviews |  -  |

