# \CampaignsAPI

All URIs are relative to *https://up.go-adserver.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiV1CampaignsGet**](CampaignsAPI.md#ApiV1CampaignsGet) | **Get** /api/v1/campaigns | List the caller&#39;s campaigns across all types (or one type).
[**ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsGet**](CampaignsAPI.md#ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsGet) | **Get** /api/v1/campaigns/ron/{campaignId}/ads/{adId}/zone-bids | List per-zone bid overrides for a RON ad.
[**ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPut**](CampaignsAPI.md#ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPut) | **Put** /api/v1/campaigns/ron/{campaignId}/ads/{adId}/zone-bids | Replace the per-zone bid overrides on a RON ad.
[**ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsZoneIdDelete**](CampaignsAPI.md#ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsZoneIdDelete) | **Delete** /api/v1/campaigns/ron/{campaignId}/ads/{adId}/zone-bids/{zoneId} | Clear a single per-zone bid override.
[**ApiV1CampaignsTypeCampaignIdAdsAdIdActivePatch**](CampaignsAPI.md#ApiV1CampaignsTypeCampaignIdAdsAdIdActivePatch) | **Patch** /api/v1/campaigns/{type}/{campaignId}/ads/{adId}/active | Pause or unpause a single ad.
[**ApiV1CampaignsTypeCampaignIdAdsAdIdBidPatch**](CampaignsAPI.md#ApiV1CampaignsTypeCampaignIdAdsAdIdBidPatch) | **Patch** /api/v1/campaigns/{type}/{campaignId}/ads/{adId}/bid | Set a single ad&#39;s bid.
[**ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost**](CampaignsAPI.md#ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost) | **Post** /api/v1/campaigns/{type}/{campaignId}/ads/{adId}/clone | Clone a single ad within a campaign.
[**ApiV1CampaignsTypeCampaignIdAdsAdIdDelete**](CampaignsAPI.md#ApiV1CampaignsTypeCampaignIdAdsAdIdDelete) | **Delete** /api/v1/campaigns/{type}/{campaignId}/ads/{adId} | Soft-delete an ad.
[**ApiV1CampaignsTypeCampaignIdAdsAdIdGet**](CampaignsAPI.md#ApiV1CampaignsTypeCampaignIdAdsAdIdGet) | **Get** /api/v1/campaigns/{type}/{campaignId}/ads/{adId} | Show one ad.
[**ApiV1CampaignsTypeCampaignIdAdsAdIdPut**](CampaignsAPI.md#ApiV1CampaignsTypeCampaignIdAdsAdIdPut) | **Put** /api/v1/campaigns/{type}/{campaignId}/ads/{adId} | Update an ad.
[**ApiV1CampaignsTypeCampaignIdAdsGet**](CampaignsAPI.md#ApiV1CampaignsTypeCampaignIdAdsGet) | **Get** /api/v1/campaigns/{type}/{campaignId}/ads | List ads on a campaign.
[**ApiV1CampaignsTypeCampaignIdAdsPost**](CampaignsAPI.md#ApiV1CampaignsTypeCampaignIdAdsPost) | **Post** /api/v1/campaigns/{type}/{campaignId}/ads | Create an ad on a campaign (smart-default, JSON-only).
[**ApiV1CampaignsTypeCampaignIdSchemaAdsGet**](CampaignsAPI.md#ApiV1CampaignsTypeCampaignIdSchemaAdsGet) | **Get** /api/v1/campaigns/{type}/{campaignId}/_schema/ads | Field metadata for ad creation, scoped to a campaign.
[**ApiV1CampaignsTypeIdActivePatch**](CampaignsAPI.md#ApiV1CampaignsTypeIdActivePatch) | **Patch** /api/v1/campaigns/{type}/{id}/active | Pause or unpause a campaign.
[**ApiV1CampaignsTypeIdBidsPatch**](CampaignsAPI.md#ApiV1CampaignsTypeIdBidsPatch) | **Patch** /api/v1/campaigns/{type}/{id}/bids | Mass update bids on every ad in a campaign.
[**ApiV1CampaignsTypeIdClonePost**](CampaignsAPI.md#ApiV1CampaignsTypeIdClonePost) | **Post** /api/v1/campaigns/{type}/{id}/clone | Clone a campaign and all its ads.
[**ApiV1CampaignsTypeIdDelete**](CampaignsAPI.md#ApiV1CampaignsTypeIdDelete) | **Delete** /api/v1/campaigns/{type}/{id} | Soft-delete a campaign.
[**ApiV1CampaignsTypeIdFiltersFilterTypeFilterIdDelete**](CampaignsAPI.md#ApiV1CampaignsTypeIdFiltersFilterTypeFilterIdDelete) | **Delete** /api/v1/campaigns/{type}/{id}/filters/{filter_type}/{filter_id} | Detach a filter from this campaign.
[**ApiV1CampaignsTypeIdFiltersGet**](CampaignsAPI.md#ApiV1CampaignsTypeIdFiltersGet) | **Get** /api/v1/campaigns/{type}/{id}/filters | List filters attached to this campaign.
[**ApiV1CampaignsTypeIdFiltersPost**](CampaignsAPI.md#ApiV1CampaignsTypeIdFiltersPost) | **Post** /api/v1/campaigns/{type}/{id}/filters | Attach a filter to this campaign.
[**ApiV1CampaignsTypeIdGet**](CampaignsAPI.md#ApiV1CampaignsTypeIdGet) | **Get** /api/v1/campaigns/{type}/{id} | Get a single campaign.
[**ApiV1CampaignsTypeIdMinBidGet**](CampaignsAPI.md#ApiV1CampaignsTypeIdMinBidGet) | **Get** /api/v1/campaigns/{type}/{id}/min-bid | Get the campaign&#39;s minimum acceptable CPC bid.
[**ApiV1CampaignsTypePost**](CampaignsAPI.md#ApiV1CampaignsTypePost) | **Post** /api/v1/campaigns/{type} | Create a new campaign (smart-default).
[**ApiV1CampaignsTypeSchemaAdsGet**](CampaignsAPI.md#ApiV1CampaignsTypeSchemaAdsGet) | **Get** /api/v1/campaigns/{type}/_schema/ads | Field metadata for ad creation.
[**ApiV1CampaignsTypeSchemaGet**](CampaignsAPI.md#ApiV1CampaignsTypeSchemaGet) | **Get** /api/v1/campaigns/{type}/_schema | Field metadata for create/update.



## ApiV1CampaignsGet

> ApiV1CampaignsGet200Response ApiV1CampaignsGet(ctx).Type_(type_).Page(page).PerPage(perPage).Fields(fields).Execute()

List the caller's campaigns across all types (or one type).



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
	type_ := "type__example" // string |  (optional) (default to "all")
	page := int32(56) // int32 |  (optional) (default to 1)
	perPage := int32(56) // int32 |  (optional) (default to 50)
	fields := "fields_example" // string | CSV of fields to return; `*` returns everything available. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CampaignsAPI.ApiV1CampaignsGet(context.Background()).Type_(type_).Page(page).PerPage(perPage).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CampaignsGet`: ApiV1CampaignsGet200Response
	fmt.Fprintf(os.Stdout, "Response from `CampaignsAPI.ApiV1CampaignsGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **type_** | **string** |  | [default to &quot;all&quot;]
 **page** | **int32** |  | [default to 1]
 **perPage** | **int32** |  | [default to 50]
 **fields** | **string** | CSV of fields to return; &#x60;*&#x60; returns everything available. | 

### Return type

[**ApiV1CampaignsGet200Response**](ApiV1CampaignsGet200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsGet

> ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsGet200Response ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsGet(ctx, campaignId, adId).Execute()

List per-zone bid overrides for a RON ad.



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
	campaignId := int32(56) // int32 | 
	adId := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CampaignsAPI.ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsGet(context.Background(), campaignId, adId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsGet`: ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsGet200Response
	fmt.Fprintf(os.Stdout, "Response from `CampaignsAPI.ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**campaignId** | **int32** |  | 
**adId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsGet200Response**](ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsGet200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPut

> ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPut200Response ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPut(ctx, campaignId, adId).ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPutRequest(apiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPutRequest).Execute()

Replace the per-zone bid overrides on a RON ad.



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
	campaignId := int32(56) // int32 | 
	adId := int32(56) // int32 | 
	apiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPutRequest := *openapiclient.NewApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPutRequest([]openapiclient.ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPutRequestZoneBidsInner{*openapiclient.NewApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPutRequestZoneBidsInner(int32(123), float32(123))}) // ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPutRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CampaignsAPI.ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPut(context.Background(), campaignId, adId).ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPutRequest(apiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPutRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPut``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPut`: ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPut200Response
	fmt.Fprintf(os.Stdout, "Response from `CampaignsAPI.ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPut`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**campaignId** | **int32** |  | 
**adId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPutRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **apiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPutRequest** | [**ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPutRequest**](ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPutRequest.md) |  | 

### Return type

[**ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPut200Response**](ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsPut200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsZoneIdDelete

> ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsZoneIdDelete200Response ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsZoneIdDelete(ctx, campaignId, adId, zoneId).Execute()

Clear a single per-zone bid override.



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
	campaignId := int32(56) // int32 | 
	adId := int32(56) // int32 | 
	zoneId := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CampaignsAPI.ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsZoneIdDelete(context.Background(), campaignId, adId, zoneId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsZoneIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsZoneIdDelete`: ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsZoneIdDelete200Response
	fmt.Fprintf(os.Stdout, "Response from `CampaignsAPI.ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsZoneIdDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**campaignId** | **int32** |  | 
**adId** | **int32** |  | 
**zoneId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsZoneIdDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

[**ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsZoneIdDelete200Response**](ApiV1CampaignsRonCampaignIdAdsAdIdZoneBidsZoneIdDelete200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1CampaignsTypeCampaignIdAdsAdIdActivePatch

> ApiV1CampaignsTypeIdActivePatch200Response ApiV1CampaignsTypeCampaignIdAdsAdIdActivePatch(ctx, type_, campaignId, adId).ApiV1CampaignsTypeIdActivePatchRequest(apiV1CampaignsTypeIdActivePatchRequest).Execute()

Pause or unpause a single ad.



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
	campaignId := int32(56) // int32 | 
	adId := int32(56) // int32 | 
	apiV1CampaignsTypeIdActivePatchRequest := *openapiclient.NewApiV1CampaignsTypeIdActivePatchRequest(false) // ApiV1CampaignsTypeIdActivePatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypeCampaignIdAdsAdIdActivePatch(context.Background(), type_, campaignId, adId).ApiV1CampaignsTypeIdActivePatchRequest(apiV1CampaignsTypeIdActivePatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypeCampaignIdAdsAdIdActivePatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CampaignsTypeCampaignIdAdsAdIdActivePatch`: ApiV1CampaignsTypeIdActivePatch200Response
	fmt.Fprintf(os.Stdout, "Response from `CampaignsAPI.ApiV1CampaignsTypeCampaignIdAdsAdIdActivePatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**campaignId** | **int32** |  | 
**adId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypeCampaignIdAdsAdIdActivePatchRequest struct via the builder pattern


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


## ApiV1CampaignsTypeCampaignIdAdsAdIdBidPatch

> ApiV1CampaignsTypeCampaignIdAdsAdIdBidPatch200Response ApiV1CampaignsTypeCampaignIdAdsAdIdBidPatch(ctx, type_, campaignId, adId).ApiV1CampaignsTypeCampaignIdAdsAdIdBidPatchRequest(apiV1CampaignsTypeCampaignIdAdsAdIdBidPatchRequest).Execute()

Set a single ad's bid.



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
	campaignId := int32(56) // int32 | 
	adId := int32(56) // int32 | 
	apiV1CampaignsTypeCampaignIdAdsAdIdBidPatchRequest := *openapiclient.NewApiV1CampaignsTypeCampaignIdAdsAdIdBidPatchRequest(float32(123)) // ApiV1CampaignsTypeCampaignIdAdsAdIdBidPatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypeCampaignIdAdsAdIdBidPatch(context.Background(), type_, campaignId, adId).ApiV1CampaignsTypeCampaignIdAdsAdIdBidPatchRequest(apiV1CampaignsTypeCampaignIdAdsAdIdBidPatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypeCampaignIdAdsAdIdBidPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CampaignsTypeCampaignIdAdsAdIdBidPatch`: ApiV1CampaignsTypeCampaignIdAdsAdIdBidPatch200Response
	fmt.Fprintf(os.Stdout, "Response from `CampaignsAPI.ApiV1CampaignsTypeCampaignIdAdsAdIdBidPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**campaignId** | **int32** |  | 
**adId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypeCampaignIdAdsAdIdBidPatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **apiV1CampaignsTypeCampaignIdAdsAdIdBidPatchRequest** | [**ApiV1CampaignsTypeCampaignIdAdsAdIdBidPatchRequest**](ApiV1CampaignsTypeCampaignIdAdsAdIdBidPatchRequest.md) |  | 

### Return type

[**ApiV1CampaignsTypeCampaignIdAdsAdIdBidPatch200Response**](ApiV1CampaignsTypeCampaignIdAdsAdIdBidPatch200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost

> ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost200Response ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost(ctx, type_, campaignId, adId).Execute()

Clone a single ad within a campaign.



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
	campaignId := int32(56) // int32 | 
	adId := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost(context.Background(), type_, campaignId, adId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost`: ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost200Response
	fmt.Fprintf(os.Stdout, "Response from `CampaignsAPI.ApiV1CampaignsTypeCampaignIdAdsAdIdClonePost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**campaignId** | **int32** |  | 
**adId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypeCampaignIdAdsAdIdClonePostRequest struct via the builder pattern


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


## ApiV1CampaignsTypeCampaignIdAdsAdIdDelete

> ApiV1CampaignsTypeCampaignIdAdsAdIdDelete(ctx, type_, campaignId, adId).Execute()

Soft-delete an ad.

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
	campaignId := int32(56) // int32 | 
	adId := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypeCampaignIdAdsAdIdDelete(context.Background(), type_, campaignId, adId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypeCampaignIdAdsAdIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**campaignId** | **int32** |  | 
**adId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypeCampaignIdAdsAdIdDeleteRequest struct via the builder pattern


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


## ApiV1CampaignsTypeCampaignIdAdsAdIdGet

> ApiV1CampaignsTypeCampaignIdAdsAdIdGet(ctx, type_, campaignId, adId).Execute()

Show one ad.

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
	campaignId := int32(56) // int32 | 
	adId := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypeCampaignIdAdsAdIdGet(context.Background(), type_, campaignId, adId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypeCampaignIdAdsAdIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**campaignId** | **int32** |  | 
**adId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypeCampaignIdAdsAdIdGetRequest struct via the builder pattern


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


## ApiV1CampaignsTypeCampaignIdAdsAdIdPut

> ApiV1CampaignsTypeCampaignIdAdsAdIdPut(ctx, type_, campaignId, adId).ApiV1CampaignsTypeCampaignIdAdsAdIdPutRequest(apiV1CampaignsTypeCampaignIdAdsAdIdPutRequest).Execute()

Update an ad.



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
	campaignId := int32(56) // int32 | 
	adId := int32(56) // int32 | 
	apiV1CampaignsTypeCampaignIdAdsAdIdPutRequest := *openapiclient.NewApiV1CampaignsTypeCampaignIdAdsAdIdPutRequest() // ApiV1CampaignsTypeCampaignIdAdsAdIdPutRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypeCampaignIdAdsAdIdPut(context.Background(), type_, campaignId, adId).ApiV1CampaignsTypeCampaignIdAdsAdIdPutRequest(apiV1CampaignsTypeCampaignIdAdsAdIdPutRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypeCampaignIdAdsAdIdPut``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**campaignId** | **int32** |  | 
**adId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypeCampaignIdAdsAdIdPutRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **apiV1CampaignsTypeCampaignIdAdsAdIdPutRequest** | [**ApiV1CampaignsTypeCampaignIdAdsAdIdPutRequest**](ApiV1CampaignsTypeCampaignIdAdsAdIdPutRequest.md) |  | 

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


## ApiV1CampaignsTypeCampaignIdAdsGet

> ApiV1CampaignsTypeCampaignIdAdsGet200Response ApiV1CampaignsTypeCampaignIdAdsGet(ctx, type_, campaignId).Page(page).PerPage(perPage).Execute()

List ads on a campaign.



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
	campaignId := int32(56) // int32 | 
	page := int32(56) // int32 |  (optional) (default to 1)
	perPage := int32(56) // int32 |  (optional) (default to 50)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypeCampaignIdAdsGet(context.Background(), type_, campaignId).Page(page).PerPage(perPage).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypeCampaignIdAdsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CampaignsTypeCampaignIdAdsGet`: ApiV1CampaignsTypeCampaignIdAdsGet200Response
	fmt.Fprintf(os.Stdout, "Response from `CampaignsAPI.ApiV1CampaignsTypeCampaignIdAdsGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**campaignId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypeCampaignIdAdsGetRequest struct via the builder pattern


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


## ApiV1CampaignsTypeCampaignIdAdsPost

> ApiV1CampaignsTypeCampaignIdAdsPost(ctx, type_, campaignId).ApiV1CampaignsTypeCampaignIdAdsPostRequest(apiV1CampaignsTypeCampaignIdAdsPostRequest).DryRun(dryRun).Strict(strict).Execute()

Create an ad on a campaign (smart-default, JSON-only).



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
	campaignId := int32(56) // int32 | 
	apiV1CampaignsTypeCampaignIdAdsPostRequest := *openapiclient.NewApiV1CampaignsTypeCampaignIdAdsPostRequest("Promo Q3 banner", float32(0.0042)) // ApiV1CampaignsTypeCampaignIdAdsPostRequest | 
	dryRun := "dryRun_example" // string |  (optional)
	strict := "strict_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypeCampaignIdAdsPost(context.Background(), type_, campaignId).ApiV1CampaignsTypeCampaignIdAdsPostRequest(apiV1CampaignsTypeCampaignIdAdsPostRequest).DryRun(dryRun).Strict(strict).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypeCampaignIdAdsPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**campaignId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypeCampaignIdAdsPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **apiV1CampaignsTypeCampaignIdAdsPostRequest** | [**ApiV1CampaignsTypeCampaignIdAdsPostRequest**](ApiV1CampaignsTypeCampaignIdAdsPostRequest.md) |  | 
 **dryRun** | **string** |  | 
 **strict** | **string** |  | 

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


## ApiV1CampaignsTypeCampaignIdSchemaAdsGet

> ApiV1CampaignsTypeCampaignIdSchemaAdsGet(ctx, type_, campaignId).Execute()

Field metadata for ad creation, scoped to a campaign.



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
	campaignId := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypeCampaignIdSchemaAdsGet(context.Background(), type_, campaignId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypeCampaignIdSchemaAdsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**campaignId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypeCampaignIdSchemaAdsGetRequest struct via the builder pattern


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


## ApiV1CampaignsTypeIdActivePatch

> ApiV1CampaignsTypeIdActivePatch200Response ApiV1CampaignsTypeIdActivePatch(ctx, type_, id).ApiV1CampaignsTypeIdActivePatchRequest(apiV1CampaignsTypeIdActivePatchRequest).Execute()

Pause or unpause a campaign.



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
	resp, r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypeIdActivePatch(context.Background(), type_, id).ApiV1CampaignsTypeIdActivePatchRequest(apiV1CampaignsTypeIdActivePatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypeIdActivePatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CampaignsTypeIdActivePatch`: ApiV1CampaignsTypeIdActivePatch200Response
	fmt.Fprintf(os.Stdout, "Response from `CampaignsAPI.ApiV1CampaignsTypeIdActivePatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypeIdActivePatchRequest struct via the builder pattern


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


## ApiV1CampaignsTypeIdBidsPatch

> ApiV1CampaignsTypeIdBidsPatch200Response ApiV1CampaignsTypeIdBidsPatch(ctx, type_, id).ApiV1CampaignsTypeIdBidsPatchRequest(apiV1CampaignsTypeIdBidsPatchRequest).Execute()

Mass update bids on every ad in a campaign.



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
	apiV1CampaignsTypeIdBidsPatchRequest := *openapiclient.NewApiV1CampaignsTypeIdBidsPatchRequest("Mode_example") // ApiV1CampaignsTypeIdBidsPatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypeIdBidsPatch(context.Background(), type_, id).ApiV1CampaignsTypeIdBidsPatchRequest(apiV1CampaignsTypeIdBidsPatchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypeIdBidsPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CampaignsTypeIdBidsPatch`: ApiV1CampaignsTypeIdBidsPatch200Response
	fmt.Fprintf(os.Stdout, "Response from `CampaignsAPI.ApiV1CampaignsTypeIdBidsPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypeIdBidsPatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **apiV1CampaignsTypeIdBidsPatchRequest** | [**ApiV1CampaignsTypeIdBidsPatchRequest**](ApiV1CampaignsTypeIdBidsPatchRequest.md) |  | 

### Return type

[**ApiV1CampaignsTypeIdBidsPatch200Response**](ApiV1CampaignsTypeIdBidsPatch200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1CampaignsTypeIdClonePost

> ApiV1CampaignsTypeIdClonePost201Response ApiV1CampaignsTypeIdClonePost(ctx, type_, id).ApiV1CampaignsTypeIdClonePostRequest(apiV1CampaignsTypeIdClonePostRequest).Execute()

Clone a campaign and all its ads.



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
	apiV1CampaignsTypeIdClonePostRequest := *openapiclient.NewApiV1CampaignsTypeIdClonePostRequest() // ApiV1CampaignsTypeIdClonePostRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypeIdClonePost(context.Background(), type_, id).ApiV1CampaignsTypeIdClonePostRequest(apiV1CampaignsTypeIdClonePostRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypeIdClonePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CampaignsTypeIdClonePost`: ApiV1CampaignsTypeIdClonePost201Response
	fmt.Fprintf(os.Stdout, "Response from `CampaignsAPI.ApiV1CampaignsTypeIdClonePost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypeIdClonePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **apiV1CampaignsTypeIdClonePostRequest** | [**ApiV1CampaignsTypeIdClonePostRequest**](ApiV1CampaignsTypeIdClonePostRequest.md) |  | 

### Return type

[**ApiV1CampaignsTypeIdClonePost201Response**](ApiV1CampaignsTypeIdClonePost201Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1CampaignsTypeIdDelete

> ApiV1CampaignsTypeIdDelete200Response ApiV1CampaignsTypeIdDelete(ctx, type_, id).Execute()

Soft-delete a campaign.



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
	resp, r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypeIdDelete(context.Background(), type_, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypeIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CampaignsTypeIdDelete`: ApiV1CampaignsTypeIdDelete200Response
	fmt.Fprintf(os.Stdout, "Response from `CampaignsAPI.ApiV1CampaignsTypeIdDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypeIdDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ApiV1CampaignsTypeIdDelete200Response**](ApiV1CampaignsTypeIdDelete200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1CampaignsTypeIdFiltersFilterTypeFilterIdDelete

> ApiV1CampaignsTypeIdFiltersFilterTypeFilterIdDelete(ctx, type_, id, filterType, filterId).Execute()

Detach a filter from this campaign.



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
	filterType := "filterType_example" // string | 
	filterId := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypeIdFiltersFilterTypeFilterIdDelete(context.Background(), type_, id, filterType, filterId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypeIdFiltersFilterTypeFilterIdDelete``: %v\n", err)
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
**filterType** | **string** |  | 
**filterId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypeIdFiltersFilterTypeFilterIdDeleteRequest struct via the builder pattern


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


## ApiV1CampaignsTypeIdFiltersGet

> ApiV1CampaignsTypeIdFiltersGet200Response ApiV1CampaignsTypeIdFiltersGet(ctx, type_, id).Execute()

List filters attached to this campaign.



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
	resp, r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypeIdFiltersGet(context.Background(), type_, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypeIdFiltersGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CampaignsTypeIdFiltersGet`: ApiV1CampaignsTypeIdFiltersGet200Response
	fmt.Fprintf(os.Stdout, "Response from `CampaignsAPI.ApiV1CampaignsTypeIdFiltersGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypeIdFiltersGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ApiV1CampaignsTypeIdFiltersGet200Response**](ApiV1CampaignsTypeIdFiltersGet200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1CampaignsTypeIdFiltersPost

> ApiV1CampaignsTypeIdFiltersPost200Response ApiV1CampaignsTypeIdFiltersPost(ctx, type_, id).ApiV1CampaignsTypeIdFiltersPostRequest(apiV1CampaignsTypeIdFiltersPostRequest).Execute()

Attach a filter to this campaign.



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
	apiV1CampaignsTypeIdFiltersPostRequest := *openapiclient.NewApiV1CampaignsTypeIdFiltersPostRequest("FilterType_example", int32(123)) // ApiV1CampaignsTypeIdFiltersPostRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypeIdFiltersPost(context.Background(), type_, id).ApiV1CampaignsTypeIdFiltersPostRequest(apiV1CampaignsTypeIdFiltersPostRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypeIdFiltersPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CampaignsTypeIdFiltersPost`: ApiV1CampaignsTypeIdFiltersPost200Response
	fmt.Fprintf(os.Stdout, "Response from `CampaignsAPI.ApiV1CampaignsTypeIdFiltersPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypeIdFiltersPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **apiV1CampaignsTypeIdFiltersPostRequest** | [**ApiV1CampaignsTypeIdFiltersPostRequest**](ApiV1CampaignsTypeIdFiltersPostRequest.md) |  | 

### Return type

[**ApiV1CampaignsTypeIdFiltersPost200Response**](ApiV1CampaignsTypeIdFiltersPost200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1CampaignsTypeIdGet

> map[string]interface{} ApiV1CampaignsTypeIdGet(ctx, type_, id).Execute()

Get a single campaign.

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
	resp, r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypeIdGet(context.Background(), type_, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypeIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CampaignsTypeIdGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `CampaignsAPI.ApiV1CampaignsTypeIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypeIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

**map[string]interface{}**

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1CampaignsTypeIdMinBidGet

> ApiV1CampaignsTypeIdMinBidGet200Response ApiV1CampaignsTypeIdMinBidGet(ctx, type_, id).Execute()

Get the campaign's minimum acceptable CPC bid.



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
	resp, r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypeIdMinBidGet(context.Background(), type_, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypeIdMinBidGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CampaignsTypeIdMinBidGet`: ApiV1CampaignsTypeIdMinBidGet200Response
	fmt.Fprintf(os.Stdout, "Response from `CampaignsAPI.ApiV1CampaignsTypeIdMinBidGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 
**id** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypeIdMinBidGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ApiV1CampaignsTypeIdMinBidGet200Response**](ApiV1CampaignsTypeIdMinBidGet200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1CampaignsTypePost

> ApiV1CampaignsTypePost(ctx, type_).ApiV1CampaignsTypePostRequest(apiV1CampaignsTypePostRequest).DryRun(dryRun).Strict(strict).Execute()

Create a new campaign (smart-default).



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
	apiV1CampaignsTypePostRequest := *openapiclient.NewApiV1CampaignsTypePostRequest("Auto-optimised RON #1", int32(2)) // ApiV1CampaignsTypePostRequest | 
	dryRun := "dryRun_example" // string |  (optional)
	strict := "strict_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypePost(context.Background(), type_).ApiV1CampaignsTypePostRequest(apiV1CampaignsTypePostRequest).DryRun(dryRun).Strict(strict).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **apiV1CampaignsTypePostRequest** | [**ApiV1CampaignsTypePostRequest**](ApiV1CampaignsTypePostRequest.md) |  | 
 **dryRun** | **string** |  | 
 **strict** | **string** |  | 

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


## ApiV1CampaignsTypeSchemaAdsGet

> ApiV1CampaignsTypeSchemaAdsGet200Response ApiV1CampaignsTypeSchemaAdsGet(ctx, type_).Execute()

Field metadata for ad creation.



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypeSchemaAdsGet(context.Background(), type_).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypeSchemaAdsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CampaignsTypeSchemaAdsGet`: ApiV1CampaignsTypeSchemaAdsGet200Response
	fmt.Fprintf(os.Stdout, "Response from `CampaignsAPI.ApiV1CampaignsTypeSchemaAdsGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypeSchemaAdsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ApiV1CampaignsTypeSchemaAdsGet200Response**](ApiV1CampaignsTypeSchemaAdsGet200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ApiV1CampaignsTypeSchemaGet

> ApiV1CampaignsTypeSchemaGet200Response ApiV1CampaignsTypeSchemaGet(ctx, type_).Execute()

Field metadata for create/update.



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CampaignsAPI.ApiV1CampaignsTypeSchemaGet(context.Background(), type_).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CampaignsAPI.ApiV1CampaignsTypeSchemaGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApiV1CampaignsTypeSchemaGet`: ApiV1CampaignsTypeSchemaGet200Response
	fmt.Fprintf(os.Stdout, "Response from `CampaignsAPI.ApiV1CampaignsTypeSchemaGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApiV1CampaignsTypeSchemaGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ApiV1CampaignsTypeSchemaGet200Response**](ApiV1CampaignsTypeSchemaGet200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

