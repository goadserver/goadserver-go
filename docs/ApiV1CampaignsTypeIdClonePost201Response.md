# ApiV1CampaignsTypeIdClonePost201Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **int32** | The cloned campaign&#39;s id. | [optional] 
**ClonedFrom** | Pointer to **int32** | The source campaign&#39;s id. | [optional] 
**IsActive** | Pointer to **bool** | Always false — the clone lands paused. | [optional] 

## Methods

### NewApiV1CampaignsTypeIdClonePost201Response

`func NewApiV1CampaignsTypeIdClonePost201Response() *ApiV1CampaignsTypeIdClonePost201Response`

NewApiV1CampaignsTypeIdClonePost201Response instantiates a new ApiV1CampaignsTypeIdClonePost201Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiV1CampaignsTypeIdClonePost201ResponseWithDefaults

`func NewApiV1CampaignsTypeIdClonePost201ResponseWithDefaults() *ApiV1CampaignsTypeIdClonePost201Response`

NewApiV1CampaignsTypeIdClonePost201ResponseWithDefaults instantiates a new ApiV1CampaignsTypeIdClonePost201Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ApiV1CampaignsTypeIdClonePost201Response) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ApiV1CampaignsTypeIdClonePost201Response) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ApiV1CampaignsTypeIdClonePost201Response) SetId(v int32)`

SetId sets Id field to given value.

### HasId

`func (o *ApiV1CampaignsTypeIdClonePost201Response) HasId() bool`

HasId returns a boolean if a field has been set.

### GetClonedFrom

`func (o *ApiV1CampaignsTypeIdClonePost201Response) GetClonedFrom() int32`

GetClonedFrom returns the ClonedFrom field if non-nil, zero value otherwise.

### GetClonedFromOk

`func (o *ApiV1CampaignsTypeIdClonePost201Response) GetClonedFromOk() (*int32, bool)`

GetClonedFromOk returns a tuple with the ClonedFrom field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClonedFrom

`func (o *ApiV1CampaignsTypeIdClonePost201Response) SetClonedFrom(v int32)`

SetClonedFrom sets ClonedFrom field to given value.

### HasClonedFrom

`func (o *ApiV1CampaignsTypeIdClonePost201Response) HasClonedFrom() bool`

HasClonedFrom returns a boolean if a field has been set.

### GetIsActive

`func (o *ApiV1CampaignsTypeIdClonePost201Response) GetIsActive() bool`

GetIsActive returns the IsActive field if non-nil, zero value otherwise.

### GetIsActiveOk

`func (o *ApiV1CampaignsTypeIdClonePost201Response) GetIsActiveOk() (*bool, bool)`

GetIsActiveOk returns a tuple with the IsActive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsActive

`func (o *ApiV1CampaignsTypeIdClonePost201Response) SetIsActive(v bool)`

SetIsActive sets IsActive field to given value.

### HasIsActive

`func (o *ApiV1CampaignsTypeIdClonePost201Response) HasIsActive() bool`

HasIsActive returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


