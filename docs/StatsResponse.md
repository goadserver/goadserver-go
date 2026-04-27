# StatsResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**From** | Pointer to **string** |  | [optional] 
**To** | Pointer to **string** |  | [optional] 
**GroupBy** | Pointer to **[]string** |  | [optional] 
**Totals** | Pointer to **map[string]float32** |  | [optional] 
**Rows** | Pointer to **[]map[string]interface{}** |  | [optional] 
**Page** | Pointer to **int32** |  | [optional] 
**PerPage** | Pointer to **int32** |  | [optional] 
**TotalRows** | Pointer to **int32** |  | [optional] 

## Methods

### NewStatsResponse

`func NewStatsResponse() *StatsResponse`

NewStatsResponse instantiates a new StatsResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStatsResponseWithDefaults

`func NewStatsResponseWithDefaults() *StatsResponse`

NewStatsResponseWithDefaults instantiates a new StatsResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFrom

`func (o *StatsResponse) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *StatsResponse) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *StatsResponse) SetFrom(v string)`

SetFrom sets From field to given value.

### HasFrom

`func (o *StatsResponse) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetTo

`func (o *StatsResponse) GetTo() string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *StatsResponse) GetToOk() (*string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *StatsResponse) SetTo(v string)`

SetTo sets To field to given value.

### HasTo

`func (o *StatsResponse) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetGroupBy

`func (o *StatsResponse) GetGroupBy() []string`

GetGroupBy returns the GroupBy field if non-nil, zero value otherwise.

### GetGroupByOk

`func (o *StatsResponse) GetGroupByOk() (*[]string, bool)`

GetGroupByOk returns a tuple with the GroupBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGroupBy

`func (o *StatsResponse) SetGroupBy(v []string)`

SetGroupBy sets GroupBy field to given value.

### HasGroupBy

`func (o *StatsResponse) HasGroupBy() bool`

HasGroupBy returns a boolean if a field has been set.

### GetTotals

`func (o *StatsResponse) GetTotals() map[string]float32`

GetTotals returns the Totals field if non-nil, zero value otherwise.

### GetTotalsOk

`func (o *StatsResponse) GetTotalsOk() (*map[string]float32, bool)`

GetTotalsOk returns a tuple with the Totals field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotals

`func (o *StatsResponse) SetTotals(v map[string]float32)`

SetTotals sets Totals field to given value.

### HasTotals

`func (o *StatsResponse) HasTotals() bool`

HasTotals returns a boolean if a field has been set.

### GetRows

`func (o *StatsResponse) GetRows() []map[string]interface{}`

GetRows returns the Rows field if non-nil, zero value otherwise.

### GetRowsOk

`func (o *StatsResponse) GetRowsOk() (*[]map[string]interface{}, bool)`

GetRowsOk returns a tuple with the Rows field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRows

`func (o *StatsResponse) SetRows(v []map[string]interface{})`

SetRows sets Rows field to given value.

### HasRows

`func (o *StatsResponse) HasRows() bool`

HasRows returns a boolean if a field has been set.

### GetPage

`func (o *StatsResponse) GetPage() int32`

GetPage returns the Page field if non-nil, zero value otherwise.

### GetPageOk

`func (o *StatsResponse) GetPageOk() (*int32, bool)`

GetPageOk returns a tuple with the Page field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPage

`func (o *StatsResponse) SetPage(v int32)`

SetPage sets Page field to given value.

### HasPage

`func (o *StatsResponse) HasPage() bool`

HasPage returns a boolean if a field has been set.

### GetPerPage

`func (o *StatsResponse) GetPerPage() int32`

GetPerPage returns the PerPage field if non-nil, zero value otherwise.

### GetPerPageOk

`func (o *StatsResponse) GetPerPageOk() (*int32, bool)`

GetPerPageOk returns a tuple with the PerPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPerPage

`func (o *StatsResponse) SetPerPage(v int32)`

SetPerPage sets PerPage field to given value.

### HasPerPage

`func (o *StatsResponse) HasPerPage() bool`

HasPerPage returns a boolean if a field has been set.

### GetTotalRows

`func (o *StatsResponse) GetTotalRows() int32`

GetTotalRows returns the TotalRows field if non-nil, zero value otherwise.

### GetTotalRowsOk

`func (o *StatsResponse) GetTotalRowsOk() (*int32, bool)`

GetTotalRowsOk returns a tuple with the TotalRows field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalRows

`func (o *StatsResponse) SetTotalRows(v int32)`

SetTotalRows sets TotalRows field to given value.

### HasTotalRows

`func (o *StatsResponse) HasTotalRows() bool`

HasTotalRows returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


