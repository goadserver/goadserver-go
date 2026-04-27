# ApiKeyDetailsCreated

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
**Key** | Pointer to **string** | **Plaintext key — shown ONCE.** Save it now; it cannot be retrieved again. To rotate, create a new key and revoke this one.  | [optional] 
**Message** | Pointer to **string** |  | [optional] 

## Methods

### NewApiKeyDetailsCreated

`func NewApiKeyDetailsCreated() *ApiKeyDetailsCreated`

NewApiKeyDetailsCreated instantiates a new ApiKeyDetailsCreated object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiKeyDetailsCreatedWithDefaults

`func NewApiKeyDetailsCreatedWithDefaults() *ApiKeyDetailsCreated`

NewApiKeyDetailsCreatedWithDefaults instantiates a new ApiKeyDetailsCreated object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ApiKeyDetailsCreated) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ApiKeyDetailsCreated) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ApiKeyDetailsCreated) SetId(v int32)`

SetId sets Id field to given value.

### HasId

`func (o *ApiKeyDetailsCreated) HasId() bool`

HasId returns a boolean if a field has been set.

### GetName

`func (o *ApiKeyDetailsCreated) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ApiKeyDetailsCreated) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ApiKeyDetailsCreated) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ApiKeyDetailsCreated) HasName() bool`

HasName returns a boolean if a field has been set.

### GetPrefix

`func (o *ApiKeyDetailsCreated) GetPrefix() string`

GetPrefix returns the Prefix field if non-nil, zero value otherwise.

### GetPrefixOk

`func (o *ApiKeyDetailsCreated) GetPrefixOk() (*string, bool)`

GetPrefixOk returns a tuple with the Prefix field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrefix

`func (o *ApiKeyDetailsCreated) SetPrefix(v string)`

SetPrefix sets Prefix field to given value.

### HasPrefix

`func (o *ApiKeyDetailsCreated) HasPrefix() bool`

HasPrefix returns a boolean if a field has been set.

### GetScopes

`func (o *ApiKeyDetailsCreated) GetScopes() []string`

GetScopes returns the Scopes field if non-nil, zero value otherwise.

### GetScopesOk

`func (o *ApiKeyDetailsCreated) GetScopesOk() (*[]string, bool)`

GetScopesOk returns a tuple with the Scopes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScopes

`func (o *ApiKeyDetailsCreated) SetScopes(v []string)`

SetScopes sets Scopes field to given value.

### HasScopes

`func (o *ApiKeyDetailsCreated) HasScopes() bool`

HasScopes returns a boolean if a field has been set.

### GetIpAllowlist

`func (o *ApiKeyDetailsCreated) GetIpAllowlist() string`

GetIpAllowlist returns the IpAllowlist field if non-nil, zero value otherwise.

### GetIpAllowlistOk

`func (o *ApiKeyDetailsCreated) GetIpAllowlistOk() (*string, bool)`

GetIpAllowlistOk returns a tuple with the IpAllowlist field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIpAllowlist

`func (o *ApiKeyDetailsCreated) SetIpAllowlist(v string)`

SetIpAllowlist sets IpAllowlist field to given value.

### HasIpAllowlist

`func (o *ApiKeyDetailsCreated) HasIpAllowlist() bool`

HasIpAllowlist returns a boolean if a field has been set.

### GetRateLimitRpm

`func (o *ApiKeyDetailsCreated) GetRateLimitRpm() int32`

GetRateLimitRpm returns the RateLimitRpm field if non-nil, zero value otherwise.

### GetRateLimitRpmOk

`func (o *ApiKeyDetailsCreated) GetRateLimitRpmOk() (*int32, bool)`

GetRateLimitRpmOk returns a tuple with the RateLimitRpm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRateLimitRpm

`func (o *ApiKeyDetailsCreated) SetRateLimitRpm(v int32)`

SetRateLimitRpm sets RateLimitRpm field to given value.

### HasRateLimitRpm

`func (o *ApiKeyDetailsCreated) HasRateLimitRpm() bool`

HasRateLimitRpm returns a boolean if a field has been set.

### GetExpiresAt

`func (o *ApiKeyDetailsCreated) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *ApiKeyDetailsCreated) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *ApiKeyDetailsCreated) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.

