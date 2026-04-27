# \PublicAPI

All URIs are relative to *https://up.go-adserver.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiPublicOpenapiJsonGet**](PublicAPI.md#ApiPublicOpenapiJsonGet) | **Get** /api/public/openapi.json | OpenAPI spec as JSON.
[**ApiPublicOpenapiYamlGet**](PublicAPI.md#ApiPublicOpenapiYamlGet) | **Get** /api/public/openapi.yaml | Raw OpenAPI spec (this document).
[**ApiPublicRoutesTxtGet**](PublicAPI.md#ApiPublicRoutesTxtGet) | **Get** /api/public/routes.txt | Flat list of public routes — agent-friendly.



## ApiPublicOpenapiJsonGet

> ApiPublicOpenapiJsonGet(ctx).Execute()

OpenAPI spec as JSON.

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
	r, err := apiClient.PublicAPI.ApiPublicOpenapiJsonGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PublicAPI.ApiPublicOpenapiJsonGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiPublicOpenapiJsonGetRequest struct via the builder pattern


### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiPublicOpenapiYamlGet

> ApiPublicOpenapiYamlGet(ctx).Execute()

Raw OpenAPI spec (this document).

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
	r, err := apiClient.PublicAPI.ApiPublicOpenapiYamlGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PublicAPI.ApiPublicOpenapiYamlGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiPublicOpenapiYamlGetRequest struct via the builder pattern


### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiPublicRoutesTxtGet

> ApiPublicRoutesTxtGet(ctx).Execute()

Flat list of public routes — agent-friendly.

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
	r, err := apiClient.PublicAPI.ApiPublicRoutesTxtGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PublicAPI.ApiPublicRoutesTxtGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiPublicRoutesTxtGetRequest struct via the builder pattern


### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

