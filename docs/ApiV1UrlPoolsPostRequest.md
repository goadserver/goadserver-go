# ApiV1UrlPoolsPostRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Title** | **string** |  | 
**SortType** | Pointer to **string** |  | [optional] [default to "rnd"]
**ConvType** | Pointer to **int32** |  | [optional] 
**Tags** | Pointer to **string** |  | [optional] 

## Methods

### NewApiV1UrlPoolsPostRequest

`func NewApiV1UrlPoolsPostRequest(title string, ) *ApiV1UrlPoolsPostRequest`

NewApiV1UrlPoolsPostRequest instantiates a new ApiV1UrlPoolsPostRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiV1UrlPoolsPostRequestWithDefaults

`func NewApiV1UrlPoolsPostRequestWithDefaults() *ApiV1UrlPoolsPostRequest`

NewApiV1UrlPoolsPostRequestWithDefaults instantiates a new ApiV1UrlPoolsPostRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTitle

`func (o *ApiV1UrlPoolsPostRequest) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ApiV1UrlPoolsPostRequest) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ApiV1UrlPoolsPostRequest) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetSortType

`func (o *ApiV1UrlPoolsPostRequest) GetSortType() string`

GetSortType returns the SortType field if non-nil, zero value otherwise.

### GetSortTypeOk

`func (o *ApiV1UrlPoolsPostRequest) GetSortTypeOk() (*string, bool)`

GetSortTypeOk returns a tuple with the SortType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortType

`func (o *ApiV1UrlPoolsPostRequest) SetSortType(v string)`

SetSortType sets SortType field to given value.

### HasSortType

`func (o *ApiV1UrlPoolsPostRequest) HasSortType() bool`

HasSortType returns a boolean if a field has been set.

### GetConvType

`func (o *ApiV1UrlPoolsPostRequest) GetConvType() int32`

GetConvType returns the ConvType field if non-nil, zero value otherwise.

### GetConvTypeOk

`func (o *ApiV1UrlPoolsPostRequest) GetConvTypeOk() (*int32, bool)`

GetConvTypeOk returns a tuple with the ConvType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConvType

`func (o *ApiV1UrlPoolsPostRequest) SetConvType(v int32)`

SetConvType sets ConvType field to given value.

### HasConvType

`func (o *ApiV1UrlPoolsPostRequest) HasConvType() bool`

HasConvType returns a boolean if a field has been set.

### GetTags

`func (o *ApiV1UrlPoolsPostRequest) GetTags() string`

GetTags returns the Tags field if non-nil, zero value otherwise.

### GetTagsOk

`func (o *ApiV1UrlPoolsPostRequest) GetTagsOk() (*string, bool)`

GetTagsOk returns a tuple with the Tags field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTags

`func (o *ApiV1UrlPoolsPostRequest) SetTags(v string)`

SetTags sets Tags field to given value.

### HasTags

`func (o *ApiV1UrlPoolsPostRequest) HasTags() bool`

HasTags returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


