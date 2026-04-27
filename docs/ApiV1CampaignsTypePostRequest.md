# ApiV1CampaignsTypePostRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**AdType** | **int32** | See /campaigns/&lt;type&gt;/_schema for valid ids on this tenant. | 
**DailyBudget** | Pointer to **float32** |  | [optional] 
**TotalBudget** | Pointer to **float32** |  | [optional] 
**UseCampaignBudget** | Pointer to **bool** |  | [optional] [default to false]
**Countries** | Pointer to **string** |  | [optional] 
**Languages** | Pointer to **string** | CSV of language ids; \&quot;0\&quot; &#x3D; all. | [optional] 
**Categories** | Pointer to **string** |  | [optional] 
**MainCatid** | Pointer to **int32** |  | [optional] 
**DeviceTypeIds** | Pointer to **string** |  | [optional] 
**BrowserIds** | Pointer to **string** |  | [optional] 
**OsIds** | Pointer to **string** |  | [optional] 
**IspIds** | Pointer to **string** |  | [optional] 
**SiteTypes** | Pointer to **string** |  | [optional] 
**Regions** | Pointer to **string** |  | [optional] 
**DisplayTimes** | Pointer to **string** |  | [optional] 
**DisplayDays** | Pointer to **string** |  | [optional] 
**UseCapping** | Pointer to **bool** |  | [optional] 
**CappingHours** | Pointer to **int32** |  | [optional] 
**CappingMinutes** | Pointer to **int32** |  | [optional] 
**DomainFilterId** | Pointer to **int32** |  | [optional] 
**WhitelistId** | Pointer to **int32** |  | [optional] 
**RtIncludeId** | Pointer to **int32** |  | [optional] 
**RtExcludeId** | Pointer to **int32** |  | [optional] 
**IpPoolId** | Pointer to **int32** |  | [optional] 
**FxMinprice** | Pointer to **float32** |  | [optional] [default to 0]
**IsPaused** | Pointer to **bool** | Start paused (default) so you can attach ads first. | [optional] [default to true]

## Methods

### NewApiV1CampaignsTypePostRequest

`func NewApiV1CampaignsTypePostRequest(name string, adType int32, ) *ApiV1CampaignsTypePostRequest`

NewApiV1CampaignsTypePostRequest instantiates a new ApiV1CampaignsTypePostRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiV1CampaignsTypePostRequestWithDefaults

`func NewApiV1CampaignsTypePostRequestWithDefaults() *ApiV1CampaignsTypePostRequest`

