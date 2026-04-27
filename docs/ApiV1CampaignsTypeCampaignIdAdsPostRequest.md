# ApiV1CampaignsTypeCampaignIdAdsPostRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Title** | **string** |  | 
**Bid** | **float32** |  | 
**DestinationUrl** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**DisplayUrl** | Pointer to **string** |  | [optional] 
**PreviewUrl** | Pointer to **string** |  | [optional] 
**IsActive** | Pointer to **bool** |  | [optional] [default to true]
**SortWeight** | Pointer to **int32** |  | [optional] [default to 0]
**BannerPoolId** | Pointer to **int32** | Reference an existing banner pool (most common). | [optional] 
**VideoPoolId** | Pointer to **int32** |  | [optional] 
**UrlPoolId** | Pointer to **int32** | Independent click-URL rotation pool — combinable with any banner ref. | [optional] 
**CreativeId** | Pointer to **int32** | Reference a single creative directly. | [optional] 
**BannerUrl** | Pointer to **string** | Direct image URL (hosted-elsewhere creatives). | [optional] 
**BannerHtml** | Pointer to **string** | Raw HTML/JS payload (tag-based ad units). | [optional] 
**Bansizeid** | Pointer to **int32** | Auto-derived for pool/creative refs; required for url/html on size-aware adtypes. | [optional] 

## Methods

### NewApiV1CampaignsTypeCampaignIdAdsPostRequest

`func NewApiV1CampaignsTypeCampaignIdAdsPostRequest(title string, bid float32, ) *ApiV1CampaignsTypeCampaignIdAdsPostRequest`

NewApiV1CampaignsTypeCampaignIdAdsPostRequest instantiates a new ApiV1CampaignsTypeCampaignIdAdsPostRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiV1CampaignsTypeCampaignIdAdsPostRequestWithDefaults

`func NewApiV1CampaignsTypeCampaignIdAdsPostRequestWithDefaults() *ApiV1CampaignsTypeCampaignIdAdsPostRequest`

NewApiV1CampaignsTypeCampaignIdAdsPostRequestWithDefaults instantiates a new ApiV1CampaignsTypeCampaignIdAdsPostRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTitle

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetBid

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetBid() float32`

GetBid returns the Bid field if non-nil, zero value otherwise.

### GetBidOk

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetBidOk() (*float32, bool)`

GetBidOk returns a tuple with the Bid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBid

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) SetBid(v float32)`

SetBid sets Bid field to given value.


### GetDestinationUrl

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetDestinationUrl() string`

GetDestinationUrl returns the DestinationUrl field if non-nil, zero value otherwise.

### GetDestinationUrlOk

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetDestinationUrlOk() (*string, bool)`

GetDestinationUrlOk returns a tuple with the DestinationUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDestinationUrl

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) SetDestinationUrl(v string)`

SetDestinationUrl sets DestinationUrl field to given value.

### HasDestinationUrl

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) HasDestinationUrl() bool`

HasDestinationUrl returns a boolean if a field has been set.

### GetDescription

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetDisplayUrl

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetDisplayUrl() string`

GetDisplayUrl returns the DisplayUrl field if non-nil, zero value otherwise.

### GetDisplayUrlOk

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetDisplayUrlOk() (*string, bool)`

GetDisplayUrlOk returns a tuple with the DisplayUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayUrl

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) SetDisplayUrl(v string)`

SetDisplayUrl sets DisplayUrl field to given value.

### HasDisplayUrl

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) HasDisplayUrl() bool`

HasDisplayUrl returns a boolean if a field has been set.

### GetPreviewUrl

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetPreviewUrl() string`

GetPreviewUrl returns the PreviewUrl field if non-nil, zero value otherwise.

### GetPreviewUrlOk

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetPreviewUrlOk() (*string, bool)`

GetPreviewUrlOk returns a tuple with the PreviewUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPreviewUrl

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) SetPreviewUrl(v string)`

SetPreviewUrl sets PreviewUrl field to given value.

### HasPreviewUrl

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) HasPreviewUrl() bool`

HasPreviewUrl returns a boolean if a field has been set.

### GetIsActive

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetIsActive() bool`

GetIsActive returns the IsActive field if non-nil, zero value otherwise.

### GetIsActiveOk

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetIsActiveOk() (*bool, bool)`

GetIsActiveOk returns a tuple with the IsActive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsActive

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) SetIsActive(v bool)`

