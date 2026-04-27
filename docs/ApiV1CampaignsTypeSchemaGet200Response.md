# ApiV1CampaignsTypeSchemaGet200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CampaignType** | Pointer to **string** |  | [optional] 
**Fields** | Pointer to [**[]ApiV1CampaignsTypeSchemaGet200ResponseFieldsInner**](ApiV1CampaignsTypeSchemaGet200ResponseFieldsInner.md) |  | [optional] 
**Notes** | Pointer to **[]string** |  | [optional] 

## Methods

### NewApiV1CampaignsTypeSchemaGet200Response

`func NewApiV1CampaignsTypeSchemaGet200Response() *ApiV1CampaignsTypeSchemaGet200Response`

NewApiV1CampaignsTypeSchemaGet200Response instantiates a new ApiV1CampaignsTypeSchemaGet200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApiV1CampaignsTypeSchemaGet200ResponseWithDefaults

`func NewApiV1CampaignsTypeSchemaGet200ResponseWithDefaults() *ApiV1CampaignsTypeSchemaGet200Response`

NewApiV1CampaignsTypeSchemaGet200ResponseWithDefaults instantiates a new ApiV1CampaignsTypeSchemaGet200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCampaignType

`func (o *ApiV1CampaignsTypeSchemaGet200Response) GetCampaignType() string`

GetCampaignType returns the CampaignType field if non-nil, zero value otherwise.

### GetCampaignTypeOk

`func (o *ApiV1CampaignsTypeSchemaGet200Response) GetCampaignTypeOk() (*string, bool)`

GetCampaignTypeOk returns a tuple with the CampaignType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCampaignType

`func (o *ApiV1CampaignsTypeSchemaGet200Response) SetCampaignType(v string)`

SetCampaignType sets CampaignType field to given value.

### HasCampaignType

`func (o *ApiV1CampaignsTypeSchemaGet200Response) HasCampaignType() bool`

HasCampaignType returns a boolean if a field has been set.

### GetFields

`func (o *ApiV1CampaignsTypeSchemaGet200Response) GetFields() []ApiV1CampaignsTypeSchemaGet200ResponseFieldsInner`

GetFields returns the Fields field if non-nil, zero value otherwise.

### GetFieldsOk

`func (o *ApiV1CampaignsTypeSchemaGet200Response) GetFieldsOk() (*[]ApiV1CampaignsTypeSchemaGet200ResponseFieldsInner, bool)`

GetFieldsOk returns a tuple with the Fields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFields

`func (o *ApiV1CampaignsTypeSchemaGet200Response) SetFields(v []ApiV1CampaignsTypeSchemaGet200ResponseFieldsInner)`

SetFields sets Fields field to given value.

### HasFields

`func (o *ApiV1CampaignsTypeSchemaGet200Response) HasFields() bool`

HasFields returns a boolean if a field has been set.

### GetNotes

`func (o *ApiV1CampaignsTypeSchemaGet200Response) GetNotes() []string`

GetNotes returns the Notes field if non-nil, zero value otherwise.

### GetNotesOk

`func (o *ApiV1CampaignsTypeSchemaGet200Response) GetNotesOk() (*[]string, bool)`

GetNotesOk returns a tuple with the Notes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNotes

`func (o *ApiV1CampaignsTypeSchemaGet200Response) SetNotes(v []string)`

SetNotes sets Notes field to given value.

### HasNotes

`func (o *ApiV1CampaignsTypeSchemaGet200Response) HasNotes() bool`

HasNotes returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


