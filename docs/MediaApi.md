# MediaApi

All URIs are relative to *https://zernio.com/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getMediaPresignedUrl**](MediaApi.md#getMediaPresignedUrl) | **POST** /v1/media/presign | Get upload URL |
| [**getMediaPresignedUrlWithHttpInfo**](MediaApi.md#getMediaPresignedUrlWithHttpInfo) | **POST** /v1/media/presign | Get upload URL |



## getMediaPresignedUrl

> GetMediaPresignedUrl200Response getMediaPresignedUrl(getMediaPresignedUrlRequest)

Get upload URL

Get a presigned URL to upload files directly to cloud storage (up to 5GB). Returns an uploadUrl and publicUrl. PUT your file to the uploadUrl, then use the publicUrl in your posts.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.MediaApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        MediaApi apiInstance = new MediaApi(defaultClient);
        GetMediaPresignedUrlRequest getMediaPresignedUrlRequest = new GetMediaPresignedUrlRequest(); // GetMediaPresignedUrlRequest | 
        try {
            GetMediaPresignedUrl200Response result = apiInstance.getMediaPresignedUrl(getMediaPresignedUrlRequest);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling MediaApi#getMediaPresignedUrl");
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
| **getMediaPresignedUrlRequest** | [**GetMediaPresignedUrlRequest**](GetMediaPresignedUrlRequest.md)|  | |

### Return type

[**GetMediaPresignedUrl200Response**](GetMediaPresignedUrl200Response.md)


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Presigned URL generated successfully |  -  |
| **400** | Invalid request (missing filename, contentType, or unsupported content type) |  -  |
| **401** | Unauthorized |  -  |

## getMediaPresignedUrlWithHttpInfo

> ApiResponse<GetMediaPresignedUrl200Response> getMediaPresignedUrl getMediaPresignedUrlWithHttpInfo(getMediaPresignedUrlRequest)

Get upload URL

Get a presigned URL to upload files directly to cloud storage (up to 5GB). Returns an uploadUrl and publicUrl. PUT your file to the uploadUrl, then use the publicUrl in your posts.

### Example

```java
// Import classes:
import dev.zernio.ApiClient;
import dev.zernio.ApiException;
import dev.zernio.ApiResponse;
import dev.zernio.Configuration;
import dev.zernio.auth.*;
import dev.zernio.models.*;
import dev.zernio.api.MediaApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://zernio.com/api");
        
        // Configure HTTP bearer authorization: bearerAuth
        HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
        bearerAuth.setBearerToken("BEARER TOKEN");

        MediaApi apiInstance = new MediaApi(defaultClient);
        GetMediaPresignedUrlRequest getMediaPresignedUrlRequest = new GetMediaPresignedUrlRequest(); // GetMediaPresignedUrlRequest | 
        try {
            ApiResponse<GetMediaPresignedUrl200Response> response = apiInstance.getMediaPresignedUrlWithHttpInfo(getMediaPresignedUrlRequest);
            System.out.println("Status code: " + response.getStatusCode());
            System.out.println("Response headers: " + response.getHeaders());
            System.out.println("Response body: " + response.getData());
        } catch (ApiException e) {
            System.err.println("Exception when calling MediaApi#getMediaPresignedUrl");
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
| **getMediaPresignedUrlRequest** | [**GetMediaPresignedUrlRequest**](GetMediaPresignedUrlRequest.md)|  | |

### Return type

ApiResponse<[**GetMediaPresignedUrl200Response**](GetMediaPresignedUrl200Response.md)>


### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Presigned URL generated successfully |  -  |
| **400** | Invalid request (missing filename, contentType, or unsupported content type) |  -  |
| **401** | Unauthorized |  -  |

