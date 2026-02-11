# Coach

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Certifications** | Pointer to **[]string** | Coaching certifications and licenses | [optional] 
**CharacterId** | **string** | ID of the character (references /characters/{id}) | 
**Id** | **string** | Unique identifier for this team membership | 
**MemberType** | Pointer to **string** | Discriminator field indicating this is a coach | [optional] [default to "coach"]
**Specialty** | [**CoachSpecialty**](CoachSpecialty.md) | Coaching specialty/role | 
**TeamId** | **string** | ID of the team they belong to | 
**WinRate** | Pointer to **NullableFloat32** |  | [optional] 
**YearsWithTeam** | **int32** | Number of years with the current team | 

## Methods

### NewCoach

`func NewCoach(characterId string, id string, specialty CoachSpecialty, teamId string, yearsWithTeam int32, ) *Coach`

NewCoach instantiates a new Coach object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCoachWithDefaults

`func NewCoachWithDefaults() *Coach`

NewCoachWithDefaults instantiates a new Coach object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCertifications

`func (o *Coach) GetCertifications() []string`

GetCertifications returns the Certifications field if non-nil, zero value otherwise.

### GetCertificationsOk

`func (o *Coach) GetCertificationsOk() (*[]string, bool)`

GetCertificationsOk returns a tuple with the Certifications field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCertifications

`func (o *Coach) SetCertifications(v []string)`

SetCertifications sets Certifications field to given value.

### HasCertifications

`func (o *Coach) HasCertifications() bool`

HasCertifications returns a boolean if a field has been set.

### GetCharacterId

`func (o *Coach) GetCharacterId() string`

GetCharacterId returns the CharacterId field if non-nil, zero value otherwise.

### GetCharacterIdOk

`func (o *Coach) GetCharacterIdOk() (*string, bool)`

GetCharacterIdOk returns a tuple with the CharacterId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCharacterId

`func (o *Coach) SetCharacterId(v string)`

SetCharacterId sets CharacterId field to given value.


### GetId

`func (o *Coach) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Coach) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Coach) SetId(v string)`

SetId sets Id field to given value.


### GetMemberType

`func (o *Coach) GetMemberType() string`

GetMemberType returns the MemberType field if non-nil, zero value otherwise.

### GetMemberTypeOk

`func (o *Coach) GetMemberTypeOk() (*string, bool)`

GetMemberTypeOk returns a tuple with the MemberType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMemberType

`func (o *Coach) SetMemberType(v string)`

SetMemberType sets MemberType field to given value.

### HasMemberType

`func (o *Coach) HasMemberType() bool`

HasMemberType returns a boolean if a field has been set.

### GetSpecialty

`func (o *Coach) GetSpecialty() CoachSpecialty`

GetSpecialty returns the Specialty field if non-nil, zero value otherwise.

### GetSpecialtyOk

`func (o *Coach) GetSpecialtyOk() (*CoachSpecialty, bool)`

GetSpecialtyOk returns a tuple with the Specialty field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSpecialty

`func (o *Coach) SetSpecialty(v CoachSpecialty)`

SetSpecialty sets Specialty field to given value.


### GetTeamId

`func (o *Coach) GetTeamId() string`

GetTeamId returns the TeamId field if non-nil, zero value otherwise.

### GetTeamIdOk

`func (o *Coach) GetTeamIdOk() (*string, bool)`

GetTeamIdOk returns a tuple with the TeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamId

`func (o *Coach) SetTeamId(v string)`

SetTeamId sets TeamId field to given value.


### GetWinRate

`func (o *Coach) GetWinRate() float32`

GetWinRate returns the WinRate field if non-nil, zero value otherwise.

### GetWinRateOk

`func (o *Coach) GetWinRateOk() (*float32, bool)`

GetWinRateOk returns a tuple with the WinRate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWinRate

`func (o *Coach) SetWinRate(v float32)`

SetWinRate sets WinRate field to given value.

### HasWinRate

`func (o *Coach) HasWinRate() bool`

HasWinRate returns a boolean if a field has been set.

### SetWinRateNil

`func (o *Coach) SetWinRateNil(b bool)`

 SetWinRateNil sets the value for WinRate to be an explicit nil

### UnsetWinRate
`func (o *Coach) UnsetWinRate()`

UnsetWinRate ensures that no value is present for WinRate, not even an explicit nil
### GetYearsWithTeam

`func (o *Coach) GetYearsWithTeam() int32`

GetYearsWithTeam returns the YearsWithTeam field if non-nil, zero value otherwise.

### GetYearsWithTeamOk

`func (o *Coach) GetYearsWithTeamOk() (*int32, bool)`

GetYearsWithTeamOk returns a tuple with the YearsWithTeam field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetYearsWithTeam

`func (o *Coach) SetYearsWithTeam(v int32)`

SetYearsWithTeam sets YearsWithTeam field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


