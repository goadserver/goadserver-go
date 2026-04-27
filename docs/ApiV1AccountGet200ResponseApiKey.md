# ApiV1AccountGet200ResponseApiKey

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **int32** |  | [optional] 
**Scopes** | Pointer to **[]string** |  | [optional] 
**ResourceFilter** | Pointer to [**ResourceFilter**](ResourceFilter.md) |  | [optional] 

## Methods

### NewApiV1AccountGet200ResponseApiKey

`func NewApiV1AccountGet200ResponseApiKey() *ApiV1AccountGet200ResponseApiKey`

NewApiV1AccountGet200ResponseApiKey instantiates a new ApiV1AccountGet200ResponseApiKey object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiV1AccountGet200ResponseApiKeyWithDefaults

`func NewApiV1AccountGet200ResponseApiKeyWithDefaults() *ApiV1AccountGet200ResponseApiKey`

NewApiV1AccountGet200ResponseApiKeyWithDefaults instantiates a new ApiV1AccountGet200ResponseApiKey object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ApiV1AccountGet200ResponseApiKey) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ApiV1AccountGet200ResponseApiKey) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ApiV1AccountGet200ResponseApiKey) SetId(v int32)`

SetId sets Id field to given value.

### HasId

`func (o *ApiV1AccountGet200ResponseApiKey) HasId() bool`

HasId returns a boolean if a field has been set.

### GetScopes

`func (o *ApiV1AccountGet200ResponseApiKey) GetScopes() []string`

GetScopes returns the Scopes field if non-nil, zero value otherwise.

### GetScopesOk

`func (o *ApiV1AccountGet200ResponseApiKey) GetScopesOk() (*[]string, bool)`

GetScopesOk returns a tuple with the Scopes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScopes

`func (o *ApiV1AccountGet200ResponseApiKey) SetScopes(v []string)`

SetScopes sets Scopes field to given value.

### HasScopes

`func (o *ApiV1AccountGet200ResponseApiKey) HasScopes() bool`

HasScopes returns a boolean if a field has been set.

### GetResourceFilter

`func (o *ApiV1AccountGet200ResponseApiKey) GetResourceFilter() ResourceFilter`

GetResourceFilter returns the ResourceFilter field if non-nil, zero value otherwise.

### GetResourceFilterOk

`func (o *ApiV1AccountGet200ResponseApiKey) GetResourceFilterOk() (*ResourceFilter, bool)`

GetResourceFilterOk returns a tuple with the ResourceFilter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResourceFilter

`func (o *ApiV1AccountGet200ResponseApiKey) SetResourceFilter(v ResourceFilter)`

SetResourceFilter sets ResourceFilter field to given value.

### HasResourceFilter

`func (o *ApiV1AccountGet200ResponseApiKey) HasResourceFilter() bool`

HasResourceFilter returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


