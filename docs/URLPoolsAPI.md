# \URLPoolsAPI

All URIs are relative to *https://up.go-adserver.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiV1UrlPoolsGet**](URLPoolsAPI.md#ApiV1UrlPoolsGet) | **Get** /api/v1/url-pools | List URL pools.
[**ApiV1UrlPoolsIdClonePost**](URLPoolsAPI.md#ApiV1UrlPoolsIdClonePost) | **Post** /api/v1/url-pools/{id}/clone | Clone a URL pool with all its URLs.
[**ApiV1UrlPoolsIdDelete**](URLPoolsAPI.md#ApiV1UrlPoolsIdDelete) | **Delete** /api/v1/url-pools/{id} | Soft-delete a URL pool.
[**ApiV1UrlPoolsIdGet**](URLPoolsAPI.md#ApiV1UrlPoolsIdGet) | **Get** /api/v1/url-pools/{id} | Show one URL pool.
[**ApiV1UrlPoolsIdPut**](URLPoolsAPI.md#ApiV1UrlPoolsIdPut) | **Put** /api/v1/url-pools/{id} | Update URL pool meta.
[**ApiV1UrlPoolsIdUrlsGet**](URLPoolsAPI.md#ApiV1UrlPoolsIdUrlsGet) | **Get** /api/v1/url-pools/{id}/urls | List URLs in a pool.
[**ApiV1UrlPoolsIdUrlsPost**](URLPoolsAPI.md#ApiV1UrlPoolsIdUrlsPost) | **Post** /api/v1/url-pools/{id}/urls | Add a URL to a pool.
[**ApiV1UrlPoolsIdUrlsUrlIdClonePost**](URLPoolsAPI.md#ApiV1UrlPoolsIdUrlsUrlIdClonePost) | **Post** /api/v1/url-pools/{id}/urls/{urlId}/clone | Clone a single URL within the same pool.
[**ApiV1UrlPoolsIdUrlsUrlIdDelete**](URLPoolsAPI.md#ApiV1UrlPoolsIdUrlsUrlIdDelete) | **Delete** /api/v1/url-pools/{id}/urls/{urlId} | Soft-delete a single URL.
[**ApiV1UrlPoolsIdUrlsUrlIdGet**](URLPoolsAPI.md#ApiV1UrlPoolsIdUrlsUrlIdGet) | **Get** /api/v1/url-pools/{id}/urls/{urlId} | Show a single URL.
[**ApiV1UrlPoolsIdUrlsUrlIdPut**](URLPoolsAPI.md#ApiV1UrlPoolsIdUrlsUrlIdPut) | **Put** /api/v1/url-pools/{id}/urls/{urlId} | Update a single URL.
[**ApiV1UrlPoolsIdUrlsUrlIdTogglePut**](URLPoolsAPI.md#ApiV1UrlPoolsIdUrlsUrlIdTogglePut) | **Put** /api/v1/url-pools/{id}/urls/{urlId}/toggle | Toggle a URL on / off.
[**ApiV1UrlPoolsIdUrlsUrlIdWeightPut**](URLPoolsAPI.md#ApiV1UrlPoolsIdUrlsUrlIdWeightPut) | **Put** /api/v1/url-pools/{id}/urls/{urlId}/weight | Set a URL&#39;s rotation weight.
[**ApiV1UrlPoolsIdUsedInGet**](URLPoolsAPI.md#ApiV1UrlPoolsIdUsedInGet) | **Get** /api/v1/url-pools/{id}/used-in | List campaigns / ads that reference this URL pool.
[**ApiV1UrlPoolsPost**](URLPoolsAPI.md#ApiV1UrlPoolsPost) | **Post** /api/v1/url-pools | Create a URL pool.



## ApiV1UrlPoolsGet

> ApiV1CampaignsTypeCampaignIdAdsGet200Response ApiV1UrlPoolsGet(ctx).Page(page).PerPage(perPage).Execute()

List URL pools.

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
	page := int32(56) // int32 |  (optional) (default to 1)
	perPage := int32(56) // int32 |  (optional) (default to 50)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.URLPoolsAPI.ApiV1UrlPoolsGet(context.Background()).Page(page).PerPage(perPage).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `URLPoolsAPI.ApiV1UrlPoolsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1UrlPoolsGet`: ApiV1CampaignsTypeCampaignIdAdsGet200Response
	fmt.Fprintf(os.Stdout, "Response from `URLPoolsAPI.ApiV1UrlPoolsGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiV1UrlPoolsGetRequest struct via the builder pattern


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


## ApiV1UrlPoolsIdClonePost

> ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost200Response ApiV1UrlPoolsIdClonePost(ctx, id).Execute()

Clone a URL pool with all its URLs.



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
	resp, r, err := apiClient.URLPoolsAPI.ApiV1UrlPoolsIdClonePost(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `URLPoolsAPI.ApiV1UrlPoolsIdClonePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1UrlPoolsIdClonePost`: ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost200Response
	fmt.Fprintf(os.Stdout, "Response from `URLPoolsAPI.ApiV1UrlPoolsIdClonePost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1UrlPoolsIdClonePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost200Response**](ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1UrlPoolsIdDelete

> ApiV1UrlPoolsIdDelete(ctx, id).Execute()

Soft-delete a URL pool.

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
	r, err := apiClient.URLPoolsAPI.ApiV1UrlPoolsIdDelete(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `URLPoolsAPI.ApiV1UrlPoolsIdDelete``: %v\n", err)
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

Other parameters are passed through a pointer to a apiApiV1UrlPoolsIdDeleteRequest struct via the builder pattern


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


## ApiV1UrlPoolsIdGet

> ApiV1UrlPoolsIdGet(ctx, id).Execute()

Show one URL pool.

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
	r, err := apiClient.URLPoolsAPI.ApiV1UrlPoolsIdGet(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `URLPoolsAPI.ApiV1UrlPoolsIdGet``: %v\n", err)
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

Other parameters are passed through a pointer to a apiApiV1UrlPoolsIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1UrlPoolsIdPut

> ApiV1UrlPoolsIdPut(ctx, id).ApiV1UrlPoolsIdPutRequest(apiV1UrlPoolsIdPutRequest).Execute()

Update URL pool meta.

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
	apiV1UrlPoolsIdPutRequest := *openapiclient.NewApiV1UrlPoolsIdPutRequest() // ApiV1UrlPoolsIdPutRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.URLPoolsAPI.ApiV1UrlPoolsIdPut(context.Background(), id).ApiV1UrlPoolsIdPutRequest(apiV1UrlPoolsIdPutRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `URLPoolsAPI.ApiV1UrlPoolsIdPut``: %v\n", err)
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

Other parameters are passed through a pointer to a apiApiV1UrlPoolsIdPutRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **apiV1UrlPoolsIdPutRequest** | [**ApiV1UrlPoolsIdPutRequest**](ApiV1UrlPoolsIdPutRequest.md) |  | 

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


## ApiV1UrlPoolsIdUrlsGet

> ApiV1UrlPoolsIdUrlsGet(ctx, id).Execute()

List URLs in a pool.

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
	r, err := apiClient.URLPoolsAPI.ApiV1UrlPoolsIdUrlsGet(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `URLPoolsAPI.ApiV1UrlPoolsIdUrlsGet``: %v\n", err)
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

Other parameters are passed through a pointer to a apiApiV1UrlPoolsIdUrlsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1UrlPoolsIdUrlsPost

> ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost200Response ApiV1UrlPoolsIdUrlsPost(ctx, id).ApiV1UrlPoolsIdUrlsPostRequest(apiV1UrlPoolsIdUrlsPostRequest).Execute()

Add a URL to a pool.

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
	apiV1UrlPoolsIdUrlsPostRequest := *openapiclient.NewApiV1UrlPoolsIdUrlsPostRequest("https://example.com/lander?src={subid}") // ApiV1UrlPoolsIdUrlsPostRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.URLPoolsAPI.ApiV1UrlPoolsIdUrlsPost(context.Background(), id).ApiV1UrlPoolsIdUrlsPostRequest(apiV1UrlPoolsIdUrlsPostRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `URLPoolsAPI.ApiV1UrlPoolsIdUrlsPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1UrlPoolsIdUrlsPost`: ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost200Response
	fmt.Fprintf(os.Stdout, "Response from `URLPoolsAPI.ApiV1UrlPoolsIdUrlsPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1UrlPoolsIdUrlsPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **apiV1UrlPoolsIdUrlsPostRequest** | [**ApiV1UrlPoolsIdUrlsPostRequest**](ApiV1UrlPoolsIdUrlsPostRequest.md) |  | 

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


## ApiV1UrlPoolsIdUrlsUrlIdClonePost

> ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost200Response ApiV1UrlPoolsIdUrlsUrlIdClonePost(ctx, id, urlId).Execute()

Clone a single URL within the same pool.

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
	urlId := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.URLPoolsAPI.ApiV1UrlPoolsIdUrlsUrlIdClonePost(context.Background(), id, urlId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `URLPoolsAPI.ApiV1UrlPoolsIdUrlsUrlIdClonePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1UrlPoolsIdUrlsUrlIdClonePost`: ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost200Response
	fmt.Fprintf(os.Stdout, "Response from `URLPoolsAPI.ApiV1UrlPoolsIdUrlsUrlIdClonePost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 
**urlId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1UrlPoolsIdUrlsUrlIdClonePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost200Response**](ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1UrlPoolsIdUrlsUrlIdDelete

> ApiV1UrlPoolsIdUrlsUrlIdDelete(ctx, id, urlId).Execute()

Soft-delete a single URL.

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
	urlId := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.URLPoolsAPI.ApiV1UrlPoolsIdUrlsUrlIdDelete(context.Background(), id, urlId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `URLPoolsAPI.ApiV1UrlPoolsIdUrlsUrlIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 
**urlId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1UrlPoolsIdUrlsUrlIdDeleteRequest struct via the builder pattern


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


## ApiV1UrlPoolsIdUrlsUrlIdGet

> ApiV1UrlPoolsIdUrlsUrlIdGet(ctx, id, urlId).Execute()

Show a single URL.

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
	urlId := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.URLPoolsAPI.ApiV1UrlPoolsIdUrlsUrlIdGet(context.Background(), id, urlId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `URLPoolsAPI.ApiV1UrlPoolsIdUrlsUrlIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 
**urlId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1UrlPoolsIdUrlsUrlIdGetRequest struct via the builder pattern


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


## ApiV1UrlPoolsIdUrlsUrlIdPut

> ApiV1UrlPoolsIdUrlsUrlIdPut(ctx, id, urlId).ApiV1UrlPoolsIdUrlsUrlIdPutRequest(apiV1UrlPoolsIdUrlsUrlIdPutRequest).Execute()

Update a single URL.



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
	urlId := int32(56) // int32 | 
	apiV1UrlPoolsIdUrlsUrlIdPutRequest := *openapiclient.NewApiV1UrlPoolsIdUrlsUrlIdPutRequest() // ApiV1UrlPoolsIdUrlsUrlIdPutRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.URLPoolsAPI.ApiV1UrlPoolsIdUrlsUrlIdPut(context.Background(), id, urlId).ApiV1UrlPoolsIdUrlsUrlIdPutRequest(apiV1UrlPoolsIdUrlsUrlIdPutRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `URLPoolsAPI.ApiV1UrlPoolsIdUrlsUrlIdPut``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 
**urlId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1UrlPoolsIdUrlsUrlIdPutRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **apiV1UrlPoolsIdUrlsUrlIdPutRequest** | [**ApiV1UrlPoolsIdUrlsUrlIdPutRequest**](ApiV1UrlPoolsIdUrlsUrlIdPutRequest.md) |  | 

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


## ApiV1UrlPoolsIdUrlsUrlIdTogglePut

> ApiV1UrlPoolsIdUrlsUrlIdTogglePut(ctx, id, urlId).Execute()

Toggle a URL on / off.

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
	urlId := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.URLPoolsAPI.ApiV1UrlPoolsIdUrlsUrlIdTogglePut(context.Background(), id, urlId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `URLPoolsAPI.ApiV1UrlPoolsIdUrlsUrlIdTogglePut``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 
**urlId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1UrlPoolsIdUrlsUrlIdTogglePutRequest struct via the builder pattern


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


## ApiV1UrlPoolsIdUrlsUrlIdWeightPut

> ApiV1UrlPoolsIdUrlsUrlIdWeightPut(ctx, id, urlId).ApiV1UrlPoolsIdUrlsUrlIdWeightPutRequest(apiV1UrlPoolsIdUrlsUrlIdWeightPutRequest).Execute()

Set a URL's rotation weight.



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
	urlId := int32(56) // int32 | 
	apiV1UrlPoolsIdUrlsUrlIdWeightPutRequest := *openapiclient.NewApiV1UrlPoolsIdUrlsUrlIdWeightPutRequest(int32(123)) // ApiV1UrlPoolsIdUrlsUrlIdWeightPutRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.URLPoolsAPI.ApiV1UrlPoolsIdUrlsUrlIdWeightPut(context.Background(), id, urlId).ApiV1UrlPoolsIdUrlsUrlIdWeightPutRequest(apiV1UrlPoolsIdUrlsUrlIdWeightPutRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `URLPoolsAPI.ApiV1UrlPoolsIdUrlsUrlIdWeightPut``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 
**urlId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1UrlPoolsIdUrlsUrlIdWeightPutRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **apiV1UrlPoolsIdUrlsUrlIdWeightPutRequest** | [**ApiV1UrlPoolsIdUrlsUrlIdWeightPutRequest**](ApiV1UrlPoolsIdUrlsUrlIdWeightPutRequest.md) |  | 

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


## ApiV1UrlPoolsIdUsedInGet

> ApiV1UrlPoolsIdUsedInGet(ctx, id).Execute()

List campaigns / ads that reference this URL pool.

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
	r, err := apiClient.URLPoolsAPI.ApiV1UrlPoolsIdUsedInGet(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `URLPoolsAPI.ApiV1UrlPoolsIdUsedInGet``: %v\n", err)
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

Other parameters are passed through a pointer to a apiApiV1UrlPoolsIdUsedInGetRequest struct via the builder pattern


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


## ApiV1UrlPoolsPost

> ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost200Response ApiV1UrlPoolsPost(ctx).ApiV1UrlPoolsPostRequest(apiV1UrlPoolsPostRequest).Execute()

Create a URL pool.

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
	apiV1UrlPoolsPostRequest := *openapiclient.NewApiV1UrlPoolsPostRequest("Title_example") // ApiV1UrlPoolsPostRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.URLPoolsAPI.ApiV1UrlPoolsPost(context.Background()).ApiV1UrlPoolsPostRequest(apiV1UrlPoolsPostRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `URLPoolsAPI.ApiV1UrlPoolsPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1UrlPoolsPost`: ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost200Response
	fmt.Fprintf(os.Stdout, "Response from `URLPoolsAPI.ApiV1UrlPoolsPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiV1UrlPoolsPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **apiV1UrlPoolsPostRequest** | [**ApiV1UrlPoolsPostRequest**](ApiV1UrlPoolsPostRequest.md) |  | 

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

