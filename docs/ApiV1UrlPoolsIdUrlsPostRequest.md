# ApiV1UrlPoolsIdUrlsPostRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Url** | **string** |  | 
**Title** | Pointer to **string** |  | [optional] 
**Weight** | Pointer to **int32** |  | [optional] [default to 1]
**Properties** | Pointer to **string** |  | [optional] 

## Methods

### NewApiV1UrlPoolsIdUrlsPostRequest

`func NewApiV1UrlPoolsIdUrlsPostRequest(url string, ) *ApiV1UrlPoolsIdUrlsPostRequest`

NewApiV1UrlPoolsIdUrlsPostRequest instantiates a new ApiV1UrlPoolsIdUrlsPostRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiV1UrlPoolsIdUrlsPostRequestWithDefaults

`func NewApiV1UrlPoolsIdUrlsPostRequestWithDefaults() *ApiV1UrlPoolsIdUrlsPostRequest`

NewApiV1UrlPoolsIdUrlsPostRequestWithDefaults instantiates a new ApiV1UrlPoolsIdUrlsPostRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUrl

`func (o *ApiV1UrlPoolsIdUrlsPostRequest) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *ApiV1UrlPoolsIdUrlsPostRequest) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *ApiV1UrlPoolsIdUrlsPostRequest) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetTitle

`func (o *ApiV1UrlPoolsIdUrlsPostRequest) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ApiV1UrlPoolsIdUrlsPostRequest) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ApiV1UrlPoolsIdUrlsPostRequest) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *ApiV1UrlPoolsIdUrlsPostRequest) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### GetWeight

`func (o *ApiV1UrlPoolsIdUrlsPostRequest) GetWeight() int32`

GetWeight returns the Weight field if non-nil, zero value otherwise.

### GetWeightOk

`func (o *ApiV1UrlPoolsIdUrlsPostRequest) GetWeightOk() (*int32, bool)`

GetWeightOk returns a tuple with the Weight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWeight

`func (o *ApiV1UrlPoolsIdUrlsPostRequest) SetWeight(v int32)`

SetWeight sets Weight field to given value.

### HasWeight

`func (o *ApiV1UrlPoolsIdUrlsPostRequest) HasWeight() bool`

HasWeight returns a boolean if a field has been set.

### GetProperties

`func (o *ApiV1UrlPoolsIdUrlsPostRequest) GetProperties() string`

GetProperties returns the Properties field if non-nil, zero value otherwise.

### GetPropertiesOk

`func (o *ApiV1UrlPoolsIdUrlsPostRequest) GetPropertiesOk() (*string, bool)`

GetPropertiesOk returns a tuple with the Properties field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProperties

`func (o *ApiV1UrlPoolsIdUrlsPostRequest) SetProperties(v string)`

SetProperties sets Properties field to given value.

### HasProperties

`func (o *ApiV1UrlPoolsIdUrlsPostRequest) HasProperties() bool`

HasProperties returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


