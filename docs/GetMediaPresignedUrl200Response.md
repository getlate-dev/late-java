

# GetMediaPresignedUrl200Response


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**uploadUrl** | **URI** | Presigned URL to PUT your file to (expires in 1 hour) |  [optional] |
|**publicUrl** | **URI** | Public URL where the file will be accessible after upload |  [optional] |
|**key** | **String** | Storage key/path of the file |  [optional] |
|**type** | [**TypeEnum**](#TypeEnum) | Detected file type based on content type |  [optional] |



## Enum: TypeEnum

| Name | Value |
|---- | -----|
| IMAGE | &quot;image&quot; |
| VIDEO | &quot;video&quot; |
| DOCUMENT | &quot;document&quot; |



