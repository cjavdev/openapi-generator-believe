# TurningPoint

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CharacterInvolved** | Pointer to **NullableString** |  | [optional] 
**Description** | **string** | What happened | 
**EmotionalImpact** | **string** | How this affected the team emotionally | 
**Minute** | **int32** | Minute of the match | 

## Methods

### NewTurningPoint

`func NewTurningPoint(description string, emotionalImpact string, minute int32, ) *TurningPoint`

NewTurningPoint instantiates a new TurningPoint object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTurningPointWithDefaults

`func NewTurningPointWithDefaults() *TurningPoint`

NewTurningPointWithDefaults instantiates a new TurningPoint object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCharacterInvolved

`func (o *TurningPoint) GetCharacterInvolved() string`

GetCharacterInvolved returns the CharacterInvolved field if non-nil, zero value otherwise.

### GetCharacterInvolvedOk

`func (o *TurningPoint) GetCharacterInvolvedOk() (*string, bool)`

GetCharacterInvolvedOk returns a tuple with the CharacterInvolved field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCharacterInvolved

`func (o *TurningPoint) SetCharacterInvolved(v string)`

SetCharacterInvolved sets CharacterInvolved field to given value.

### HasCharacterInvolved

`func (o *TurningPoint) HasCharacterInvolved() bool`

HasCharacterInvolved returns a boolean if a field has been set.

### SetCharacterInvolvedNil

`func (o *TurningPoint) SetCharacterInvolvedNil(b bool)`

 SetCharacterInvolvedNil sets the value for CharacterInvolved to be an explicit nil

### UnsetCharacterInvolved
`func (o *TurningPoint) UnsetCharacterInvolved()`

UnsetCharacterInvolved ensures that no value is present for CharacterInvolved, not even an explicit nil
### GetDescription

`func (o *TurningPoint) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *TurningPoint) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *TurningPoint) SetDescription(v string)`

SetDescription sets Description field to given value.


### GetEmotionalImpact

`func (o *TurningPoint) GetEmotionalImpact() string`

GetEmotionalImpact returns the EmotionalImpact field if non-nil, zero value otherwise.

### GetEmotionalImpactOk

`func (o *TurningPoint) GetEmotionalImpactOk() (*string, bool)`

GetEmotionalImpactOk returns a tuple with the EmotionalImpact field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmotionalImpact

`func (o *TurningPoint) SetEmotionalImpact(v string)`

SetEmotionalImpact sets EmotionalImpact field to given value.


### GetMinute

`func (o *TurningPoint) GetMinute() int32`

GetMinute returns the Minute field if non-nil, zero value otherwise.

### GetMinuteOk

`func (o *TurningPoint) GetMinuteOk() (*int32, bool)`

GetMinuteOk returns a tuple with the Minute field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinute

`func (o *TurningPoint) SetMinute(v int32)`

SetMinute sets Minute field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


