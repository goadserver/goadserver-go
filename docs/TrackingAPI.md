# \TrackingAPI

All URIs are relative to *https://up.goadserver.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiV1TrackingConversionTypesGet**](TrackingAPI.md#ApiV1TrackingConversionTypesGet) | **Get** /api/v1/tracking/conversion-types | Available conversion types for the caller&#39;s account.
[**ApiV1TrackingPixelsGet**](TrackingAPI.md#ApiV1TrackingPixelsGet) | **Get** /api/v1/tracking/pixels | List the caller&#39;s conversion-tracking pixels.
[**ApiV1TrackingPixelsIdDelete**](TrackingAPI.md#ApiV1TrackingPixelsIdDelete) | **Delete** /api/v1/tracking/pixels/{id} | Delete a pixel.
[**ApiV1TrackingPixelsIdGet**](TrackingAPI.md#ApiV1TrackingPixelsIdGet) | **Get** /api/v1/tracking/pixels/{id} | Get one pixel.
[**ApiV1TrackingPixelsIdPut**](TrackingAPI.md#ApiV1TrackingPixelsIdPut) | **Put** /api/v1/tracking/pixels/{id} | Update a pixel&#39;s name or conversion type.
[**ApiV1TrackingPixelsPost**](TrackingAPI.md#ApiV1TrackingPixelsPost) | **Post** /api/v1/tracking/pixels | Create a new tracking pixel.



## ApiV1TrackingConversionTypesGet

> ApiV1TrackingConversionTypesGet200Response ApiV1TrackingConversionTypesGet(ctx).Execute()

Available conversion types for the caller's account.



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
	resp, r, err := apiClient.TrackingAPI.ApiV1TrackingConversionTypesGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TrackingAPI.ApiV1TrackingConversionTypesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1TrackingConversionTypesGet`: ApiV1TrackingConversionTypesGet200Response
	fmt.Fprintf(os.Stdout, "Response from `TrackingAPI.ApiV1TrackingConversionTypesGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1TrackingConversionTypesGetRequest struct via the builder pattern


### Return type

[**ApiV1TrackingConversionTypesGet200Response**](ApiV1TrackingConversionTypesGet200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1TrackingPixelsGet

> ApiV1TrackingPixelsGet200Response ApiV1TrackingPixelsGet(ctx).ConversionTypeId(conversionTypeId).Name(name).Page(page).PerPage(perPage).Execute()

List the caller's conversion-tracking pixels.

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
	conversionTypeId := int32(56) // int32 | Filter by conversion type. (optional)
	name := "name_example" // string | Substring search on name. (optional)
	page := int32(56) // int32 |  (optional) (default to 1)
	perPage := int32(56) // int32 |  (optional) (default to 100)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TrackingAPI.ApiV1TrackingPixelsGet(context.Background()).ConversionTypeId(conversionTypeId).Name(name).Page(page).PerPage(perPage).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TrackingAPI.ApiV1TrackingPixelsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1TrackingPixelsGet`: ApiV1TrackingPixelsGet200Response
	fmt.Fprintf(os.Stdout, "Response from `TrackingAPI.ApiV1TrackingPixelsGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiV1TrackingPixelsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conversionTypeId** | **int32** | Filter by conversion type. | 
 **name** | **string** | Substring search on name. | 
 **page** | **int32** |  | [default to 1]
 **perPage** | **int32** |  | [default to 100]

### Return type

[**ApiV1TrackingPixelsGet200Response**](ApiV1TrackingPixelsGet200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1TrackingPixelsIdDelete

> ApiV1TrackingPixelsIdDelete(ctx, id).Execute()

Delete a pixel.

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
	r, err := apiClient.TrackingAPI.ApiV1TrackingPixelsIdDelete(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TrackingAPI.ApiV1TrackingPixelsIdDelete``: %v\n", err)
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

Other parameters are passed through a pointer to a apiApiV1TrackingPixelsIdDeleteRequest struct via the builder pattern


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


## ApiV1TrackingPixelsIdGet

> TrackingPixel ApiV1TrackingPixelsIdGet(ctx, id).Execute()

Get one pixel.

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
	resp, r, err := apiClient.TrackingAPI.ApiV1TrackingPixelsIdGet(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TrackingAPI.ApiV1TrackingPixelsIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1TrackingPixelsIdGet`: TrackingPixel
	fmt.Fprintf(os.Stdout, "Response from `TrackingAPI.ApiV1TrackingPixelsIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1TrackingPixelsIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**TrackingPixel**](TrackingPixel.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1TrackingPixelsIdPut

> TrackingPixel ApiV1TrackingPixelsIdPut(ctx, id).ApiV1TrackingPixelsIdPutRequest(apiV1TrackingPixelsIdPutRequest).Execute()

Update a pixel's name or conversion type.

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
	apiV1TrackingPixelsIdPutRequest := *openapiclient.NewApiV1TrackingPixelsIdPutRequest() // ApiV1TrackingPixelsIdPutRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TrackingAPI.ApiV1TrackingPixelsIdPut(context.Background(), id).ApiV1TrackingPixelsIdPutRequest(apiV1TrackingPixelsIdPutRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TrackingAPI.ApiV1TrackingPixelsIdPut``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1TrackingPixelsIdPut`: TrackingPixel
	fmt.Fprintf(os.Stdout, "Response from `TrackingAPI.ApiV1TrackingPixelsIdPut`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1TrackingPixelsIdPutRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **apiV1TrackingPixelsIdPutRequest** | [**ApiV1TrackingPixelsIdPutRequest**](ApiV1TrackingPixelsIdPutRequest.md) |  | 

### Return type

[**TrackingPixel**](TrackingPixel.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1TrackingPixelsPost

> TrackingPixel ApiV1TrackingPixelsPost(ctx).ApiV1TrackingPixelsPostRequest(apiV1TrackingPixelsPostRequest).Execute()

Create a new tracking pixel.



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
	apiV1TrackingPixelsPostRequest := *openapiclient.NewApiV1TrackingPixelsPostRequest("Signup confirmation", int32(1)) // ApiV1TrackingPixelsPostRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TrackingAPI.ApiV1TrackingPixelsPost(context.Background()).ApiV1TrackingPixelsPostRequest(apiV1TrackingPixelsPostRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TrackingAPI.ApiV1TrackingPixelsPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1TrackingPixelsPost`: TrackingPixel
	fmt.Fprintf(os.Stdout, "Response from `TrackingAPI.ApiV1TrackingPixelsPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiV1TrackingPixelsPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiV1TrackingPixelsPostRequest** | [**ApiV1TrackingPixelsPostRequest**](ApiV1TrackingPixelsPostRequest.md) |  | 

### Return type

[**TrackingPixel**](TrackingPixel.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

