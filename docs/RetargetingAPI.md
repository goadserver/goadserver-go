# \RetargetingAPI

All URIs are relative to *https://up.go-adserver.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiV1RetargetingPixelsGet**](RetargetingAPI.md#ApiV1RetargetingPixelsGet) | **Get** /api/v1/retargeting/pixels | List the caller&#39;s retargeting pixels.
[**ApiV1RetargetingPixelsIdActivePatch**](RetargetingAPI.md#ApiV1RetargetingPixelsIdActivePatch) | **Patch** /api/v1/retargeting/pixels/{id}/active | Activate or deactivate a retargeting pixel.
[**ApiV1RetargetingPixelsIdDelete**](RetargetingAPI.md#ApiV1RetargetingPixelsIdDelete) | **Delete** /api/v1/retargeting/pixels/{id} | Soft-delete a retargeting pixel and clear its captured visitors.
[**ApiV1RetargetingPixelsIdGet**](RetargetingAPI.md#ApiV1RetargetingPixelsIdGet) | **Get** /api/v1/retargeting/pixels/{id} | Get one retargeting pixel.
[**ApiV1RetargetingPixelsIdPut**](RetargetingAPI.md#ApiV1RetargetingPixelsIdPut) | **Put** /api/v1/retargeting/pixels/{id} | Rename a retargeting pixel.
[**ApiV1RetargetingPixelsPost**](RetargetingAPI.md#ApiV1RetargetingPixelsPost) | **Post** /api/v1/retargeting/pixels | Create a retargeting pixel.



## ApiV1RetargetingPixelsGet

> ApiV1RetargetingPixelsGet200Response ApiV1RetargetingPixelsGet(ctx).Execute()

List the caller's retargeting pixels.

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/goadserver/goadserver-go"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RetargetingAPI.ApiV1RetargetingPixelsGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RetargetingAPI.ApiV1RetargetingPixelsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1RetargetingPixelsGet`: ApiV1RetargetingPixelsGet200Response
	fmt.Fprintf(os.Stdout, "Response from `RetargetingAPI.ApiV1RetargetingPixelsGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1RetargetingPixelsGetRequest struct via the builder pattern


### Return type

[**ApiV1RetargetingPixelsGet200Response**](ApiV1RetargetingPixelsGet200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1RetargetingPixelsIdActivePatch

> ApiV1RetargetingPixelsIdActivePatch200Response ApiV1RetargetingPixelsIdActivePatch(ctx, id).ApiV1CampaignsTypeIdActivePatchRequest(apiV1CampaignsTypeIdActivePatchRequest).Execute()

Activate or deactivate a retargeting pixel.

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/goadserver/goadserver-go"
)

func main() {
	id := int32(56) // int32 | 
	apiV1CampaignsTypeIdActivePatchRequest := *openapiclient.NewApiV1CampaignsTypeIdActivePatchRequest(false) // ApiV1CampaignsTypeIdActivePatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RetargetingAPI.ApiV1RetargetingPixelsIdActivePatch(context.Background(), id).ApiV1CampaignsTypeIdActivePatchRequest(apiV1CampaignsTypeIdActivePatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RetargetingAPI.ApiV1RetargetingPixelsIdActivePatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1RetargetingPixelsIdActivePatch`: ApiV1RetargetingPixelsIdActivePatch200Response
	fmt.Fprintf(os.Stdout, "Response from `RetargetingAPI.ApiV1RetargetingPixelsIdActivePatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1RetargetingPixelsIdActivePatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **apiV1CampaignsTypeIdActivePatchRequest** | [**ApiV1CampaignsTypeIdActivePatchRequest**](ApiV1CampaignsTypeIdActivePatchRequest.md) |  | 

### Return type

[**ApiV1RetargetingPixelsIdActivePatch200Response**](ApiV1RetargetingPixelsIdActivePatch200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1RetargetingPixelsIdDelete

> ApiV1RetargetingPixelsIdDelete(ctx, id).Execute()

Soft-delete a retargeting pixel and clear its captured visitors.



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/goadserver/goadserver-go"
)

func main() {
	id := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.RetargetingAPI.ApiV1RetargetingPixelsIdDelete(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RetargetingAPI.ApiV1RetargetingPixelsIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1RetargetingPixelsIdDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1RetargetingPixelsIdGet

> RetargetingPixel ApiV1RetargetingPixelsIdGet(ctx, id).Execute()

Get one retargeting pixel.

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/goadserver/goadserver-go"
)

func main() {
	id := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RetargetingAPI.ApiV1RetargetingPixelsIdGet(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RetargetingAPI.ApiV1RetargetingPixelsIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1RetargetingPixelsIdGet`: RetargetingPixel
	fmt.Fprintf(os.Stdout, "Response from `RetargetingAPI.ApiV1RetargetingPixelsIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1RetargetingPixelsIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**RetargetingPixel**](RetargetingPixel.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1RetargetingPixelsIdPut

> ApiV1RetargetingPixelsIdPut(ctx, id).ApiV1RetargetingPixelsIdPutRequest(apiV1RetargetingPixelsIdPutRequest).Execute()

Rename a retargeting pixel.

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/goadserver/goadserver-go"
)

func main() {
	id := int32(56) // int32 | 
	apiV1RetargetingPixelsIdPutRequest := *openapiclient.NewApiV1RetargetingPixelsIdPutRequest() // ApiV1RetargetingPixelsIdPutRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.RetargetingAPI.ApiV1RetargetingPixelsIdPut(context.Background(), id).ApiV1RetargetingPixelsIdPutRequest(apiV1RetargetingPixelsIdPutRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RetargetingAPI.ApiV1RetargetingPixelsIdPut``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1RetargetingPixelsIdPutRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **apiV1RetargetingPixelsIdPutRequest** | [**ApiV1RetargetingPixelsIdPutRequest**](ApiV1RetargetingPixelsIdPutRequest.md) |  | 

### Return type

 (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1RetargetingPixelsPost

> RetargetingPixel ApiV1RetargetingPixelsPost(ctx).ApiV1RetargetingPixelsPostRequest(apiV1RetargetingPixelsPostRequest).Execute()

Create a retargeting pixel.

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/goadserver/goadserver-go"
)

func main() {
	apiV1RetargetingPixelsPostRequest := *openapiclient.NewApiV1RetargetingPixelsPostRequest("Cart abandoners") // ApiV1RetargetingPixelsPostRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RetargetingAPI.ApiV1RetargetingPixelsPost(context.Background()).ApiV1RetargetingPixelsPostRequest(apiV1RetargetingPixelsPostRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RetargetingAPI.ApiV1RetargetingPixelsPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1RetargetingPixelsPost`: RetargetingPixel
	fmt.Fprintf(os.Stdout, "Response from `RetargetingAPI.ApiV1RetargetingPixelsPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiV1RetargetingPixelsPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiV1RetargetingPixelsPostRequest** | [**ApiV1RetargetingPixelsPostRequest**](ApiV1RetargetingPixelsPostRequest.md) |  | 

### Return type

[**RetargetingPixel**](RetargetingPixel.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