### HasExpiresAt

`func (o *ApiKeyDetailsCreated) HasExpiresAt() bool`

HasExpiresAt returns a boolean if a field has been set.

### GetLastUsedAt

`func (o *ApiKeyDetailsCreated) GetLastUsedAt() time.Time`

GetLastUsedAt returns the LastUsedAt field if non-nil, zero value otherwise.

### GetLastUsedAtOk

`func (o *ApiKeyDetailsCreated) GetLastUsedAtOk() (*time.Time, bool)`

GetLastUsedAtOk returns a tuple with the LastUsedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastUsedAt

`func (o *ApiKeyDetailsCreated) SetLastUsedAt(v time.Time)`

SetLastUsedAt sets LastUsedAt field to given value.

### HasLastUsedAt

`func (o *ApiKeyDetailsCreated) HasLastUsedAt() bool`

HasLastUsedAt returns a boolean if a field has been set.

### GetLastUsedIp

`func (o *ApiKeyDetailsCreated) GetLastUsedIp() string`

GetLastUsedIp returns the LastUsedIp field if non-nil, zero value otherwise.

### GetLastUsedIpOk

`func (o *ApiKeyDetailsCreated) GetLastUsedIpOk() (*string, bool)`

GetLastUsedIpOk returns a tuple with the LastUsedIp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastUsedIp

`func (o *ApiKeyDetailsCreated) SetLastUsedIp(v string)`

SetLastUsedIp sets LastUsedIp field to given value.

### HasLastUsedIp

`func (o *ApiKeyDetailsCreated) HasLastUsedIp() bool`

HasLastUsedIp returns a boolean if a field has been set.

### GetCallCount

`func (o *ApiKeyDetailsCreated) GetCallCount() int32`

GetCallCount returns the CallCount field if non-nil, zero value otherwise.

### GetCallCountOk

`func (o *ApiKeyDetailsCreated) GetCallCountOk() (*int32, bool)`

GetCallCountOk returns a tuple with the CallCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCallCount

`func (o *ApiKeyDetailsCreated) SetCallCount(v int32)`

SetCallCount sets CallCount field to given value.

### HasCallCount

`func (o *ApiKeyDetailsCreated) HasCallCount() bool`

HasCallCount returns a boolean if a field has been set.

### GetRevokedAt

`func (o *ApiKeyDetailsCreated) GetRevokedAt() time.Time`

GetRevokedAt returns the RevokedAt field if non-nil, zero value otherwise.

### GetRevokedAtOk

`func (o *ApiKeyDetailsCreated) GetRevokedAtOk() (*time.Time, bool)`

GetRevokedAtOk returns a tuple with the RevokedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRevokedAt

`func (o *ApiKeyDetailsCreated) SetRevokedAt(v time.Time)`

SetRevokedAt sets RevokedAt field to given value.

### HasRevokedAt

`func (o *ApiKeyDetailsCreated) HasRevokedAt() bool`

HasRevokedAt returns a boolean if a field has been set.

### GetCreatedAt

`func (o *ApiKeyDetailsCreated) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *ApiKeyDetailsCreated) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *ApiKeyDetailsCreated) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *ApiKeyDetailsCreated) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetKey

`func (o *ApiKeyDetailsCreated) GetKey() string`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *ApiKeyDetailsCreated) GetKeyOk() (*string, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *ApiKeyDetailsCreated) SetKey(v string)`

SetKey sets Key field to given value.

### HasKey

`func (o *ApiKeyDetailsCreated) HasKey() bool`

HasKey returns a boolean if a field has been set.

### GetMessage

`func (o *ApiKeyDetailsCreated) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *ApiKeyDetailsCreated) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *ApiKeyDetailsCreated) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *ApiKeyDetailsCreated) HasMessage() bool`

HasMessage returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


