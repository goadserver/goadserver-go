# ApiV1CreativePoolsPostRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Title** | **string** |  | 
**Type** | Pointer to **string** |  | [optional] [default to "banner"]
**Tags** | Pointer to **string** | CSV of tag ids. | [optional] 

## Methods

### NewApiV1CreativePoolsPostRequest

`func NewApiV1CreativePoolsPostRequest(title string, ) *ApiV1CreativePoolsPostRequest`

NewApiV1CreativePoolsPostRequest instantiates a new ApiV1CreativePoolsPostRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiV1CreativePoolsPostRequestWithDefaults

`func NewApiV1CreativePoolsPostRequestWithDefaults() *ApiV1CreativePoolsPostRequest`

NewApiV1CreativePoolsPostRequestWithDefaults instantiates a new ApiV1CreativePoolsPostRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTitle

`func (o *ApiV1CreativePoolsPostRequest) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ApiV1CreativePoolsPostRequest) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ApiV1CreativePoolsPostRequest) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetType

`func (o *ApiV1CreativePoolsPostRequest) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ApiV1CreativePoolsPostRequest) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ApiV1CreativePoolsPostRequest) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *ApiV1CreativePoolsPostRequest) HasType() bool`

HasType returns a boolean if a field has been set.

### GetTags

`func (o *ApiV1CreativePoolsPostRequest) GetTags() string`

GetTags returns the Tags field if non-nil, zero value otherwise.

### GetTagsOk

`func (o *ApiV1CreativePoolsPostRequest) GetTagsOk() (*string, bool)`

GetTagsOk returns a tuple with the Tags field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTags

`func (o *ApiV1CreativePoolsPostRequest) SetTags(v string)`

SetTags sets Tags field to given value.

### HasTags

`func (o *ApiV1CreativePoolsPostRequest) HasTags() bool`

HasTags returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


