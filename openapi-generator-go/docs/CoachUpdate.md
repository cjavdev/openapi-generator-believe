# CoachUpdate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Certifications** | Pointer to **[]string** |  | [optional] 
**Specialty** | Pointer to [**NullableCoachSpecialty**](CoachSpecialty.md) |  | [optional] 
**TeamId** | Pointer to **NullableString** |  | [optional] 
**WinRate** | Pointer to **NullableFloat32** |  | [optional] 
**YearsWithTeam** | Pointer to **NullableInt32** |  | [optional] 

## Methods

### NewCoachUpdate

`func NewCoachUpdate() *CoachUpdate`

NewCoachUpdate instantiates a new CoachUpdate object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCoachUpdateWithDefaults

`func NewCoachUpdateWithDefaults() *CoachUpdate`

NewCoachUpdateWithDefaults instantiates a new CoachUpdate object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCertifications

`func (o *CoachUpdate) GetCertifications() []string`

GetCertifications returns the Certifications field if non-nil, zero value otherwise.

### GetCertificationsOk

`func (o *CoachUpdate) GetCertificationsOk() (*[]string, bool)`

GetCertificationsOk returns a tuple with the Certifications field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCertifications

`func (o *CoachUpdate) SetCertifications(v []string)`

SetCertifications sets Certifications field to given value.

### HasCertifications

`func (o *CoachUpdate) HasCertifications() bool`

HasCertifications returns a boolean if a field has been set.

### SetCertificationsNil

`func (o *CoachUpdate) SetCertificationsNil(b bool)`

 SetCertificationsNil sets the value for Certifications to be an explicit nil

### UnsetCertifications
`func (o *CoachUpdate) UnsetCertifications()`

UnsetCertifications ensures that no value is present for Certifications, not even an explicit nil
### GetSpecialty

`func (o *CoachUpdate) GetSpecialty() CoachSpecialty`

GetSpecialty returns the Specialty field if non-nil, zero value otherwise.

### GetSpecialtyOk

`func (o *CoachUpdate) GetSpecialtyOk() (*CoachSpecialty, bool)`

GetSpecialtyOk returns a tuple with the Specialty field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSpecialty

`func (o *CoachUpdate) SetSpecialty(v CoachSpecialty)`

SetSpecialty sets Specialty field to given value.

### HasSpecialty

`func (o *CoachUpdate) HasSpecialty() bool`

HasSpecialty returns a boolean if a field has been set.

### SetSpecialtyNil

`func (o *CoachUpdate) SetSpecialtyNil(b bool)`

 SetSpecialtyNil sets the value for Specialty to be an explicit nil

### UnsetSpecialty
`func (o *CoachUpdate) UnsetSpecialty()`

UnsetSpecialty ensures that no value is present for Specialty, not even an explicit nil
### GetTeamId

`func (o *CoachUpdate) GetTeamId() string`

GetTeamId returns the TeamId field if non-nil, zero value otherwise.

### GetTeamIdOk

`func (o *CoachUpdate) GetTeamIdOk() (*string, bool)`

GetTeamIdOk returns a tuple with the TeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamId

`func (o *CoachUpdate) SetTeamId(v string)`

SetTeamId sets TeamId field to given value.

### HasTeamId

`func (o *CoachUpdate) HasTeamId() bool`

HasTeamId returns a boolean if a field has been set.

### SetTeamIdNil

`func (o *CoachUpdate) SetTeamIdNil(b bool)`

 SetTeamIdNil sets the value for TeamId to be an explicit nil

### UnsetTeamId
`func (o *CoachUpdate) UnsetTeamId()`

UnsetTeamId ensures that no value is present for TeamId, not even an explicit nil
### GetWinRate

`func (o *CoachUpdate) GetWinRate() float32`

GetWinRate returns the WinRate field if non-nil, zero value otherwise.

### GetWinRateOk

`func (o *CoachUpdate) GetWinRateOk() (*float32, bool)`

GetWinRateOk returns a tuple with the WinRate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWinRate

`func (o *CoachUpdate) SetWinRate(v float32)`

SetWinRate sets WinRate field to given value.

### HasWinRate

`func (o *CoachUpdate) HasWinRate() bool`

HasWinRate returns a boolean if a field has been set.

### SetWinRateNil

`func (o *CoachUpdate) SetWinRateNil(b bool)`

 SetWinRateNil sets the value for WinRate to be an explicit nil

### UnsetWinRate
`func (o *CoachUpdate) UnsetWinRate()`

UnsetWinRate ensures that no value is present for WinRate, not even an explicit nil
### GetYearsWithTeam

`func (o *CoachUpdate) GetYearsWithTeam() int32`

GetYearsWithTeam returns the YearsWithTeam field if non-nil, zero value otherwise.

### GetYearsWithTeamOk

`func (o *CoachUpdate) GetYearsWithTeamOk() (*int32, bool)`

GetYearsWithTeamOk returns a tuple with the YearsWithTeam field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetYearsWithTeam

`func (o *CoachUpdate) SetYearsWithTeam(v int32)`

SetYearsWithTeam sets YearsWithTeam field to given value.

### HasYearsWithTeam

`func (o *CoachUpdate) HasYearsWithTeam() bool`

HasYearsWithTeam returns a boolean if a field has been set.

### SetYearsWithTeamNil

`func (o *CoachUpdate) SetYearsWithTeamNil(b bool)`

 SetYearsWithTeamNil sets the value for YearsWithTeam to be an explicit nil

### UnsetYearsWithTeam
`func (o *CoachUpdate) UnsetYearsWithTeam()`

UnsetYearsWithTeam ensures that no value is present for YearsWithTeam, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


