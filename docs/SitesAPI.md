# \SitesAPI

All URIs are relative to *https://up.goadserver.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiV1SitesGet**](SitesAPI.md#ApiV1SitesGet) | **Get** /api/v1/sites | List the caller&#39;s websites.



## ApiV1SitesGet

> ApiV1SitesGet200Response ApiV1SitesGet(ctx).Execute()

List the caller's websites.

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
	resp, r, err := apiClient.SitesAPI.ApiV1SitesGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SitesAPI.ApiV1SitesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1SitesGet`: ApiV1SitesGet200Response
	fmt.Fprintf(os.Stdout, "Response from `SitesAPI.ApiV1SitesGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1SitesGetRequest struct via the builder pattern


### Return type

[**ApiV1SitesGet200Response**](ApiV1SitesGet200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

