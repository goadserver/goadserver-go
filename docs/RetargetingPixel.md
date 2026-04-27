# RetargetingPixel

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **int32** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**IsActive** | Pointer to **bool** |  | [optional] 
**Visitors** | Pointer to **int32** | Captured visitor count from ClickHouse. | [optional] 

## Methods

### NewRetargetingPixel

`func NewRetargetingPixel() *RetargetingPixel`

NewRetargetingPixel instantiates a new RetargetingPixel object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRetargetingPixelWithDefaults

`func NewRetargetingPixelWithDefaults() *RetargetingPixel`

NewRetargetingPixelWithDefaults instantiates a new RetargetingPixel object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *RetargetingPixel) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *RetargetingPixel) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *RetargetingPixel) SetId(v int32)`

SetId sets Id field to given value.

### HasId

`func (o *RetargetingPixel) HasId() bool`

HasId returns a boolean if a field has been set.

### GetName

`func (o *RetargetingPixel) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *RetargetingPixel) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *RetargetingPixel) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *RetargetingPixel) HasName() bool`

HasName returns a boolean if a field has been set.

### GetIsActive

`func (o *RetargetingPixel) GetIsActive() bool`

GetIsActive returns the IsActive field if non-nil, zero value otherwise.

### GetIsActiveOk

`func (o *RetargetingPixel) GetIsActiveOk() (*bool, bool)`

GetIsActiveOk returns a tuple with the IsActive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsActive

`func (o *RetargetingPixel) SetIsActive(v bool)`

SetIsActive sets IsActive field to given value.

### HasIsActive

`func (o *RetargetingPixel) HasIsActive() bool`

HasIsActive returns a boolean if a field has been set.

### GetVisitors

`func (o *RetargetingPixel) GetVisitors() int32`

GetVisitors returns the Visitors field if non-nil, zero value otherwise.

### GetVisitorsOk

`func (o *RetargetingPixel) GetVisitorsOk() (*int32, bool)`

GetVisitorsOk returns a tuple with the Visitors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVisitors

`func (o *RetargetingPixel) SetVisitors(v int32)`

SetVisitors sets Visitors field to given value.

### HasVisitors

`func (o *RetargetingPixel) HasVisitors() bool`

HasVisitors returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


