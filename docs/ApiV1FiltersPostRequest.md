# ApiV1FiltersPostRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** |  | 
**Name** | **string** |  | 
**Items** | **[]string** |  | 
**CampaignIds** | Pointer to **[]int32** | Exclusion filters: limits this filter to these campaigns. Empty/omitted &#x3D; applies to all. | [optional] 
**AdType** | Pointer to **int32** | 0 &#x3D; all ad types, otherwise the adtypeid this filter applies to. | [optional] [default to 0]

## Methods

### NewApiV1FiltersPostRequest

`func NewApiV1FiltersPostRequest(type_ string, name string, items []string, ) *ApiV1FiltersPostRequest`

NewApiV1FiltersPostRequest instantiates a new ApiV1FiltersPostRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiV1FiltersPostRequestWithDefaults

`func NewApiV1FiltersPostRequestWithDefaults() *ApiV1FiltersPostRequest`

NewApiV1FiltersPostRequestWithDefaults instantiates a new ApiV1FiltersPostRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *ApiV1FiltersPostRequest) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ApiV1FiltersPostRequest) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ApiV1FiltersPostRequest) SetType(v string)`

SetType sets Type field to given value.


### GetName

`func (o *ApiV1FiltersPostRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ApiV1FiltersPostRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ApiV1FiltersPostRequest) SetName(v string)`

SetName sets Name field to given value.


### GetItems

`func (o *ApiV1FiltersPostRequest) GetItems() []string`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *ApiV1FiltersPostRequest) GetItemsOk() (*[]string, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *ApiV1FiltersPostRequest) SetItems(v []string)`

SetItems sets Items field to given value.


### GetCampaignIds

`func (o *ApiV1FiltersPostRequest) GetCampaignIds() []int32`

GetCampaignIds returns the CampaignIds field if non-nil, zero value otherwise.

### GetCampaignIdsOk

`func (o *ApiV1FiltersPostRequest) GetCampaignIdsOk() (*[]int32, bool)`

GetCampaignIdsOk returns a tuple with the CampaignIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCampaignIds

`func (o *ApiV1FiltersPostRequest) SetCampaignIds(v []int32)`

SetCampaignIds sets CampaignIds field to given value.

### HasCampaignIds

`func (o *ApiV1FiltersPostRequest) HasCampaignIds() bool`

HasCampaignIds returns a boolean if a field has been set.

### GetAdType

`func (o *ApiV1FiltersPostRequest) GetAdType() int32`

GetAdType returns the AdType field if non-nil, zero value otherwise.

### GetAdTypeOk

`func (o *ApiV1FiltersPostRequest) GetAdTypeOk() (*int32, bool)`

GetAdTypeOk returns a tuple with the AdType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdType

`func (o *ApiV1FiltersPostRequest) SetAdType(v int32)`

SetAdType sets AdType field to given value.

### HasAdType

`func (o *ApiV1FiltersPostRequest) HasAdType() bool`

HasAdType returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


