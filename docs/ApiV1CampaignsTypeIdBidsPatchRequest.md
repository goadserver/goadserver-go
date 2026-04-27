# ApiV1CampaignsTypeIdBidsPatchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Mode** | **string** |  | 
**Value** | Pointer to **float32** | Required when mode&#x3D;set. New absolute bid (&gt;&#x3D; 0). | [optional] 
**Pct** | Pointer to **float32** | Required when mode&#x3D;pct_inc / pct_dec. Percent change (&gt; 0). | [optional] 
**AdIds** | Pointer to **[]int32** | Optional. Subset of ad ids to update. Omit/empty for \&quot;all ads\&quot;. | [optional] 

## Methods

### NewApiV1CampaignsTypeIdBidsPatchRequest

`func NewApiV1CampaignsTypeIdBidsPatchRequest(mode string, ) *ApiV1CampaignsTypeIdBidsPatchRequest`

NewApiV1CampaignsTypeIdBidsPatchRequest instantiates a new ApiV1CampaignsTypeIdBidsPatchRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiV1CampaignsTypeIdBidsPatchRequestWithDefaults

`func NewApiV1CampaignsTypeIdBidsPatchRequestWithDefaults() *ApiV1CampaignsTypeIdBidsPatchRequest`

NewApiV1CampaignsTypeIdBidsPatchRequestWithDefaults instantiates a new ApiV1CampaignsTypeIdBidsPatchRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMode

`func (o *ApiV1CampaignsTypeIdBidsPatchRequest) GetMode() string`

GetMode returns the Mode field if non-nil, zero value otherwise.

### GetModeOk

`func (o *ApiV1CampaignsTypeIdBidsPatchRequest) GetModeOk() (*string, bool)`

GetModeOk returns a tuple with the Mode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMode

`func (o *ApiV1CampaignsTypeIdBidsPatchRequest) SetMode(v string)`

SetMode sets Mode field to given value.


### GetValue

`func (o *ApiV1CampaignsTypeIdBidsPatchRequest) GetValue() float32`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *ApiV1CampaignsTypeIdBidsPatchRequest) GetValueOk() (*float32, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *ApiV1CampaignsTypeIdBidsPatchRequest) SetValue(v float32)`

SetValue sets Value field to given value.

### HasValue

`func (o *ApiV1CampaignsTypeIdBidsPatchRequest) HasValue() bool`

HasValue returns a boolean if a field has been set.

### GetPct

`func (o *ApiV1CampaignsTypeIdBidsPatchRequest) GetPct() float32`

GetPct returns the Pct field if non-nil, zero value otherwise.

### GetPctOk

`func (o *ApiV1CampaignsTypeIdBidsPatchRequest) GetPctOk() (*float32, bool)`

GetPctOk returns a tuple with the Pct field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPct

`func (o *ApiV1CampaignsTypeIdBidsPatchRequest) SetPct(v float32)`

SetPct sets Pct field to given value.

### HasPct

`func (o *ApiV1CampaignsTypeIdBidsPatchRequest) HasPct() bool`

HasPct returns a boolean if a field has been set.

### GetAdIds

`func (o *ApiV1CampaignsTypeIdBidsPatchRequest) GetAdIds() []int32`

GetAdIds returns the AdIds field if non-nil, zero value otherwise.

### GetAdIdsOk

`func (o *ApiV1CampaignsTypeIdBidsPatchRequest) GetAdIdsOk() (*[]int32, bool)`

GetAdIdsOk returns a tuple with the AdIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdIds

`func (o *ApiV1CampaignsTypeIdBidsPatchRequest) SetAdIds(v []int32)`

SetAdIds sets AdIds field to given value.

### HasAdIds

`func (o *ApiV1CampaignsTypeIdBidsPatchRequest) HasAdIds() bool`

HasAdIds returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


