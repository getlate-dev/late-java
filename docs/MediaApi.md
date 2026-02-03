# MediaApi

All URIs are relative to *https://getlate.dev/api*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getMediaPresignedUrl**](MediaApi.md#getMediaPresignedUrl) | **POST** /v1/media/presign | Get a presigned URL for direct file upload (up to 5GB) |
| [**getMediaPresignedUrlWithHttpInfo**](MediaApi.md#getMediaPresignedUrlWithHttpInfo) | **POST** /v1/media/presign | Get a presigned URL for direct file upload (up to 5GB) |



## getMediaPresignedUrl

> GetMediaPresignedUrl200Response getMediaPresignedUrl(getMediaPresignedUrlRequest)

Get a presigned URL for direct file upload (up to 5GB)

Get a presigned URL to upload files directly to cloud storage. This is the recommended method for uploading files of any size, especially files larger than ~4MB.  **How it works:** 1. Call this endpoint with the filename and content type 2. Receive an &#x60;uploadUrl&#x60; (presigned) and &#x60;publicUrl&#x60; 3. PUT your file directly to the &#x60;uploadUrl&#x60; 4. Use the &#x60;publicUrl&#x60; in your posts  **Benefits:** - Supports files up to 5GB - Files upload directly to storage (faster, no server bottleneck) - No 413 errors from server body size limits  **Example:** &#x60;&#x60;&#x60;javascript // Step 1: Get presigned URL const response &#x3D; await fetch(&#39;https://getlate.dev/api/v1/media/presign&#39;, {   method: &#39;POST&#39;,   headers: {     &#39;Authorization&#39;: &#39;Bearer YOUR_API_KEY&#39;,     &#39;Content-Type&#39;: &#39;application/json&#39;   },   body: JSON.stringify({     filename: &#39;my-video.mp4&#39;,     contentType: &#39;video/mp4&#39;   }) }); const { uploadUrl, publicUrl } &#x3D; await response.json();  // Step 2: Upload file directly to storage await fetch(uploadUrl, {   method: &#39;PUT&#39;,   body: file,   headers: { &#39;Content-Type&#39;: &#39;video/mp4&#39; } });  // Step 3: Use publicUrl when creating your post // The publicUrl is ready to use immediately after upload completes &#x60;&#x60;&#x60; 

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

Get a presigned URL for direct file upload (up to 5GB)

Get a presigned URL to upload files directly to cloud storage. This is the recommended method for uploading files of any size, especially files larger than ~4MB.  **How it works:** 1. Call this endpoint with the filename and content type 2. Receive an &#x60;uploadUrl&#x60; (presigned) and &#x60;publicUrl&#x60; 3. PUT your file directly to the &#x60;uploadUrl&#x60; 4. Use the &#x60;publicUrl&#x60; in your posts  **Benefits:** - Supports files up to 5GB - Files upload directly to storage (faster, no server bottleneck) - No 413 errors from server body size limits  **Example:** &#x60;&#x60;&#x60;javascript // Step 1: Get presigned URL const response &#x3D; await fetch(&#39;https://getlate.dev/api/v1/media/presign&#39;, {   method: &#39;POST&#39;,   headers: {     &#39;Authorization&#39;: &#39;Bearer YOUR_API_KEY&#39;,     &#39;Content-Type&#39;: &#39;application/json&#39;   },   body: JSON.stringify({     filename: &#39;my-video.mp4&#39;,     contentType: &#39;video/mp4&#39;   }) }); const { uploadUrl, publicUrl } &#x3D; await response.json();  // Step 2: Upload file directly to storage await fetch(uploadUrl, {   method: &#39;PUT&#39;,   body: file,   headers: { &#39;Content-Type&#39;: &#39;video/mp4&#39; } });  // Step 3: Use publicUrl when creating your post // The publicUrl is ready to use immediately after upload completes &#x60;&#x60;&#x60; 

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

