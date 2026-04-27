# \CreativePoolsAPI

All URIs are relative to *https://up.goadserver.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiV1CreativePoolsGet**](CreativePoolsAPI.md#ApiV1CreativePoolsGet) | **Get** /api/v1/creative-pools | List creative pools.
[**ApiV1CreativePoolsIdClonePost**](CreativePoolsAPI.md#ApiV1CreativePoolsIdClonePost) | **Post** /api/v1/creative-pools/{id}/clone | Clone a creative pool with all its items.
[**ApiV1CreativePoolsIdDelete**](CreativePoolsAPI.md#ApiV1CreativePoolsIdDelete) | **Delete** /api/v1/creative-pools/{id} | Soft-delete a creative pool.
[**ApiV1CreativePoolsIdGet**](CreativePoolsAPI.md#ApiV1CreativePoolsIdGet) | **Get** /api/v1/creative-pools/{id} | Show a single creative pool.
[**ApiV1CreativePoolsIdItemsGet**](CreativePoolsAPI.md#ApiV1CreativePoolsIdItemsGet) | **Get** /api/v1/creative-pools/{id}/items | List items in a creative pool.
[**ApiV1CreativePoolsIdItemsItemIdDelete**](CreativePoolsAPI.md#ApiV1CreativePoolsIdItemsItemIdDelete) | **Delete** /api/v1/creative-pools/{id}/items/{itemId} | Soft-delete a single pool item.
[**ApiV1CreativePoolsIdItemsItemIdPut**](CreativePoolsAPI.md#ApiV1CreativePoolsIdItemsItemIdPut) | **Put** /api/v1/creative-pools/{id}/items/{itemId} | Update a single pool item.
[**ApiV1CreativePoolsIdItemsItemIdTogglePut**](CreativePoolsAPI.md#ApiV1CreativePoolsIdItemsItemIdTogglePut) | **Put** /api/v1/creative-pools/{id}/items/{itemId}/toggle | Toggle a pool item on / off.
[**ApiV1CreativePoolsIdPut**](CreativePoolsAPI.md#ApiV1CreativePoolsIdPut) | **Put** /api/v1/creative-pools/{id} | Update creative pool meta.
[**ApiV1CreativePoolsIdUsedInGet**](CreativePoolsAPI.md#ApiV1CreativePoolsIdUsedInGet) | **Get** /api/v1/creative-pools/{id}/used-in | List campaigns / ads that reference this pool.
[**ApiV1CreativePoolsPost**](CreativePoolsAPI.md#ApiV1CreativePoolsPost) | **Post** /api/v1/creative-pools | Create a creative pool.



## ApiV1CreativePoolsGet

> ApiV1CreativePoolsGet200Response ApiV1CreativePoolsGet(ctx).Type_(type_).Title(title).Page(page).PerPage(perPage).Sort(sort).Execute()

List creative pools.



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
	type_ := "type__example" // string |  (optional)
	title := "title_example" // string |  (optional)
	page := int32(56) // int32 |  (optional) (default to 1)
	perPage := int32(56) // int32 |  (optional) (default to 50)
	sort := "sort_example" // string |  (optional) (default to "id")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CreativePoolsAPI.ApiV1CreativePoolsGet(context.Background()).Type_(type_).Title(title).Page(page).PerPage(perPage).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CreativePoolsAPI.ApiV1CreativePoolsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CreativePoolsGet`: ApiV1CreativePoolsGet200Response
	fmt.Fprintf(os.Stdout, "Response from `CreativePoolsAPI.ApiV1CreativePoolsGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CreativePoolsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **type_** | **string** |  | 
 **title** | **string** |  | 
 **page** | **int32** |  | [default to 1]
 **perPage** | **int32** |  | [default to 50]
 **sort** | **string** |  | [default to &quot;id&quot;]

### Return type

[**ApiV1CreativePoolsGet200Response**](ApiV1CreativePoolsGet200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1CreativePoolsIdClonePost

> ApiV1CreativePoolsIdClonePost201Response ApiV1CreativePoolsIdClonePost(ctx, id).Execute()

Clone a creative pool with all its items.



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
	resp, r, err := apiClient.CreativePoolsAPI.ApiV1CreativePoolsIdClonePost(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CreativePoolsAPI.ApiV1CreativePoolsIdClonePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CreativePoolsIdClonePost`: ApiV1CreativePoolsIdClonePost201Response
	fmt.Fprintf(os.Stdout, "Response from `CreativePoolsAPI.ApiV1CreativePoolsIdClonePost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CreativePoolsIdClonePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ApiV1CreativePoolsIdClonePost201Response**](ApiV1CreativePoolsIdClonePost201Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1CreativePoolsIdDelete

> ApiV1CreativePoolsIdDelete200Response ApiV1CreativePoolsIdDelete(ctx, id).Execute()

Soft-delete a creative pool.



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
	resp, r, err := apiClient.CreativePoolsAPI.ApiV1CreativePoolsIdDelete(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CreativePoolsAPI.ApiV1CreativePoolsIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CreativePoolsIdDelete`: ApiV1CreativePoolsIdDelete200Response
	fmt.Fprintf(os.Stdout, "Response from `CreativePoolsAPI.ApiV1CreativePoolsIdDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CreativePoolsIdDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ApiV1CreativePoolsIdDelete200Response**](ApiV1CreativePoolsIdDelete200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1CreativePoolsIdGet

> ApiV1CreativePoolsIdGet200Response ApiV1CreativePoolsIdGet(ctx, id).Execute()

Show a single creative pool.

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
	resp, r, err := apiClient.CreativePoolsAPI.ApiV1CreativePoolsIdGet(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CreativePoolsAPI.ApiV1CreativePoolsIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CreativePoolsIdGet`: ApiV1CreativePoolsIdGet200Response
	fmt.Fprintf(os.Stdout, "Response from `CreativePoolsAPI.ApiV1CreativePoolsIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CreativePoolsIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ApiV1CreativePoolsIdGet200Response**](ApiV1CreativePoolsIdGet200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1CreativePoolsIdItemsGet

> ApiV1CampaignsTypeCampaignIdAdsGet200Response ApiV1CreativePoolsIdItemsGet(ctx, id).Page(page).PerPage(perPage).Execute()

List items in a creative pool.



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
	page := int32(56) // int32 |  (optional) (default to 1)
	perPage := int32(56) // int32 |  (optional) (default to 50)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CreativePoolsAPI.ApiV1CreativePoolsIdItemsGet(context.Background(), id).Page(page).PerPage(perPage).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CreativePoolsAPI.ApiV1CreativePoolsIdItemsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CreativePoolsIdItemsGet`: ApiV1CampaignsTypeCampaignIdAdsGet200Response
	fmt.Fprintf(os.Stdout, "Response from `CreativePoolsAPI.ApiV1CreativePoolsIdItemsGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CreativePoolsIdItemsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** |  | [default to 1]
 **perPage** | **int32** |  | [default to 50]

### Return type

[**ApiV1CampaignsTypeCampaignIdAdsGet200Response**](ApiV1CampaignsTypeCampaignIdAdsGet200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1CreativePoolsIdItemsItemIdDelete

> ApiV1CreativePoolsIdItemsItemIdDelete(ctx, id, itemId).Execute()

Soft-delete a single pool item.



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
	itemId := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.CreativePoolsAPI.ApiV1CreativePoolsIdItemsItemIdDelete(context.Background(), id, itemId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CreativePoolsAPI.ApiV1CreativePoolsIdItemsItemIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 
**itemId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CreativePoolsIdItemsItemIdDeleteRequest struct via the builder pattern


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


## ApiV1CreativePoolsIdItemsItemIdPut

> ApiV1CreativePoolsIdItemsItemIdPut(ctx, id, itemId).ApiV1CreativePoolsIdItemsItemIdPutRequest(apiV1CreativePoolsIdItemsItemIdPutRequest).Execute()

Update a single pool item.



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
	itemId := int32(56) // int32 | 
	apiV1CreativePoolsIdItemsItemIdPutRequest := *openapiclient.NewApiV1CreativePoolsIdItemsItemIdPutRequest() // ApiV1CreativePoolsIdItemsItemIdPutRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.CreativePoolsAPI.ApiV1CreativePoolsIdItemsItemIdPut(context.Background(), id, itemId).ApiV1CreativePoolsIdItemsItemIdPutRequest(apiV1CreativePoolsIdItemsItemIdPutRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CreativePoolsAPI.ApiV1CreativePoolsIdItemsItemIdPut``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 
**itemId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CreativePoolsIdItemsItemIdPutRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **apiV1CreativePoolsIdItemsItemIdPutRequest** | [**ApiV1CreativePoolsIdItemsItemIdPutRequest**](ApiV1CreativePoolsIdItemsItemIdPutRequest.md) |  | 

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


## ApiV1CreativePoolsIdItemsItemIdTogglePut

> ApiV1CreativePoolsIdItemsItemIdTogglePut(ctx, id, itemId).Execute()

Toggle a pool item on / off.



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
	itemId := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.CreativePoolsAPI.ApiV1CreativePoolsIdItemsItemIdTogglePut(context.Background(), id, itemId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CreativePoolsAPI.ApiV1CreativePoolsIdItemsItemIdTogglePut``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 
**itemId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CreativePoolsIdItemsItemIdTogglePutRequest struct via the builder pattern


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


## ApiV1CreativePoolsIdPut

> ApiV1CreativePoolsIdPut(ctx, id).ApiV1CreativePoolsIdPutRequest(apiV1CreativePoolsIdPutRequest).Execute()

Update creative pool meta.



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
	apiV1CreativePoolsIdPutRequest := *openapiclient.NewApiV1CreativePoolsIdPutRequest() // ApiV1CreativePoolsIdPutRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.CreativePoolsAPI.ApiV1CreativePoolsIdPut(context.Background(), id).ApiV1CreativePoolsIdPutRequest(apiV1CreativePoolsIdPutRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CreativePoolsAPI.ApiV1CreativePoolsIdPut``: %v\n", err)
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

Other parameters are passed through a pointer to a apiApiV1CreativePoolsIdPutRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **apiV1CreativePoolsIdPutRequest** | [**ApiV1CreativePoolsIdPutRequest**](ApiV1CreativePoolsIdPutRequest.md) |  | 

### Return type

 (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1CreativePoolsIdUsedInGet

> ApiV1CreativePoolsIdUsedInGet200Response ApiV1CreativePoolsIdUsedInGet(ctx, id).Execute()

List campaigns / ads that reference this pool.

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
	resp, r, err := apiClient.CreativePoolsAPI.ApiV1CreativePoolsIdUsedInGet(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CreativePoolsAPI.ApiV1CreativePoolsIdUsedInGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CreativePoolsIdUsedInGet`: ApiV1CreativePoolsIdUsedInGet200Response
	fmt.Fprintf(os.Stdout, "Response from `CreativePoolsAPI.ApiV1CreativePoolsIdUsedInGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CreativePoolsIdUsedInGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ApiV1CreativePoolsIdUsedInGet200Response**](ApiV1CreativePoolsIdUsedInGet200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1CreativePoolsPost

> ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost200Response ApiV1CreativePoolsPost(ctx).ApiV1CreativePoolsPostRequest(apiV1CreativePoolsPostRequest).Execute()

Create a creative pool.



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
	apiV1CreativePoolsPostRequest := *openapiclient.NewApiV1CreativePoolsPostRequest("300x250 Promo Q3") // ApiV1CreativePoolsPostRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CreativePoolsAPI.ApiV1CreativePoolsPost(context.Background()).ApiV1CreativePoolsPostRequest(apiV1CreativePoolsPostRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CreativePoolsAPI.ApiV1CreativePoolsPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CreativePoolsPost`: ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost200Response
	fmt.Fprintf(os.Stdout, "Response from `CreativePoolsAPI.ApiV1CreativePoolsPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CreativePoolsPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiV1CreativePoolsPostRequest** | [**ApiV1CreativePoolsPostRequest**](ApiV1CreativePoolsPostRequest.md) |  | 

### Return type

[**ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost200Response**](ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

