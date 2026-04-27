# TrackingPixel

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **int32** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**ConversionTypeId** | Pointer to **int32** |  | [optional] 
**PixelCode** | Pointer to **string** | Server-generated 32-char hex; embed in tracking URL. | [optional] 

## Methods

### NewTrackingPixel

`func NewTrackingPixel() *TrackingPixel`

NewTrackingPixel instantiates a new TrackingPixel object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTrackingPixelWithDefaults

`func NewTrackingPixelWithDefaults() *TrackingPixel`

NewTrackingPixelWithDefaults instantiates a new TrackingPixel object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *TrackingPixel) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *TrackingPixel) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *TrackingPixel) SetId(v int32)`

SetId sets Id field to given value.

### HasId

`func (o *TrackingPixel) HasId() bool`

HasId returns a boolean if a field has been set.

### GetName

`func (o *TrackingPixel) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *TrackingPixel) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *TrackingPixel) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *TrackingPixel) HasName() bool`

HasName returns a boolean if a field has been set.

### GetConversionTypeId

`func (o *TrackingPixel) GetConversionTypeId() int32`

GetConversionTypeId returns the ConversionTypeId field if non-nil, zero value otherwise.

### GetConversionTypeIdOk

`func (o *TrackingPixel) GetConversionTypeIdOk() (*int32, bool)`

GetConversionTypeIdOk returns a tuple with the ConversionTypeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConversionTypeId

`func (o *TrackingPixel) SetConversionTypeId(v int32)`

SetConversionTypeId sets ConversionTypeId field to given value.

### HasConversionTypeId

`func (o *TrackingPixel) HasConversionTypeId() bool`

HasConversionTypeId returns a boolean if a field has been set.

### GetPixelCode

`func (o *TrackingPixel) GetPixelCode() string`

GetPixelCode returns the PixelCode field if non-nil, zero value otherwise.

### GetPixelCodeOk

`func (o *TrackingPixel) GetPixelCodeOk() (*string, bool)`

GetPixelCodeOk returns a tuple with the PixelCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPixelCode

`func (o *TrackingPixel) SetPixelCode(v string)`

SetPixelCode sets PixelCode field to given value.

### HasPixelCode

`func (o *TrackingPixel) HasPixelCode() bool`

HasPixelCode returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


