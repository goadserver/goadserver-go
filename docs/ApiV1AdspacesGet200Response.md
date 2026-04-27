# ApiV1AdspacesGet200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | Pointer to [**[]ApiV1AdspacesGet200ResponseDataInner**](ApiV1AdspacesGet200ResponseDataInner.md) |  | [optional] 
**Page** | Pointer to **int32** |  | [optional] 
**PerPage** | Pointer to **int32** |  | [optional] 
**TotalRows** | Pointer to **int32** |  | [optional] 

## Methods

### NewApiV1AdspacesGet200Response

`func NewApiV1AdspacesGet200Response() *ApiV1AdspacesGet200Response`

NewApiV1AdspacesGet200Response instantiates a new ApiV1AdspacesGet200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiV1AdspacesGet200ResponseWithDefaults

`func NewApiV1AdspacesGet200ResponseWithDefaults() *ApiV1AdspacesGet200Response`

NewApiV1AdspacesGet200ResponseWithDefaults instantiates a new ApiV1AdspacesGet200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *ApiV1AdspacesGet200Response) GetData() []ApiV1AdspacesGet200ResponseDataInner`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ApiV1AdspacesGet200Response) GetDataOk() (*[]ApiV1AdspacesGet200ResponseDataInner, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ApiV1AdspacesGet200Response) SetData(v []ApiV1AdspacesGet200ResponseDataInner)`

SetData sets Data field to given value.

### HasData

`func (o *ApiV1AdspacesGet200Response) HasData() bool`

HasData returns a boolean if a field has been set.

### GetPage

`func (o *ApiV1AdspacesGet200Response) GetPage() int32`

GetPage returns the Page field if non-nil, zero value otherwise.

### GetPageOk

`func (o *ApiV1AdspacesGet200Response) GetPageOk() (*int32, bool)`

GetPageOk returns a tuple with the Page field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPage

`func (o *ApiV1AdspacesGet200Response) SetPage(v int32)`

SetPage sets Page field to given value.

### HasPage

`func (o *ApiV1AdspacesGet200Response) HasPage() bool`

HasPage returns a boolean if a field has been set.

### GetPerPage

`func (o *ApiV1AdspacesGet200Response) GetPerPage() int32`

GetPerPage returns the PerPage field if non-nil, zero value otherwise.

### GetPerPageOk

`func (o *ApiV1AdspacesGet200Response) GetPerPageOk() (*int32, bool)`

GetPerPageOk returns a tuple with the PerPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPerPage

`func (o *ApiV1AdspacesGet200Response) SetPerPage(v int32)`

SetPerPage sets PerPage field to given value.

### HasPerPage

`func (o *ApiV1AdspacesGet200Response) HasPerPage() bool`

HasPerPage returns a boolean if a field has been set.

### GetTotalRows

`func (o *ApiV1AdspacesGet200Response) GetTotalRows() int32`

GetTotalRows returns the TotalRows field if non-nil, zero value otherwise.

### GetTotalRowsOk

`func (o *ApiV1AdspacesGet200Response) GetTotalRowsOk() (*int32, bool)`

GetTotalRowsOk returns a tuple with the TotalRows field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalRows

`func (o *ApiV1AdspacesGet200Response) SetTotalRows(v int32)`

SetTotalRows sets TotalRows field to given value.

### HasTotalRows

`func (o *ApiV1AdspacesGet200Response) HasTotalRows() bool`

HasTotalRows returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


