# BelieveRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Context** | Pointer to **NullableString** |  | [optional] 
**Intensity** | Pointer to **int32** | How intense is the response needed (1&#x3D;gentle, 10&#x3D;full Ted) | [optional] [default to 5]
**Situation** | **string** | Describe your situation | 
**SituationType** | [**SituationType**](SituationType.md) | Type of situation | 

## Methods

### NewBelieveRequest

`func NewBelieveRequest(situation string, situationType SituationType, ) *BelieveRequest`

NewBelieveRequest instantiates a new BelieveRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBelieveRequestWithDefaults

`func NewBelieveRequestWithDefaults() *BelieveRequest`

NewBelieveRequestWithDefaults instantiates a new BelieveRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetContext

`func (o *BelieveRequest) GetContext() string`

GetContext returns the Context field if non-nil, zero value otherwise.

### GetContextOk

`func (o *BelieveRequest) GetContextOk() (*string, bool)`

GetContextOk returns a tuple with the Context field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContext

`func (o *BelieveRequest) SetContext(v string)`

SetContext sets Context field to given value.

### HasContext

`func (o *BelieveRequest) HasContext() bool`

HasContext returns a boolean if a field has been set.

### SetContextNil

`func (o *BelieveRequest) SetContextNil(b bool)`

 SetContextNil sets the value for Context to be an explicit nil

### UnsetContext
`func (o *BelieveRequest) UnsetContext()`

UnsetContext ensures that no value is present for Context, not even an explicit nil
### GetIntensity

`func (o *BelieveRequest) GetIntensity() int32`

GetIntensity returns the Intensity field if non-nil, zero value otherwise.

### GetIntensityOk

`func (o *BelieveRequest) GetIntensityOk() (*int32, bool)`

GetIntensityOk returns a tuple with the Intensity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIntensity

`func (o *BelieveRequest) SetIntensity(v int32)`

SetIntensity sets Intensity field to given value.

### HasIntensity

`func (o *BelieveRequest) HasIntensity() bool`

HasIntensity returns a boolean if a field has been set.

### GetSituation

`func (o *BelieveRequest) GetSituation() string`

GetSituation returns the Situation field if non-nil, zero value otherwise.

### GetSituationOk

`func (o *BelieveRequest) GetSituationOk() (*string, bool)`

GetSituationOk returns a tuple with the Situation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSituation

`func (o *BelieveRequest) SetSituation(v string)`

SetSituation sets Situation field to given value.


### GetSituationType

`func (o *BelieveRequest) GetSituationType() SituationType`

GetSituationType returns the SituationType field if non-nil, zero value otherwise.

### GetSituationTypeOk

`func (o *BelieveRequest) GetSituationTypeOk() (*SituationType, bool)`

GetSituationTypeOk returns a tuple with the SituationType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSituationType

`func (o *BelieveRequest) SetSituationType(v SituationType)`

SetSituationType sets SituationType field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