SetIsActive sets IsActive field to given value.

### HasIsActive

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) HasIsActive() bool`

HasIsActive returns a boolean if a field has been set.

### GetSortWeight

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetSortWeight() int32`

GetSortWeight returns the SortWeight field if non-nil, zero value otherwise.

### GetSortWeightOk

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetSortWeightOk() (*int32, bool)`

GetSortWeightOk returns a tuple with the SortWeight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortWeight

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) SetSortWeight(v int32)`

SetSortWeight sets SortWeight field to given value.

### HasSortWeight

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) HasSortWeight() bool`

HasSortWeight returns a boolean if a field has been set.

### GetBannerPoolId

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetBannerPoolId() int32`

GetBannerPoolId returns the BannerPoolId field if non-nil, zero value otherwise.

### GetBannerPoolIdOk

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetBannerPoolIdOk() (*int32, bool)`

GetBannerPoolIdOk returns a tuple with the BannerPoolId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBannerPoolId

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) SetBannerPoolId(v int32)`

SetBannerPoolId sets BannerPoolId field to given value.

### HasBannerPoolId

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) HasBannerPoolId() bool`

HasBannerPoolId returns a boolean if a field has been set.

### GetVideoPoolId

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetVideoPoolId() int32`

GetVideoPoolId returns the VideoPoolId field if non-nil, zero value otherwise.

### GetVideoPoolIdOk

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetVideoPoolIdOk() (*int32, bool)`

GetVideoPoolIdOk returns a tuple with the VideoPoolId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVideoPoolId

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) SetVideoPoolId(v int32)`

SetVideoPoolId sets VideoPoolId field to given value.

### HasVideoPoolId

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) HasVideoPoolId() bool`

HasVideoPoolId returns a boolean if a field has been set.

### GetUrlPoolId

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetUrlPoolId() int32`

GetUrlPoolId returns the UrlPoolId field if non-nil, zero value otherwise.

### GetUrlPoolIdOk

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetUrlPoolIdOk() (*int32, bool)`

GetUrlPoolIdOk returns a tuple with the UrlPoolId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrlPoolId

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) SetUrlPoolId(v int32)`

SetUrlPoolId sets UrlPoolId field to given value.

### HasUrlPoolId

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) HasUrlPoolId() bool`

HasUrlPoolId returns a boolean if a field has been set.

### GetCreativeId

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetCreativeId() int32`

GetCreativeId returns the CreativeId field if non-nil, zero value otherwise.

### GetCreativeIdOk

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetCreativeIdOk() (*int32, bool)`

GetCreativeIdOk returns a tuple with the CreativeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreativeId

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) SetCreativeId(v int32)`

SetCreativeId sets CreativeId field to given value.

### HasCreativeId

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) HasCreativeId() bool`

HasCreativeId returns a boolean if a field has been set.

### GetBannerUrl

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetBannerUrl() string`

GetBannerUrl returns the BannerUrl field if non-nil, zero value otherwise.

### GetBannerUrlOk

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetBannerUrlOk() (*string, bool)`

GetBannerUrlOk returns a tuple with the BannerUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBannerUrl

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) SetBannerUrl(v string)`

SetBannerUrl sets BannerUrl field to given value.

### HasBannerUrl

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) HasBannerUrl() bool`

HasBannerUrl returns a boolean if a field has been set.

### GetBannerHtml

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetBannerHtml() string`

GetBannerHtml returns the BannerHtml field if non-nil, zero value otherwise.

### GetBannerHtmlOk

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetBannerHtmlOk() (*string, bool)`

GetBannerHtmlOk returns a tuple with the BannerHtml field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBannerHtml

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) SetBannerHtml(v string)`

SetBannerHtml sets BannerHtml field to given value.

### HasBannerHtml

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) HasBannerHtml() bool`

HasBannerHtml returns a boolean if a field has been set.

### GetBansizeid

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetBansizeid() int32`

GetBansizeid returns the Bansizeid field if non-nil, zero value otherwise.

### GetBansizeidOk

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) GetBansizeidOk() (*int32, bool)`

GetBansizeidOk returns a tuple with the Bansizeid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBansizeid

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) SetBansizeid(v int32)`

SetBansizeid sets Bansizeid field to given value.

### HasBansizeid

`func (o *ApiV1CampaignsTypeCampaignIdAdsPostRequest) HasBansizeid() bool`

HasBansizeid returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


