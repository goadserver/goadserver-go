# \FundsAPI

All URIs are relative to *https://up.go-adserver.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiV1FundsGet**](FundsAPI.md#ApiV1FundsGet) | **Get** /api/v1/funds | Current advertiser balance + pending deposits.



## ApiV1FundsGet

> ApiV1FundsGet200Response ApiV1FundsGet(ctx).Execute()

Current advertiser balance + pending deposits.



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
	resp, r, err := apiClient.FundsAPI.ApiV1FundsGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FundsAPI.ApiV1FundsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1FundsGet`: ApiV1FundsGet200Response
	fmt.Fprintf(os.Stdout, "Response from `FundsAPI.ApiV1FundsGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1FundsGetRequest struct via the builder pattern


### Return type

[**ApiV1FundsGet200Response**](ApiV1FundsGet200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

