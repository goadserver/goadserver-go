# FilterDetail

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | Pointer to **string** |  | [optional] 
**Id** | Pointer to **int32** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**IsActive** | Pointer to **bool** |  | [optional] 
**AdType** | Pointer to **int32** | 0 &#x3D; applies to all ad types, otherwise the adtypeid this filter targets. | [optional] 
**ItemCount** | Pointer to **int32** | Number of items (domains/ISPs/etc.) currently in the filter. | [optional] 
**Items** | Pointer to **[]string** | Domain IDs / adzone IDs / ISP IDs / SubID strings — depends on filter type. | [optional] 
**CampaignIds** | Pointer to **[]string** | Campaigns this filter applies to. Empty &#x3D; applies to all campaigns. (Exclusion filters only.) | [optional] 
**Ranges** | Pointer to [**[]FilterDetailAllOfRanges**](FilterDetailAllOfRanges.md) | IP CIDR ranges with their captured IP counts. (&#x60;type&#x3D;ip&#x60; only.) | [optional] 

## Methods

### NewFilterDetail

`func NewFilterDetail() *FilterDetail`

NewFilterDetail instantiates a new FilterDetail object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFilterDetailWithDefaults

`func NewFilterDetailWithDefaults() *FilterDetail`

NewFilterDetailWithDefaults instantiates a new FilterDetail object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *FilterDetail) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *FilterDetail) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *FilterDetail) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *FilterDetail) HasType() bool`

HasType returns a boolean if a field has been set.

### GetId

`func (o *FilterDetail) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *FilterDetail) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *FilterDetail) SetId(v int32)`

SetId sets Id field to given value.

### HasId

`func (o *FilterDetail) HasId() bool`

HasId returns a boolean if a field has been set.

### GetName

`func (o *FilterDetail) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *FilterDetail) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *FilterDetail) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *FilterDetail) HasName() bool`

HasName returns a boolean if a field has been set.

### GetIsActive

`func (o *FilterDetail) GetIsActive() bool`

GetIsActive returns the IsActive field if non-nil, zero value otherwise.

### GetIsActiveOk

`func (o *FilterDetail) GetIsActiveOk() (*bool, bool)`

GetIsActiveOk returns a tuple with the IsActive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsActive

`func (o *FilterDetail) SetIsActive(v bool)`

SetIsActive sets IsActive field to given value.

### HasIsActive

`func (o *FilterDetail) HasIsActive() bool`

HasIsActive returns a boolean if a field has been set.

### GetAdType

`func (o *FilterDetail) GetAdType() int32`

GetAdType returns the AdType field if non-nil, zero value otherwise.

### GetAdTypeOk

`func (o *FilterDetail) GetAdTypeOk() (*int32, bool)`

GetAdTypeOk returns a tuple with the AdType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdType

`func (o *FilterDetail) SetAdType(v int32)`

SetAdType sets AdType field to given value.

### HasAdType

`func (o *FilterDetail) HasAdType() bool`

HasAdType returns a boolean if a field has been set.

### GetItemCount

`func (o *FilterDetail) GetItemCount() int32`

GetItemCount returns the ItemCount field if non-nil, zero value otherwise.

### GetItemCountOk

`func (o *FilterDetail) GetItemCountOk() (*int32, bool)`

GetItemCountOk returns a tuple with the ItemCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItemCount

`func (o *FilterDetail) SetItemCount(v int32)`

SetItemCount sets ItemCount field to given value.

### HasItemCount

`func (o *FilterDetail) HasItemCount() bool`

HasItemCount returns a boolean if a field has been set.

### GetItems

`func (o *FilterDetail) GetItems() []string`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *FilterDetail) GetItemsOk() (*[]string, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *FilterDetail) SetItems(v []string)`

SetItems sets Items field to given value.

### HasItems

`func (o *FilterDetail) HasItems() bool`

HasItems returns a boolean if a field has been set.

### GetCampaignIds

`func (o *FilterDetail) GetCampaignIds() []string`

GetCampaignIds returns the CampaignIds field if non-nil, zero value otherwise.

### GetCampaignIdsOk

`func (o *FilterDetail) GetCampaignIdsOk() (*[]string, bool)`

GetCampaignIdsOk returns a tuple with the CampaignIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCampaignIds

`func (o *FilterDetail) SetCampaignIds(v []string)`

SetCampaignIds sets CampaignIds field to given value.

### HasCampaignIds

`func (o *FilterDetail) HasCampaignIds() bool`

HasCampaignIds returns a boolean if a field has been set.

### GetRanges

`func (o *FilterDetail) GetRanges() []FilterDetailAllOfRanges`

GetRanges returns the Ranges field if non-nil, zero value otherwise.

### GetRangesOk

`func (o *FilterDetail) GetRangesOk() (*[]FilterDetailAllOfRanges, bool)`

GetRangesOk returns a tuple with the Ranges field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRanges

`func (o *FilterDetail) SetRanges(v []FilterDetailAllOfRanges)`

SetRanges sets Ranges field to given value.

### HasRanges

`func (o *FilterDetail) HasRanges() bool`

HasRanges returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


