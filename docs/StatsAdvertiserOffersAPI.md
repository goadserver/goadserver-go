# \StatsAdvertiserOffersAPI

All URIs are relative to *https://up.goadserver.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiV1AdvertiserOffersStatsGet**](StatsAdvertiserOffersAPI.md#ApiV1AdvertiserOffersStatsGet) | **Get** /api/v1/advertiser/offers/stats | CPA / affiliate offer performance — advertiser side.



## ApiV1AdvertiserOffersStatsGet

> StatsResponse ApiV1AdvertiserOffersStatsGet(ctx).From(from).To(to).Interval(interval).GroupBy(groupBy).Metrics(metrics).Format(format).Page(page).PerPage(perPage).Sort(sort).Execute()

CPA / affiliate offer performance — advertiser side.



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/goadserver/goadserver-go"
)

func main() {
	from := time.Now() // string | ISO date — inclusive start. Defaults to 7 days ago. (optional)
	to := time.Now() // string | ISO date — inclusive end. Defaults to today. Max range 92 days. (optional)
	interval := "interval_example" // string |  (optional) (default to "sum")
	groupBy := "groupBy_example" // string | Comma-separated dimensions to aggregate by, in priority order. Max 4 dimensions. Available dimensions vary per endpoint — see the per-endpoint description.  (optional)
	metrics := "metrics_example" // string | Optional comma-separated metric whitelist. When omitted, all metrics for the endpoint are returned.  (optional)
	format := "format_example" // string |  (optional) (default to "json")
	page := int32(56) // int32 |  (optional) (default to 1)
	perPage := int32(56) // int32 |  (optional) (default to 100)
	sort := "sort_example" // string | Field name. Prefix with `-` for descending (e.g. `-views`). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StatsAdvertiserOffersAPI.ApiV1AdvertiserOffersStatsGet(context.Background()).From(from).To(to).Interval(interval).GroupBy(groupBy).Metrics(metrics).Format(format).Page(page).PerPage(perPage).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StatsAdvertiserOffersAPI.ApiV1AdvertiserOffersStatsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1AdvertiserOffersStatsGet`: StatsResponse
	fmt.Fprintf(os.Stdout, "Response from `StatsAdvertiserOffersAPI.ApiV1AdvertiserOffersStatsGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiV1AdvertiserOffersStatsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **from** | **string** | ISO date — inclusive start. Defaults to 7 days ago. | 
 **to** | **string** | ISO date — inclusive end. Defaults to today. Max range 92 days. | 
 **interval** | **string** |  | [default to &quot;sum&quot;]
 **groupBy** | **string** | Comma-separated dimensions to aggregate by, in priority order. Max 4 dimensions. Available dimensions vary per endpoint — see the per-endpoint description.  | 
 **metrics** | **string** | Optional comma-separated metric whitelist. When omitted, all metrics for the endpoint are returned.  | 
 **format** | **string** |  | [default to &quot;json&quot;]
 **page** | **int32** |  | [default to 1]
 **perPage** | **int32** |  | [default to 100]
 **sort** | **string** | Field name. Prefix with &#x60;-&#x60; for descending (e.g. &#x60;-views&#x60;). | 

### Return type

[**StatsResponse**](StatsResponse.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

