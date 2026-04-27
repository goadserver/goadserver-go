# ApiKeyDetails

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **int32** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**Prefix** | Pointer to **string** |  | [optional] 
**Scopes** | Pointer to **[]string** |  | [optional] 
**IpAllowlist** | Pointer to **string** | CSV of IPs/CIDRs, empty &#x3D; any | [optional] 
**RateLimitRpm** | Pointer to **int32** | 0 &#x3D; system default (60) | [optional] 
**ExpiresAt** | Pointer to **time.Time** |  | [optional] 
**LastUsedAt** | Pointer to **time.Time** |  | [optional] 
**LastUsedIp** | Pointer to **string** |  | [optional] 
**CallCount** | Pointer to **int32** |  | [optional] 
**RevokedAt** | Pointer to **time.Time** |  | [optional] 
**CreatedAt** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewApiKeyDetails

`func NewApiKeyDetails() *ApiKeyDetails`

NewApiKeyDetails instantiates a new ApiKeyDetails object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiKeyDetailsWithDefaults

`func NewApiKeyDetailsWithDefaults() *ApiKeyDetails`

NewApiKeyDetailsWithDefaults instantiates a new ApiKeyDetails object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ApiKeyDetails) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ApiKeyDetails) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ApiKeyDetails) SetId(v int32)`

SetId sets Id field to given value.

### HasId

`func (o *ApiKeyDetails) HasId() bool`

HasId returns a boolean if a field has been set.

### GetName

`func (o *ApiKeyDetails) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ApiKeyDetails) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ApiKeyDetails) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ApiKeyDetails) HasName() bool`

HasName returns a boolean if a field has been set.

### GetPrefix

`func (o *ApiKeyDetails) GetPrefix() string`

GetPrefix returns the Prefix field if non-nil, zero value otherwise.

### GetPrefixOk

`func (o *ApiKeyDetails) GetPrefixOk() (*string, bool)`

GetPrefixOk returns a tuple with the Prefix field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrefix

`func (o *ApiKeyDetails) SetPrefix(v string)`

SetPrefix sets Prefix field to given value.

### HasPrefix

`func (o *ApiKeyDetails) HasPrefix() bool`

HasPrefix returns a boolean if a field has been set.

### GetScopes

`func (o *ApiKeyDetails) GetScopes() []string`

GetScopes returns the Scopes field if non-nil, zero value otherwise.

### GetScopesOk

`func (o *ApiKeyDetails) GetScopesOk() (*[]string, bool)`

GetScopesOk returns a tuple with the Scopes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScopes

`func (o *ApiKeyDetails) SetScopes(v []string)`

SetScopes sets Scopes field to given value.

### HasScopes

`func (o *ApiKeyDetails) HasScopes() bool`

HasScopes returns a boolean if a field has been set.

### GetIpAllowlist

`func (o *ApiKeyDetails) GetIpAllowlist() string`

GetIpAllowlist returns the IpAllowlist field if non-nil, zero value otherwise.

### GetIpAllowlistOk

`func (o *ApiKeyDetails) GetIpAllowlistOk() (*string, bool)`

GetIpAllowlistOk returns a tuple with the IpAllowlist field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIpAllowlist

`func (o *ApiKeyDetails) SetIpAllowlist(v string)`

SetIpAllowlist sets IpAllowlist field to given value.

### HasIpAllowlist

`func (o *ApiKeyDetails) HasIpAllowlist() bool`

HasIpAllowlist returns a boolean if a field has been set.

### GetRateLimitRpm

`func (o *ApiKeyDetails) GetRateLimitRpm() int32`

GetRateLimitRpm returns the RateLimitRpm field if non-nil, zero value otherwise.

### GetRateLimitRpmOk

`func (o *ApiKeyDetails) GetRateLimitRpmOk() (*int32, bool)`

GetRateLimitRpmOk returns a tuple with the RateLimitRpm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRateLimitRpm

`func (o *ApiKeyDetails) SetRateLimitRpm(v int32)`

SetRateLimitRpm sets RateLimitRpm field to given value.

### HasRateLimitRpm

`func (o *ApiKeyDetails) HasRateLimitRpm() bool`

HasRateLimitRpm returns a boolean if a field has been set.

### GetExpiresAt

`func (o *ApiKeyDetails) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *ApiKeyDetails) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *ApiKeyDetails) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.

### HasExpiresAt

`func (o *ApiKeyDetails) HasExpiresAt() bool`

HasExpiresAt returns a boolean if a field has been set.

### GetLastUsedAt

`func (o *ApiKeyDetails) GetLastUsedAt() time.Time`

GetLastUsedAt returns the LastUsedAt field if non-nil, zero value otherwise.

### GetLastUsedAtOk

`func (o *ApiKeyDetails) GetLastUsedAtOk() (*time.Time, bool)`

GetLastUsedAtOk returns a tuple with the LastUsedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastUsedAt

`func (o *ApiKeyDetails) SetLastUsedAt(v time.Time)`

SetLastUsedAt sets LastUsedAt field to given value.

### HasLastUsedAt

`func (o *ApiKeyDetails) HasLastUsedAt() bool`

HasLastUsedAt returns a boolean if a field has been set.

### GetLastUsedIp

`func (o *ApiKeyDetails) GetLastUsedIp() string`

GetLastUsedIp returns the LastUsedIp field if non-nil, zero value otherwise.

### GetLastUsedIpOk

`func (o *ApiKeyDetails) GetLastUsedIpOk() (*string, bool)`

GetLastUsedIpOk returns a tuple with the LastUsedIp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastUsedIp

`func (o *ApiKeyDetails) SetLastUsedIp(v string)`

SetLastUsedIp sets LastUsedIp field to given value.

### HasLastUsedIp

`func (o *ApiKeyDetails) HasLastUsedIp() bool`

HasLastUsedIp returns a boolean if a field has been set.

### GetCallCount

`func (o *ApiKeyDetails) GetCallCount() int32`

GetCallCount returns the CallCount field if non-nil, zero value otherwise.

### GetCallCountOk

`func (o *ApiKeyDetails) GetCallCountOk() (*int32, bool)`

GetCallCountOk returns a tuple with the CallCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCallCount

`func (o *ApiKeyDetails) SetCallCount(v int32)`

SetCallCount sets CallCount field to given value.

### HasCallCount

`func (o *ApiKeyDetails) HasCallCount() bool`

HasCallCount returns a boolean if a field has been set.

### GetRevokedAt

`func (o *ApiKeyDetails) GetRevokedAt() time.Time`

GetRevokedAt returns the RevokedAt field if non-nil, zero value otherwise.

### GetRevokedAtOk

`func (o *ApiKeyDetails) GetRevokedAtOk() (*time.Time, bool)`

GetRevokedAtOk returns a tuple with the RevokedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRevokedAt

`func (o *ApiKeyDetails) SetRevokedAt(v time.Time)`

SetRevokedAt sets RevokedAt field to given value.

### HasRevokedAt

`func (o *ApiKeyDetails) HasRevokedAt() bool`

HasRevokedAt returns a boolean if a field has been set.

### GetCreatedAt

`func (o *ApiKeyDetails) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *ApiKeyDetails) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *ApiKeyDetails) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *ApiKeyDetails) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


