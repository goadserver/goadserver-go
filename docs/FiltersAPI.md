# \FiltersAPI

All URIs are relative to *https://up.go-adserver.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiV1FiltersGet**](FiltersAPI.md#ApiV1FiltersGet) | **Get** /api/v1/filters | List all filters across types.
[**ApiV1FiltersPost**](FiltersAPI.md#ApiV1FiltersPost) | **Post** /api/v1/filters | Create a filter and populate it with items.
[**ApiV1FiltersTypeIdActivePatch**](FiltersAPI.md#ApiV1FiltersTypeIdActivePatch) | **Patch** /api/v1/filters/{type}/{id}/active | Activate or deactivate a filter (exclusion types only).
[**ApiV1FiltersTypeIdDelete**](FiltersAPI.md#ApiV1FiltersTypeIdDelete) | **Delete** /api/v1/filters/{type}/{id} | Delete a filter (and its items, for IP pools).
[**ApiV1FiltersTypeIdGet**](FiltersAPI.md#ApiV1FiltersTypeIdGet) | **Get** /api/v1/filters/{type}/{id} | Get a single filter with its items.
[**ApiV1FiltersTypeIdItemsItemDelete**](FiltersAPI.md#ApiV1FiltersTypeIdItemsItemDelete) | **Delete** /api/v1/filters/{type}/{id}/items/{item} | Remove a single item from a filter.
[**ApiV1FiltersTypeIdItemsPost**](FiltersAPI.md#ApiV1FiltersTypeIdItemsPost) | **Post** /api/v1/filters/{type}/{id}/items | Add items to an existing filter.



## ApiV1FiltersGet

> ApiV1FiltersGet200Response ApiV1FiltersGet(ctx).Type_(type_).Execute()

List all filters across types.



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
	type_ := "type__example" // string | Filter to one type. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FiltersAPI.ApiV1FiltersGet(context.Background()).Type_(type_).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FiltersAPI.ApiV1FiltersGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1FiltersGet`: ApiV1FiltersGet200Response
	fmt.Fprintf(os.Stdout, "Response from `FiltersAPI.ApiV1FiltersGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiV1FiltersGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **type_** | **string** | Filter to one type. | 

### Return type

[**ApiV1FiltersGet200Response**](ApiV1FiltersGet200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1FiltersPost

> FilterDetail ApiV1FiltersPost(ctx).ApiV1FiltersPostRequest(apiV1FiltersPostRequest).Execute()

Create a filter and populate it with items.



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
	apiV1FiltersPostRequest := *openapiclient.NewApiV1FiltersPostRequest("Type_example", "Name_example", []string{"Items_example"}) // ApiV1FiltersPostRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FiltersAPI.ApiV1FiltersPost(context.Background()).ApiV1FiltersPostRequest(apiV1FiltersPostRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FiltersAPI.ApiV1FiltersPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1FiltersPost`: FilterDetail
	fmt.Fprintf(os.Stdout, "Response from `FiltersAPI.ApiV1FiltersPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiV1FiltersPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiV1FiltersPostRequest** | [**ApiV1FiltersPostRequest**](ApiV1FiltersPostRequest.md) |  | 

### Return type

[**FilterDetail**](FilterDetail.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1FiltersTypeIdActivePatch

> ApiV1FiltersTypeIdActivePatch200Response ApiV1FiltersTypeIdActivePatch(ctx, type_, id).ApiV1CampaignsTypeIdActivePatchRequest(apiV1CampaignsTypeIdActivePatchRequest).Execute()

Activate or deactivate a filter (exclusion types only).



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
	type_ := "type__example" // string | 
	id := int32(56) // int32 | 
	apiV1CampaignsTypeIdActivePatchRequest := *openapiclient.NewApiV1CampaignsTypeIdActivePatchRequest(false) // ApiV1CampaignsTypeIdActivePatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FiltersAPI.ApiV1FiltersTypeIdActivePatch(context.Background(), type_, id).ApiV1CampaignsTypeIdActivePatchRequest(apiV1CampaignsTypeIdActivePatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FiltersAPI.ApiV1FiltersTypeIdActivePatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1FiltersTypeIdActivePatch`: ApiV1FiltersTypeIdActivePatch200Response
	fmt.Fprintf(os.Stdout, "Response from `FiltersAPI.ApiV1FiltersTypeIdActivePatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1FiltersTypeIdActivePatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **apiV1CampaignsTypeIdActivePatchRequest** | [**ApiV1CampaignsTypeIdActivePatchRequest**](ApiV1CampaignsTypeIdActivePatchRequest.md) |  | 

### Return type

[**ApiV1FiltersTypeIdActivePatch200Response**](ApiV1FiltersTypeIdActivePatch200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1FiltersTypeIdDelete

> ApiV1FiltersTypeIdDelete(ctx, type_, id).Execute()

Delete a filter (and its items, for IP pools).

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
	type_ := "type__example" // string | 
	id := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.FiltersAPI.ApiV1FiltersTypeIdDelete(context.Background(), type_, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FiltersAPI.ApiV1FiltersTypeIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1FiltersTypeIdDeleteRequest struct via the builder pattern


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


## ApiV1FiltersTypeIdGet

> FilterDetail ApiV1FiltersTypeIdGet(ctx, type_, id).Execute()

Get a single filter with its items.

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
	type_ := "type__example" // string | 
	id := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FiltersAPI.ApiV1FiltersTypeIdGet(context.Background(), type_, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FiltersAPI.ApiV1FiltersTypeIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1FiltersTypeIdGet`: FilterDetail
	fmt.Fprintf(os.Stdout, "Response from `FiltersAPI.ApiV1FiltersTypeIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1FiltersTypeIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**FilterDetail**](FilterDetail.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1FiltersTypeIdItemsItemDelete

> ApiV1FiltersTypeIdItemsItemDelete200Response ApiV1FiltersTypeIdItemsItemDelete(ctx, type_, id, item).Execute()

Remove a single item from a filter.



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
	type_ := "type__example" // string | 
	id := int32(56) // int32 | 
	item := "item_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FiltersAPI.ApiV1FiltersTypeIdItemsItemDelete(context.Background(), type_, id, item).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FiltersAPI.ApiV1FiltersTypeIdItemsItemDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1FiltersTypeIdItemsItemDelete`: ApiV1FiltersTypeIdItemsItemDelete200Response
	fmt.Fprintf(os.Stdout, "Response from `FiltersAPI.ApiV1FiltersTypeIdItemsItemDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**id** | **int32** |  | 
**item** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1FiltersTypeIdItemsItemDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

[**ApiV1FiltersTypeIdItemsItemDelete200Response**](ApiV1FiltersTypeIdItemsItemDelete200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1FiltersTypeIdItemsPost

> ApiV1FiltersTypeIdItemsPost200Response ApiV1FiltersTypeIdItemsPost(ctx, type_, id).ApiV1FiltersTypeIdItemsPostRequest(apiV1FiltersTypeIdItemsPostRequest).Execute()

Add items to an existing filter.



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
	type_ := "type__example" // string | 
	id := int32(56) // int32 | 
	apiV1FiltersTypeIdItemsPostRequest := *openapiclient.NewApiV1FiltersTypeIdItemsPostRequest([]string{"Items_example"}) // ApiV1FiltersTypeIdItemsPostRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FiltersAPI.ApiV1FiltersTypeIdItemsPost(context.Background(), type_, id).ApiV1FiltersTypeIdItemsPostRequest(apiV1FiltersTypeIdItemsPostRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FiltersAPI.ApiV1FiltersTypeIdItemsPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1FiltersTypeIdItemsPost`: ApiV1FiltersTypeIdItemsPost200Response
	fmt.Fprintf(os.Stdout, "Response from `FiltersAPI.ApiV1FiltersTypeIdItemsPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1FiltersTypeIdItemsPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **apiV1FiltersTypeIdItemsPostRequest** | [**ApiV1FiltersTypeIdItemsPostRequest**](ApiV1FiltersTypeIdItemsPostRequest.md) |  | 

### Return type

[**ApiV1FiltersTypeIdItemsPost200Response**](ApiV1FiltersTypeIdItemsPost200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

