# \AdspacesAPI

All URIs are relative to *https://up.goadserver.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiV1AdspacesGet**](AdspacesAPI.md#ApiV1AdspacesGet) | **Get** /api/v1/adspaces | List ad zones owned by the caller.
[**ApiV1AdspacesIdActivePatch**](AdspacesAPI.md#ApiV1AdspacesIdActivePatch) | **Patch** /api/v1/adspaces/{id}/active | Activate or deactivate an adspace.
[**ApiV1AdspacesIdGet**](AdspacesAPI.md#ApiV1AdspacesIdGet) | **Get** /api/v1/adspaces/{id} | Get a single adspace.



## ApiV1AdspacesGet

> ApiV1AdspacesGet200Response ApiV1AdspacesGet(ctx).SiteId(siteId).Page(page).PerPage(perPage).Execute()

List ad zones owned by the caller.

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
	siteId := int32(56) // int32 | Filter to one site. (optional)
	page := int32(56) // int32 |  (optional) (default to 1)
	perPage := int32(56) // int32 |  (optional) (default to 100)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AdspacesAPI.ApiV1AdspacesGet(context.Background()).SiteId(siteId).Page(page).PerPage(perPage).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdspacesAPI.ApiV1AdspacesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1AdspacesGet`: ApiV1AdspacesGet200Response
	fmt.Fprintf(os.Stdout, "Response from `AdspacesAPI.ApiV1AdspacesGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiV1AdspacesGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **siteId** | **int32** | Filter to one site. | 
 **page** | **int32** |  | [default to 1]
 **perPage** | **int32** |  | [default to 100]

### Return type

[**ApiV1AdspacesGet200Response**](ApiV1AdspacesGet200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1AdspacesIdActivePatch

> ApiV1CampaignsTypeIdActivePatch200Response ApiV1AdspacesIdActivePatch(ctx, id).ApiV1CampaignsTypeIdActivePatchRequest(apiV1CampaignsTypeIdActivePatchRequest).Execute()

Activate or deactivate an adspace.



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
	resp, r, err := apiClient.AdspacesAPI.ApiV1AdspacesIdActivePatch(context.Background(), id).ApiV1CampaignsTypeIdActivePatchRequest(apiV1CampaignsTypeIdActivePatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdspacesAPI.ApiV1AdspacesIdActivePatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1AdspacesIdActivePatch`: ApiV1CampaignsTypeIdActivePatch200Response
	fmt.Fprintf(os.Stdout, "Response from `AdspacesAPI.ApiV1AdspacesIdActivePatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1AdspacesIdActivePatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **apiV1CampaignsTypeIdActivePatchRequest** | [**ApiV1CampaignsTypeIdActivePatchRequest**](ApiV1CampaignsTypeIdActivePatchRequest.md) |  | 

### Return type

[**ApiV1CampaignsTypeIdActivePatch200Response**](ApiV1CampaignsTypeIdActivePatch200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1AdspacesIdGet

> ApiV1AdspacesIdGet(ctx, id).Execute()

Get a single adspace.

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
	r, err := apiClient.AdspacesAPI.ApiV1AdspacesIdGet(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdspacesAPI.ApiV1AdspacesIdGet``: %v\n", err)
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

Other parameters are passed through a pointer to a apiApiV1AdspacesIdGetRequest struct via the builder pattern


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