NewApiV1CampaignsTypePostRequestWithDefaults instantiates a new ApiV1CampaignsTypePostRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *ApiV1CampaignsTypePostRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ApiV1CampaignsTypePostRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ApiV1CampaignsTypePostRequest) SetName(v string)`

SetName sets Name field to given value.


### GetAdType

`func (o *ApiV1CampaignsTypePostRequest) GetAdType() int32`

GetAdType returns the AdType field if non-nil, zero value otherwise.

### GetAdTypeOk

`func (o *ApiV1CampaignsTypePostRequest) GetAdTypeOk() (*int32, bool)`

GetAdTypeOk returns a tuple with the AdType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdType

`func (o *ApiV1CampaignsTypePostRequest) SetAdType(v int32)`

SetAdType sets AdType field to given value.


### GetDailyBudget

`func (o *ApiV1CampaignsTypePostRequest) GetDailyBudget() float32`

GetDailyBudget returns the DailyBudget field if non-nil, zero value otherwise.

### GetDailyBudgetOk

`func (o *ApiV1CampaignsTypePostRequest) GetDailyBudgetOk() (*float32, bool)`

GetDailyBudgetOk returns a tuple with the DailyBudget field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDailyBudget

`func (o *ApiV1CampaignsTypePostRequest) SetDailyBudget(v float32)`

SetDailyBudget sets DailyBudget field to given value.

### HasDailyBudget

`func (o *ApiV1CampaignsTypePostRequest) HasDailyBudget() bool`

HasDailyBudget returns a boolean if a field has been set.

### GetTotalBudget

`func (o *ApiV1CampaignsTypePostRequest) GetTotalBudget() float32`

GetTotalBudget returns the TotalBudget field if non-nil, zero value otherwise.

### GetTotalBudgetOk

`func (o *ApiV1CampaignsTypePostRequest) GetTotalBudgetOk() (*float32, bool)`

GetTotalBudgetOk returns a tuple with the TotalBudget field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalBudget

`func (o *ApiV1CampaignsTypePostRequest) SetTotalBudget(v float32)`

SetTotalBudget sets TotalBudget field to given value.

### HasTotalBudget

`func (o *ApiV1CampaignsTypePostRequest) HasTotalBudget() bool`

HasTotalBudget returns a boolean if a field has been set.

### GetUseCampaignBudget

`func (o *ApiV1CampaignsTypePostRequest) GetUseCampaignBudget() bool`

GetUseCampaignBudget returns the UseCampaignBudget field if non-nil, zero value otherwise.

### GetUseCampaignBudgetOk

`func (o *ApiV1CampaignsTypePostRequest) GetUseCampaignBudgetOk() (*bool, bool)`

GetUseCampaignBudgetOk returns a tuple with the UseCampaignBudget field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUseCampaignBudget

`func (o *ApiV1CampaignsTypePostRequest) SetUseCampaignBudget(v bool)`

SetUseCampaignBudget sets UseCampaignBudget field to given value.

### HasUseCampaignBudget

`func (o *ApiV1CampaignsTypePostRequest) HasUseCampaignBudget() bool`

HasUseCampaignBudget returns a boolean if a field has been set.

### GetCountries

`func (o *ApiV1CampaignsTypePostRequest) GetCountries() string`

GetCountries returns the Countries field if non-nil, zero value otherwise.

### GetCountriesOk

`func (o *ApiV1CampaignsTypePostRequest) GetCountriesOk() (*string, bool)`

GetCountriesOk returns a tuple with the Countries field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountries

`func (o *ApiV1CampaignsTypePostRequest) SetCountries(v string)`

SetCountries sets Countries field to given value.

### HasCountries

`func (o *ApiV1CampaignsTypePostRequest) HasCountries() bool`

HasCountries returns a boolean if a field has been set.

### GetLanguages

`func (o *ApiV1CampaignsTypePostRequest) GetLanguages() string`

GetLanguages returns the Languages field if non-nil, zero value otherwise.

### GetLanguagesOk

`func (o *ApiV1CampaignsTypePostRequest) GetLanguagesOk() (*string, bool)`

GetLanguagesOk returns a tuple with the Languages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLanguages

`func (o *ApiV1CampaignsTypePostRequest) SetLanguages(v string)`

SetLanguages sets Languages field to given value.

### HasLanguages

`func (o *ApiV1CampaignsTypePostRequest) HasLanguages() bool`

HasLanguages returns a boolean if a field has been set.

### GetCategories

`func (o *ApiV1CampaignsTypePostRequest) GetCategories() string`

GetCategories returns the Categories field if non-nil, zero value otherwise.

### GetCategoriesOk

`func (o *ApiV1CampaignsTypePostRequest) GetCategoriesOk() (*string, bool)`

GetCategoriesOk returns a tuple with the Categories field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategories

`func (o *ApiV1CampaignsTypePostRequest) SetCategories(v string)`

SetCategories sets Categories field to given value.

### HasCategories

`func (o *ApiV1CampaignsTypePostRequest) HasCategories() bool`

HasCategories returns a boolean if a field has been set.

### GetMainCatid

`func (o *ApiV1CampaignsTypePostRequest) GetMainCatid() int32`

GetMainCatid returns the MainCatid field if non-nil, zero value otherwise.

### GetMainCatidOk

`func (o *ApiV1CampaignsTypePostRequest) GetMainCatidOk() (*int32, bool)`

GetMainCatidOk returns a tuple with the MainCatid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMainCatid

`func (o *ApiV1CampaignsTypePostRequest) SetMainCatid(v int32)`

SetMainCatid sets MainCatid field to given value.

### HasMainCatid

`func (o *ApiV1CampaignsTypePostRequest) HasMainCatid() bool`

HasMainCatid returns a boolean if a field has been set.

### GetDeviceTypeIds

`func (o *ApiV1CampaignsTypePostRequest) GetDeviceTypeIds() string`

GetDeviceTypeIds returns the DeviceTypeIds field if non-nil, zero value otherwise.

### GetDeviceTypeIdsOk

`func (o *ApiV1CampaignsTypePostRequest) GetDeviceTypeIdsOk() (*string, bool)`

GetDeviceTypeIdsOk returns a tuple with the DeviceTypeIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeviceTypeIds

`func (o *ApiV1CampaignsTypePostRequest) SetDeviceTypeIds(v string)`

SetDeviceTypeIds sets DeviceTypeIds field to given value.

### HasDeviceTypeIds

`func (o *ApiV1CampaignsTypePostRequest) HasDeviceTypeIds() bool`

HasDeviceTypeIds returns a boolean if a field has been set.

### GetBrowserIds

`func (o *ApiV1CampaignsTypePostRequest) GetBrowserIds() string`

GetBrowserIds returns the BrowserIds field if non-nil, zero value otherwise.

### GetBrowserIdsOk

`func (o *ApiV1CampaignsTypePostRequest) GetBrowserIdsOk() (*string, bool)`

GetBrowserIdsOk returns a tuple with the BrowserIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBrowserIds

`func (o *ApiV1CampaignsTypePostRequest) SetBrowserIds(v string)`

SetBrowserIds sets BrowserIds field to given value.

### HasBrowserIds

`func (o *ApiV1CampaignsTypePostRequest) HasBrowserIds() bool`

HasBrowserIds returns a boolean if a field has been set.

### GetOsIds

`func (o *ApiV1CampaignsTypePostRequest) GetOsIds() string`

GetOsIds returns the OsIds field if non-nil, zero value otherwise.

### GetOsIdsOk

`func (o *ApiV1CampaignsTypePostRequest) GetOsIdsOk() (*string, bool)`

GetOsIdsOk returns a tuple with the OsIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOsIds

`func (o *ApiV1CampaignsTypePostRequest) SetOsIds(v string)`

SetOsIds sets OsIds field to given value.

### HasOsIds

`func (o *ApiV1CampaignsTypePostRequest) HasOsIds() bool`

HasOsIds returns a boolean if a field has been set.

### GetIspIds

`func (o *ApiV1CampaignsTypePostRequest) GetIspIds() string`

GetIspIds returns the IspIds field if non-nil, zero value otherwise.

### GetIspIdsOk

`func (o *ApiV1CampaignsTypePostRequest) GetIspIdsOk() (*string, bool)`

GetIspIdsOk returns a tuple with the IspIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIspIds

`func (o *ApiV1CampaignsTypePostRequest) SetIspIds(v string)`

SetIspIds sets IspIds field to given value.

### HasIspIds

`func (o *ApiV1CampaignsTypePostRequest) HasIspIds() bool`

HasIspIds returns a boolean if a field has been set.

### GetSiteTypes

`func (o *ApiV1CampaignsTypePostRequest) GetSiteTypes() string`

GetSiteTypes returns the SiteTypes field if non-nil, zero value otherwise.

### GetSiteTypesOk

`func (o *ApiV1CampaignsTypePostRequest) GetSiteTypesOk() (*string, bool)`

GetSiteTypesOk returns a tuple with the SiteTypes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSiteTypes

`func (o *ApiV1CampaignsTypePostRequest) SetSiteTypes(v string)`

SetSiteTypes sets SiteTypes field to given value.

### HasSiteTypes

`func (o *ApiV1CampaignsTypePostRequest) HasSiteTypes() bool`

HasSiteTypes returns a boolean if a field has been set.

### GetRegions

`func (o *ApiV1CampaignsTypePostRequest) GetRegions() string`

GetRegions returns the Regions field if non-nil, zero value otherwise.

### GetRegionsOk

`func (o *ApiV1CampaignsTypePostRequest) GetRegionsOk() (*string, bool)`

GetRegionsOk returns a tuple with the Regions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegions

`func (o *ApiV1CampaignsTypePostRequest) SetRegions(v string)`

SetRegions sets Regions field to given value.

### HasRegions

`func (o *ApiV1CampaignsTypePostRequest) HasRegions() bool`

HasRegions returns a boolean if a field has been set.

### GetDisplayTimes

`func (o *ApiV1CampaignsTypePostRequest) GetDisplayTimes() string`

GetDisplayTimes returns the DisplayTimes field if non-nil, zero value otherwise.

### GetDisplayTimesOk

`func (o *ApiV1CampaignsTypePostRequest) GetDisplayTimesOk() (*string, bool)`

GetDisplayTimesOk returns a tuple with the DisplayTimes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayTimes

`func (o *ApiV1CampaignsTypePostRequest) SetDisplayTimes(v string)`

SetDisplayTimes sets DisplayTimes field to given value.

### HasDisplayTimes

`func (o *ApiV1CampaignsTypePostRequest) HasDisplayTimes() bool`

HasDisplayTimes returns a boolean if a field has been set.

### GetDisplayDays

`func (o *ApiV1CampaignsTypePostRequest) GetDisplayDays() string`

GetDisplayDays returns the DisplayDays field if non-nil, zero value otherwise.

### GetDisplayDaysOk

`func (o *ApiV1CampaignsTypePostRequest) GetDisplayDaysOk() (*string, bool)`

GetDisplayDaysOk returns a tuple with the DisplayDays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayDays

`func (o *ApiV1CampaignsTypePostRequest) SetDisplayDays(v string)`

SetDisplayDays sets DisplayDays field to given value.

### HasDisplayDays

`func (o *ApiV1CampaignsTypePostRequest) HasDisplayDays() bool`

HasDisplayDays returns a boolean if a field has been set.

### GetUseCapping

`func (o *ApiV1CampaignsTypePostRequest) GetUseCapping() bool`

GetUseCapping returns the UseCapping field if non-nil, zero value otherwise.

### GetUseCappingOk

`func (o *ApiV1CampaignsTypePostRequest) GetUseCappingOk() (*bool, bool)`

GetUseCappingOk returns a tuple with the UseCapping field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUseCapping

`func (o *ApiV1CampaignsTypePostRequest) SetUseCapping(v bool)`

SetUseCapping sets UseCapping field to given value.

### HasUseCapping

`func (o *ApiV1CampaignsTypePostRequest) HasUseCapping() bool`

HasUseCapping returns a boolean if a field has been set.

### GetCappingHours

`func (o *ApiV1CampaignsTypePostRequest) GetCappingHours() int32`

GetCappingHours returns the CappingHours field if non-nil, zero value otherwise.

### GetCappingHoursOk

`func (o *ApiV1CampaignsTypePostRequest) GetCappingHoursOk() (*int32, bool)`

GetCappingHoursOk returns a tuple with the CappingHours field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCappingHours

`func (o *ApiV1CampaignsTypePostRequest) SetCappingHours(v int32)`

SetCappingHours sets CappingHours field to given value.

### HasCappingHours

`func (o *ApiV1CampaignsTypePostRequest) HasCappingHours() bool`

HasCappingHours returns a boolean if a field has been set.

### GetCappingMinutes

`func (o *ApiV1CampaignsTypePostRequest) GetCappingMinutes() int32`

GetCappingMinutes returns the CappingMinutes field if non-nil, zero value otherwise.

### GetCappingMinutesOk

`func (o *ApiV1CampaignsTypePostRequest) GetCappingMinutesOk() (*int32, bool)`

GetCappingMinutesOk returns a tuple with the CappingMinutes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCappingMinutes

`func (o *ApiV1CampaignsTypePostRequest) SetCappingMinutes(v int32)`

SetCappingMinutes sets CappingMinutes field to given value.

### HasCappingMinutes

`func (o *ApiV1CampaignsTypePostRequest) HasCappingMinutes() bool`

HasCappingMinutes returns a boolean if a field has been set.

### GetDomainFilterId

`func (o *ApiV1CampaignsTypePostRequest) GetDomainFilterId() int32`

GetDomainFilterId returns the DomainFilterId field if non-nil, zero value otherwise.

### GetDomainFilterIdOk

`func (o *ApiV1CampaignsTypePostRequest) GetDomainFilterIdOk() (*int32, bool)`

GetDomainFilterIdOk returns a tuple with the DomainFilterId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDomainFilterId

`func (o *ApiV1CampaignsTypePostRequest) SetDomainFilterId(v int32)`

SetDomainFilterId sets DomainFilterId field to given value.

### HasDomainFilterId

`func (o *ApiV1CampaignsTypePostRequest) HasDomainFilterId() bool`

HasDomainFilterId returns a boolean if a field has been set.

### GetWhitelistId

`func (o *ApiV1CampaignsTypePostRequest) GetWhitelistId() int32`

GetWhitelistId returns the WhitelistId field if non-nil, zero value otherwise.

### GetWhitelistIdOk

`func (o *ApiV1CampaignsTypePostRequest) GetWhitelistIdOk() (*int32, bool)`

GetWhitelistIdOk returns a tuple with the WhitelistId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWhitelistId

`func (o *ApiV1CampaignsTypePostRequest) SetWhitelistId(v int32)`

SetWhitelistId sets WhitelistId field to given value.

### HasWhitelistId

`func (o *ApiV1CampaignsTypePostRequest) HasWhitelistId() bool`

HasWhitelistId returns a boolean if a field has been set.

### GetRtIncludeId

`func (o *ApiV1CampaignsTypePostRequest) GetRtIncludeId() int32`

GetRtIncludeId returns the RtIncludeId field if non-nil, zero value otherwise.

### GetRtIncludeIdOk

`func (o *ApiV1CampaignsTypePostRequest) GetRtIncludeIdOk() (*int32, bool)`

GetRtIncludeIdOk returns a tuple with the RtIncludeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRtIncludeId

`func (o *ApiV1CampaignsTypePostRequest) SetRtIncludeId(v int32)`

SetRtIncludeId sets RtIncludeId field to given value.

### HasRtIncludeId

`func (o *ApiV1CampaignsTypePostRequest) HasRtIncludeId() bool`

HasRtIncludeId returns a boolean if a field has been set.

### GetRtExcludeId

`func (o *ApiV1CampaignsTypePostRequest) GetRtExcludeId() int32`

GetRtExcludeId returns the RtExcludeId field if non-nil, zero value otherwise.

### GetRtExcludeIdOk

`func (o *ApiV1CampaignsTypePostRequest) GetRtExcludeIdOk() (*int32, bool)`

GetRtExcludeIdOk returns a tuple with the RtExcludeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRtExcludeId

`func (o *ApiV1CampaignsTypePostRequest) SetRtExcludeId(v int32)`

SetRtExcludeId sets RtExcludeId field to given value.

### HasRtExcludeId

`func (o *ApiV1CampaignsTypePostRequest) HasRtExcludeId() bool`

HasRtExcludeId returns a boolean if a field has been set.

### GetIpPoolId

`func (o *ApiV1CampaignsTypePostRequest) GetIpPoolId() int32`

GetIpPoolId returns the IpPoolId field if non-nil, zero value otherwise.

### GetIpPoolIdOk

`func (o *ApiV1CampaignsTypePostRequest) GetIpPoolIdOk() (*int32, bool)`

GetIpPoolIdOk returns a tuple with the IpPoolId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIpPoolId

`func (o *ApiV1CampaignsTypePostRequest) SetIpPoolId(v int32)`

SetIpPoolId sets IpPoolId field to given value.

### HasIpPoolId

`func (o *ApiV1CampaignsTypePostRequest) HasIpPoolId() bool`

HasIpPoolId returns a boolean if a field has been set.

### GetFxMinprice

`func (o *ApiV1CampaignsTypePostRequest) GetFxMinprice() float32`

GetFxMinprice returns the FxMinprice field if non-nil, zero value otherwise.

### GetFxMinpriceOk

`func (o *ApiV1CampaignsTypePostRequest) GetFxMinpriceOk() (*float32, bool)`

GetFxMinpriceOk returns a tuple with the FxMinprice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFxMinprice

`func (o *ApiV1CampaignsTypePostRequest) SetFxMinprice(v float32)`

SetFxMinprice sets FxMinprice field to given value.

### HasFxMinprice

`func (o *ApiV1CampaignsTypePostRequest) HasFxMinprice() bool`

HasFxMinprice returns a boolean if a field has been set.

### GetIsPaused

`func (o *ApiV1CampaignsTypePostRequest) GetIsPaused() bool`

GetIsPaused returns the IsPaused field if non-nil, zero value otherwise.

### GetIsPausedOk

`func (o *ApiV1CampaignsTypePostRequest) GetIsPausedOk() (*bool, bool)`

GetIsPausedOk returns a tuple with the IsPaused field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsPaused

`func (o *ApiV1CampaignsTypePostRequest) SetIsPaused(v bool)`

SetIsPaused sets IsPaused field to given value.

### HasIsPaused

`func (o *ApiV1CampaignsTypePostRequest) HasIsPaused() bool`

HasIsPaused returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


