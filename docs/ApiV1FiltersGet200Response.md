# ApiV1FiltersGet200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | Pointer to [**[]FilterSummary**](FilterSummary.md) |  | [optional] 
**TotalRows** | Pointer to **int32** |  | [optional] 

## Methods

### NewApiV1FiltersGet200Response

`func NewApiV1FiltersGet200Response() *ApiV1FiltersGet200Response`

NewApiV1FiltersGet200Response instantiates a new ApiV1FiltersGet200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiV1FiltersGet200ResponseWithDefaults

`func NewApiV1FiltersGet200ResponseWithDefaults() *ApiV1FiltersGet200Response`

NewApiV1FiltersGet200ResponseWithDefaults instantiates a new ApiV1FiltersGet200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *ApiV1FiltersGet200Response) GetData() []FilterSummary`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ApiV1FiltersGet200Response) GetDataOk() (*[]FilterSummary, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ApiV1FiltersGet200Response) SetData(v []FilterSummary)`

SetData sets Data field to given value.

### HasData

`func (o *ApiV1FiltersGet200Response) HasData() bool`

HasData returns a boolean if a field has been set.

### GetTotalRows

`func (o *ApiV1FiltersGet200Response) GetTotalRows() int32`

GetTotalRows returns the TotalRows field if non-nil, zero value otherwise.

### GetTotalRowsOk

`func (o *ApiV1FiltersGet200Response) GetTotalRowsOk() (*int32, bool)`

GetTotalRowsOk returns a tuple with the TotalRows field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalRows

`func (o *ApiV1FiltersGet200Response) SetTotalRows(v int32)`

SetTotalRows sets TotalRows field to given value.

### HasTotalRows

`func (o *ApiV1FiltersGet200Response) HasTotalRows() bool`

HasTotalRows returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


