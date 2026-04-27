# ApiV1FundsGet200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Currency** | Pointer to **string** |  | [optional] 
**Balance** | Pointer to **float32** |  | [optional] 
**Pending** | Pointer to **float32** |  | [optional] 
**PendingCount** | Pointer to **int32** |  | [optional] 
**MinBalance** | Pointer to **float32** |  | [optional] 
**LowBalance** | Pointer to **bool** |  | [optional] 
**LastDeposit** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewApiV1FundsGet200Response

`func NewApiV1FundsGet200Response() *ApiV1FundsGet200Response`

NewApiV1FundsGet200Response instantiates a new ApiV1FundsGet200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiV1FundsGet200ResponseWithDefaults

`func NewApiV1FundsGet200ResponseWithDefaults() *ApiV1FundsGet200Response`

NewApiV1FundsGet200ResponseWithDefaults instantiates a new ApiV1FundsGet200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCurrency

`func (o *ApiV1FundsGet200Response) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *ApiV1FundsGet200Response) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *ApiV1FundsGet200Response) SetCurrency(v string)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *ApiV1FundsGet200Response) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.

### GetBalance

`func (o *ApiV1FundsGet200Response) GetBalance() float32`

GetBalance returns the Balance field if non-nil, zero value otherwise.

### GetBalanceOk

`func (o *ApiV1FundsGet200Response) GetBalanceOk() (*float32, bool)`

GetBalanceOk returns a tuple with the Balance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBalance

`func (o *ApiV1FundsGet200Response) SetBalance(v float32)`

SetBalance sets Balance field to given value.

### HasBalance

`func (o *ApiV1FundsGet200Response) HasBalance() bool`

HasBalance returns a boolean if a field has been set.

### GetPending

`func (o *ApiV1FundsGet200Response) GetPending() float32`

GetPending returns the Pending field if non-nil, zero value otherwise.

### GetPendingOk

`func (o *ApiV1FundsGet200Response) GetPendingOk() (*float32, bool)`

GetPendingOk returns a tuple with the Pending field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPending

`func (o *ApiV1FundsGet200Response) SetPending(v float32)`

SetPending sets Pending field to given value.

### HasPending

`func (o *ApiV1FundsGet200Response) HasPending() bool`

HasPending returns a boolean if a field has been set.

### GetPendingCount

`func (o *ApiV1FundsGet200Response) GetPendingCount() int32`

GetPendingCount returns the PendingCount field if non-nil, zero value otherwise.

### GetPendingCountOk

`func (o *ApiV1FundsGet200Response) GetPendingCountOk() (*int32, bool)`

GetPendingCountOk returns a tuple with the PendingCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPendingCount

`func (o *ApiV1FundsGet200Response) SetPendingCount(v int32)`

SetPendingCount sets PendingCount field to given value.

### HasPendingCount

`func (o *ApiV1FundsGet200Response) HasPendingCount() bool`

HasPendingCount returns a boolean if a field has been set.

### GetMinBalance

`func (o *ApiV1FundsGet200Response) GetMinBalance() float32`

GetMinBalance returns the MinBalance field if non-nil, zero value otherwise.

### GetMinBalanceOk

`func (o *ApiV1FundsGet200Response) GetMinBalanceOk() (*float32, bool)`

GetMinBalanceOk returns a tuple with the MinBalance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinBalance

`func (o *ApiV1FundsGet200Response) SetMinBalance(v float32)`

SetMinBalance sets MinBalance field to given value.

### HasMinBalance

`func (o *ApiV1FundsGet200Response) HasMinBalance() bool`

HasMinBalance returns a boolean if a field has been set.

### GetLowBalance

`func (o *ApiV1FundsGet200Response) GetLowBalance() bool`

GetLowBalance returns the LowBalance field if non-nil, zero value otherwise.

### GetLowBalanceOk

`func (o *ApiV1FundsGet200Response) GetLowBalanceOk() (*bool, bool)`

GetLowBalanceOk returns a tuple with the LowBalance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLowBalance

`func (o *ApiV1FundsGet200Response) SetLowBalance(v bool)`

SetLowBalance sets LowBalance field to given value.

### HasLowBalance

`func (o *ApiV1FundsGet200Response) HasLowBalance() bool`

HasLowBalance returns a boolean if a field has been set.

### GetLastDeposit

`func (o *ApiV1FundsGet200Response) GetLastDeposit() time.Time`

GetLastDeposit returns the LastDeposit field if non-nil, zero value otherwise.

### GetLastDepositOk

`func (o *ApiV1FundsGet200Response) GetLastDepositOk() (*time.Time, bool)`

GetLastDepositOk returns a tuple with the LastDeposit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastDeposit

`func (o *ApiV1FundsGet200Response) SetLastDeposit(v time.Time)`

SetLastDeposit sets LastDeposit field to given value.

### HasLastDeposit

`func (o *ApiV1FundsGet200Response) HasLastDeposit() bool`

HasLastDeposit returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


