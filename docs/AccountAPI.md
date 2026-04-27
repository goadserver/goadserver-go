# \AccountAPI

All URIs are relative to *https://up.goadserver.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiV1AccountGet**](AccountAPI.md#ApiV1AccountGet) | **Get** /api/v1/account | Identity check — returns the authenticated user + scopes of the calling key.



## ApiV1AccountGet

> ApiV1AccountGet200Response ApiV1AccountGet(ctx).Execute()

Identity check — returns the authenticated user + scopes of the calling key.



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
	resp, r, err := apiClient.AccountAPI.ApiV1AccountGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AccountAPI.ApiV1AccountGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1AccountGet`: ApiV1AccountGet200Response
	fmt.Fprintf(os.Stdout, "Response from `AccountAPI.ApiV1AccountGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1AccountGetRequest struct via the builder pattern


### Return type

[**ApiV1AccountGet200Response**](ApiV1AccountGet200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

