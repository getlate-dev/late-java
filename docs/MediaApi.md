# MediaApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getMediaPresignedUrl**](MediaApi.md#getMediaPresignedUrl) | **POST** /v1/media/presign | Get presigned upload URL |
| [**getMediaPresignedUrlWithHttpInfo**](MediaApi.md#getMediaPresignedUrlWithHttpInfo) | **POST** /v1/media/presign | Get presigned upload URL |



## getMediaPresignedUrl

> GetMediaPresignedUrl200Response getMediaPresignedUrl(getMediaPresignedUrlRequest)

Get presigned upload URL

Get a presigned URL to upload files directly to cloud storage. Supports files up to 5GB.  How it works: call this endpoint with the filename and content type, receive an uploadUrl (presigned) and publicUrl, PUT your file directly to the uploadUrl, then use the publicUrl in your posts. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.MediaApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
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

Get presigned upload URL

Get a presigned URL to upload files directly to cloud storage. Supports files up to 5GB.  How it works: call this endpoint with the filename and content type, receive an uploadUrl (presigned) and publicUrl, PUT your file directly to the uploadUrl, then use the publicUrl in your posts. 

### Example

```java
// Import classes:
import dev.getlate.ApiClient;
import dev.getlate.ApiException;
import dev.getlate.ApiResponse;
import dev.getlate.Configuration;
import dev.getlate.auth.*;
import dev.getlate.models.*;
import dev.getlate.api.MediaApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("https://getlate.dev/api");
        
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

