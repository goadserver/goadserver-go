# FilterSummary

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | Pointer to **string** |  | [optional] 
**Id** | Pointer to **int32** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**IsActive** | Pointer to **bool** |  | [optional] 
**AdType** | Pointer to **int32** | 0 &#x3D; applies to all ad types, otherwise the adtypeid this filter targets. | [optional] 
**ItemCount** | Pointer to **int32** | Number of items (domains/ISPs/etc.) currently in the filter. | [optional] 

## Methods

### NewFilterSummary

`func NewFilterSummary() *FilterSummary`

NewFilterSummary instantiates a new FilterSummary object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFilterSummaryWithDefaults

`func NewFilterSummaryWithDefaults() *FilterSummary`

NewFilterSummaryWithDefaults instantiates a new FilterSummary object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *FilterSummary) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *FilterSummary) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *FilterSummary) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *FilterSummary) HasType() bool`

HasType returns a boolean if a field has been set.

### GetId

`func (o *FilterSummary) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *FilterSummary) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *FilterSummary) SetId(v int32)`

SetId sets Id field to given value.

### HasId

`func (o *FilterSummary) HasId() bool`

HasId returns a boolean if a field has been set.

### GetName

`func (o *FilterSummary) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *FilterSummary) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *FilterSummary) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *FilterSummary) HasName() bool`

HasName returns a boolean if a field has been set.

### GetIsActive

`func (o *FilterSummary) GetIsActive() bool`

GetIsActive returns the IsActive field if non-nil, zero value otherwise.

### GetIsActiveOk

`func (o *FilterSummary) GetIsActiveOk() (*bool, bool)`

GetIsActiveOk returns a tuple with the IsActive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsActive

`func (o *FilterSummary) SetIsActive(v bool)`

SetIsActive sets IsActive field to given value.

### HasIsActive

`func (o *FilterSummary) HasIsActive() bool`

HasIsActive returns a boolean if a field has been set.

### GetAdType

`func (o *FilterSummary) GetAdType() int32`

GetAdType returns the AdType field if non-nil, zero value otherwise.

### GetAdTypeOk

`func (o *FilterSummary) GetAdTypeOk() (*int32, bool)`

GetAdTypeOk returns a tuple with the AdType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdType

`func (o *FilterSummary) SetAdType(v int32)`

SetAdType sets AdType field to given value.

### HasAdType

`func (o *FilterSummary) HasAdType() bool`

HasAdType returns a boolean if a field has been set.

### GetItemCount

`func (o *FilterSummary) GetItemCount() int32`

GetItemCount returns the ItemCount field if non-nil, zero value otherwise.

### GetItemCountOk

`func (o *FilterSummary) GetItemCountOk() (*int32, bool)`

GetItemCountOk returns a tuple with the ItemCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItemCount

`func (o *FilterSummary) SetItemCount(v int32)`

SetItemCount sets ItemCount field to given value.

### HasItemCount

`func (o *FilterSummary) HasItemCount() bool`

HasItemCount returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


