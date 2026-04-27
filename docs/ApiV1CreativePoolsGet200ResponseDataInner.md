# ApiV1CreativePoolsGet200ResponseDataInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **int32** |  | [optional] 
**Title** | Pointer to **string** |  | [optional] 
**Type** | Pointer to **string** |  | [optional] 
**SortType** | Pointer to **string** |  | [optional] 
**ConvType** | Pointer to **int32** |  | [optional] 
**Tags** | Pointer to **string** | CSV of tag ids. | [optional] 
**Tagids** | Pointer to **[]string** |  | [optional] 
**ItemsCount** | Pointer to **int32** |  | [optional] 
**TotalSizes** | Pointer to **int32** |  | [optional] 

## Methods

### NewApiV1CreativePoolsGet200ResponseDataInner

`func NewApiV1CreativePoolsGet200ResponseDataInner() *ApiV1CreativePoolsGet200ResponseDataInner`

NewApiV1CreativePoolsGet200ResponseDataInner instantiates a new ApiV1CreativePoolsGet200ResponseDataInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiV1CreativePoolsGet200ResponseDataInnerWithDefaults

`func NewApiV1CreativePoolsGet200ResponseDataInnerWithDefaults() *ApiV1CreativePoolsGet200ResponseDataInner`

NewApiV1CreativePoolsGet200ResponseDataInnerWithDefaults instantiates a new ApiV1CreativePoolsGet200ResponseDataInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) SetId(v int32)`

SetId sets Id field to given value.

### HasId

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) HasId() bool`

HasId returns a boolean if a field has been set.

### GetTitle

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### GetType

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) HasType() bool`

HasType returns a boolean if a field has been set.

### GetSortType

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) GetSortType() string`

GetSortType returns the SortType field if non-nil, zero value otherwise.

### GetSortTypeOk

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) GetSortTypeOk() (*string, bool)`

GetSortTypeOk returns a tuple with the SortType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortType

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) SetSortType(v string)`

SetSortType sets SortType field to given value.

### HasSortType

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) HasSortType() bool`

HasSortType returns a boolean if a field has been set.

### GetConvType

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) GetConvType() int32`

GetConvType returns the ConvType field if non-nil, zero value otherwise.

### GetConvTypeOk

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) GetConvTypeOk() (*int32, bool)`

GetConvTypeOk returns a tuple with the ConvType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConvType

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) SetConvType(v int32)`

SetConvType sets ConvType field to given value.

### HasConvType

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) HasConvType() bool`

HasConvType returns a boolean if a field has been set.

### GetTags

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) GetTags() string`

GetTags returns the Tags field if non-nil, zero value otherwise.

### GetTagsOk

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) GetTagsOk() (*string, bool)`

GetTagsOk returns a tuple with the Tags field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTags

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) SetTags(v string)`

SetTags sets Tags field to given value.

### HasTags

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) HasTags() bool`

HasTags returns a boolean if a field has been set.

### GetTagids

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) GetTagids() []string`

GetTagids returns the Tagids field if non-nil, zero value otherwise.

### GetTagidsOk

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) GetTagidsOk() (*[]string, bool)`

GetTagidsOk returns a tuple with the Tagids field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTagids

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) SetTagids(v []string)`

SetTagids sets Tagids field to given value.

### HasTagids

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) HasTagids() bool`

HasTagids returns a boolean if a field has been set.

### GetItemsCount

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) GetItemsCount() int32`

GetItemsCount returns the ItemsCount field if non-nil, zero value otherwise.

### GetItemsCountOk

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) GetItemsCountOk() (*int32, bool)`

GetItemsCountOk returns a tuple with the ItemsCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItemsCount

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) SetItemsCount(v int32)`

SetItemsCount sets ItemsCount field to given value.

### HasItemsCount

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) HasItemsCount() bool`

HasItemsCount returns a boolean if a field has been set.

### GetTotalSizes

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) GetTotalSizes() int32`

GetTotalSizes returns the TotalSizes field if non-nil, zero value otherwise.

### GetTotalSizesOk

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) GetTotalSizesOk() (*int32, bool)`

GetTotalSizesOk returns a tuple with the TotalSizes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalSizes

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) SetTotalSizes(v int32)`

SetTotalSizes sets TotalSizes field to given value.

### HasTotalSizes

`func (o *ApiV1CreativePoolsGet200ResponseDataInner) HasTotalSizes() bool`

HasTotalSizes returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


