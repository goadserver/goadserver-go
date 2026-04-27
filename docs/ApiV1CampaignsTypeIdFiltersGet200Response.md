# ApiV1CampaignsTypeIdFiltersGet200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CampaignType** | Pointer to **string** |  | [optional] 
**CampaignId** | Pointer to **int32** |  | [optional] 
**Filters** | Pointer to [**[]ApiV1CampaignsTypeIdFiltersGet200ResponseFiltersInner**](ApiV1CampaignsTypeIdFiltersGet200ResponseFiltersInner.md) |  | [optional] 

## Methods

### NewApiV1CampaignsTypeIdFiltersGet200Response

`func NewApiV1CampaignsTypeIdFiltersGet200Response() *ApiV1CampaignsTypeIdFiltersGet200Response`

NewApiV1CampaignsTypeIdFiltersGet200Response instantiates a new ApiV1CampaignsTypeIdFiltersGet200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiV1CampaignsTypeIdFiltersGet200ResponseWithDefaults

`func NewApiV1CampaignsTypeIdFiltersGet200ResponseWithDefaults() *ApiV1CampaignsTypeIdFiltersGet200Response`

NewApiV1CampaignsTypeIdFiltersGet200ResponseWithDefaults instantiates a new ApiV1CampaignsTypeIdFiltersGet200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCampaignType

`func (o *ApiV1CampaignsTypeIdFiltersGet200Response) GetCampaignType() string`

GetCampaignType returns the CampaignType field if non-nil, zero value otherwise.

### GetCampaignTypeOk

`func (o *ApiV1CampaignsTypeIdFiltersGet200Response) GetCampaignTypeOk() (*string, bool)`

GetCampaignTypeOk returns a tuple with the CampaignType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCampaignType

`func (o *ApiV1CampaignsTypeIdFiltersGet200Response) SetCampaignType(v string)`

SetCampaignType sets CampaignType field to given value.

### HasCampaignType

`func (o *ApiV1CampaignsTypeIdFiltersGet200Response) HasCampaignType() bool`

HasCampaignType returns a boolean if a field has been set.

### GetCampaignId

`func (o *ApiV1CampaignsTypeIdFiltersGet200Response) GetCampaignId() int32`

GetCampaignId returns the CampaignId field if non-nil, zero value otherwise.

### GetCampaignIdOk

`func (o *ApiV1CampaignsTypeIdFiltersGet200Response) GetCampaignIdOk() (*int32, bool)`

GetCampaignIdOk returns a tuple with the CampaignId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCampaignId

`func (o *ApiV1CampaignsTypeIdFiltersGet200Response) SetCampaignId(v int32)`

SetCampaignId sets CampaignId field to given value.

### HasCampaignId

`func (o *ApiV1CampaignsTypeIdFiltersGet200Response) HasCampaignId() bool`

HasCampaignId returns a boolean if a field has been set.

### GetFilters

`func (o *ApiV1CampaignsTypeIdFiltersGet200Response) GetFilters() []ApiV1CampaignsTypeIdFiltersGet200ResponseFiltersInner`

GetFilters returns the Filters field if non-nil, zero value otherwise.

### GetFiltersOk

`func (o *ApiV1CampaignsTypeIdFiltersGet200Response) GetFiltersOk() (*[]ApiV1CampaignsTypeIdFiltersGet200ResponseFiltersInner, bool)`

GetFiltersOk returns a tuple with the Filters field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilters

`func (o *ApiV1CampaignsTypeIdFiltersGet200Response) SetFilters(v []ApiV1CampaignsTypeIdFiltersGet200ResponseFiltersInner)`

SetFilters sets Filters field to given value.

### HasFilters

`func (o *ApiV1CampaignsTypeIdFiltersGet200Response) HasFilters() bool`

HasFilters returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


