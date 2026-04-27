# ApiV1CampaignsGet200ResponseDataInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **int32** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**CampaignType** | Pointer to **string** |  | [optional] 
**AdType** | Pointer to **int32** |  | [optional] 
**SellingType** | Pointer to **int32** |  | [optional] 
**IsPaused** | Pointer to **bool** |  | [optional] 
**IsActive** | Pointer to **bool** |  | [optional] 
**IsDeleted** | Pointer to **bool** |  | [optional] 

## Methods

### NewApiV1CampaignsGet200ResponseDataInner

`func NewApiV1CampaignsGet200ResponseDataInner() *ApiV1CampaignsGet200ResponseDataInner`

NewApiV1CampaignsGet200ResponseDataInner instantiates a new ApiV1CampaignsGet200ResponseDataInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiV1CampaignsGet200ResponseDataInnerWithDefaults

`func NewApiV1CampaignsGet200ResponseDataInnerWithDefaults() *ApiV1CampaignsGet200ResponseDataInner`

NewApiV1CampaignsGet200ResponseDataInnerWithDefaults instantiates a new ApiV1CampaignsGet200ResponseDataInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ApiV1CampaignsGet200ResponseDataInner) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ApiV1CampaignsGet200ResponseDataInner) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ApiV1CampaignsGet200ResponseDataInner) SetId(v int32)`

SetId sets Id field to given value.

### HasId

`func (o *ApiV1CampaignsGet200ResponseDataInner) HasId() bool`

HasId returns a boolean if a field has been set.

### GetName

`func (o *ApiV1CampaignsGet200ResponseDataInner) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ApiV1CampaignsGet200ResponseDataInner) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ApiV1CampaignsGet200ResponseDataInner) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ApiV1CampaignsGet200ResponseDataInner) HasName() bool`

HasName returns a boolean if a field has been set.

### GetCampaignType

`func (o *ApiV1CampaignsGet200ResponseDataInner) GetCampaignType() string`

GetCampaignType returns the CampaignType field if non-nil, zero value otherwise.

### GetCampaignTypeOk

`func (o *ApiV1CampaignsGet200ResponseDataInner) GetCampaignTypeOk() (*string, bool)`

GetCampaignTypeOk returns a tuple with the CampaignType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCampaignType

`func (o *ApiV1CampaignsGet200ResponseDataInner) SetCampaignType(v string)`

SetCampaignType sets CampaignType field to given value.

### HasCampaignType

`func (o *ApiV1CampaignsGet200ResponseDataInner) HasCampaignType() bool`

HasCampaignType returns a boolean if a field has been set.

### GetAdType

`func (o *ApiV1CampaignsGet200ResponseDataInner) GetAdType() int32`

GetAdType returns the AdType field if non-nil, zero value otherwise.

### GetAdTypeOk

`func (o *ApiV1CampaignsGet200ResponseDataInner) GetAdTypeOk() (*int32, bool)`

GetAdTypeOk returns a tuple with the AdType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdType

`func (o *ApiV1CampaignsGet200ResponseDataInner) SetAdType(v int32)`

SetAdType sets AdType field to given value.

### HasAdType

`func (o *ApiV1CampaignsGet200ResponseDataInner) HasAdType() bool`

HasAdType returns a boolean if a field has been set.

### GetSellingType

`func (o *ApiV1CampaignsGet200ResponseDataInner) GetSellingType() int32`

GetSellingType returns the SellingType field if non-nil, zero value otherwise.

### GetSellingTypeOk

`func (o *ApiV1CampaignsGet200ResponseDataInner) GetSellingTypeOk() (*int32, bool)`

GetSellingTypeOk returns a tuple with the SellingType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSellingType

`func (o *ApiV1CampaignsGet200ResponseDataInner) SetSellingType(v int32)`

SetSellingType sets SellingType field to given value.

### HasSellingType

`func (o *ApiV1CampaignsGet200ResponseDataInner) HasSellingType() bool`

HasSellingType returns a boolean if a field has been set.

### GetIsPaused

`func (o *ApiV1CampaignsGet200ResponseDataInner) GetIsPaused() bool`

GetIsPaused returns the IsPaused field if non-nil, zero value otherwise.

### GetIsPausedOk

`func (o *ApiV1CampaignsGet200ResponseDataInner) GetIsPausedOk() (*bool, bool)`

GetIsPausedOk returns a tuple with the IsPaused field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsPaused

`func (o *ApiV1CampaignsGet200ResponseDataInner) SetIsPaused(v bool)`

SetIsPaused sets IsPaused field to given value.

### HasIsPaused

`func (o *ApiV1CampaignsGet200ResponseDataInner) HasIsPaused() bool`

HasIsPaused returns a boolean if a field has been set.

### GetIsActive

`func (o *ApiV1CampaignsGet200ResponseDataInner) GetIsActive() bool`

GetIsActive returns the IsActive field if non-nil, zero value otherwise.

### GetIsActiveOk

`func (o *ApiV1CampaignsGet200ResponseDataInner) GetIsActiveOk() (*bool, bool)`

GetIsActiveOk returns a tuple with the IsActive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsActive

`func (o *ApiV1CampaignsGet200ResponseDataInner) SetIsActive(v bool)`

SetIsActive sets IsActive field to given value.

### HasIsActive

`func (o *ApiV1CampaignsGet200ResponseDataInner) HasIsActive() bool`

HasIsActive returns a boolean if a field has been set.

### GetIsDeleted

`func (o *ApiV1CampaignsGet200ResponseDataInner) GetIsDeleted() bool`

GetIsDeleted returns the IsDeleted field if non-nil, zero value otherwise.

### GetIsDeletedOk

`func (o *ApiV1CampaignsGet200ResponseDataInner) GetIsDeletedOk() (*bool, bool)`

GetIsDeletedOk returns a tuple with the IsDeleted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDeleted

`func (o *ApiV1CampaignsGet200ResponseDataInner) SetIsDeleted(v bool)`

SetIsDeleted sets IsDeleted field to given value.

### HasIsDeleted

`func (o *ApiV1CampaignsGet200ResponseDataInner) HasIsDeleted() bool`

HasIsDeleted returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


