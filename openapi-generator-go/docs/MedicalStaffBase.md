# MedicalStaffBase

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CharacterId** | **string** | ID of the character (references /characters/{id}) | 
**LicenseNumber** | Pointer to **NullableString** |  | [optional] 
**MemberType** | Pointer to **string** | Discriminator field indicating this is medical staff | [optional] [default to "medical_staff"]
**Qualifications** | Pointer to **[]string** | Medical qualifications and degrees | [optional] 
**Specialty** | [**MedicalSpecialty**](MedicalSpecialty.md) | Medical specialty | 
**TeamId** | **string** | ID of the team they belong to | 
**YearsWithTeam** | **int32** | Number of years with the current team | 

## Methods

### NewMedicalStaffBase

`func NewMedicalStaffBase(characterId string, specialty MedicalSpecialty, teamId string, yearsWithTeam int32, ) *MedicalStaffBase`

NewMedicalStaffBase instantiates a new MedicalStaffBase object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMedicalStaffBaseWithDefaults

`func NewMedicalStaffBaseWithDefaults() *MedicalStaffBase`

NewMedicalStaffBaseWithDefaults instantiates a new MedicalStaffBase object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCharacterId

`func (o *MedicalStaffBase) GetCharacterId() string`

GetCharacterId returns the CharacterId field if non-nil, zero value otherwise.

### GetCharacterIdOk

`func (o *MedicalStaffBase) GetCharacterIdOk() (*string, bool)`

GetCharacterIdOk returns a tuple with the CharacterId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCharacterId

`func (o *MedicalStaffBase) SetCharacterId(v string)`

SetCharacterId sets CharacterId field to given value.


### GetLicenseNumber

`func (o *MedicalStaffBase) GetLicenseNumber() string`

GetLicenseNumber returns the LicenseNumber field if non-nil, zero value otherwise.

### GetLicenseNumberOk

`func (o *MedicalStaffBase) GetLicenseNumberOk() (*string, bool)`

GetLicenseNumberOk returns a tuple with the LicenseNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLicenseNumber

`func (o *MedicalStaffBase) SetLicenseNumber(v string)`

SetLicenseNumber sets LicenseNumber field to given value.

### HasLicenseNumber

`func (o *MedicalStaffBase) HasLicenseNumber() bool`

HasLicenseNumber returns a boolean if a field has been set.

### SetLicenseNumberNil

`func (o *MedicalStaffBase) SetLicenseNumberNil(b bool)`

 SetLicenseNumberNil sets the value for LicenseNumber to be an explicit nil

### UnsetLicenseNumber
`func (o *MedicalStaffBase) UnsetLicenseNumber()`

UnsetLicenseNumber ensures that no value is present for LicenseNumber, not even an explicit nil
### GetMemberType

`func (o *MedicalStaffBase) GetMemberType() string`

GetMemberType returns the MemberType field if non-nil, zero value otherwise.

### GetMemberTypeOk

`func (o *MedicalStaffBase) GetMemberTypeOk() (*string, bool)`

GetMemberTypeOk returns a tuple with the MemberType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMemberType

`func (o *MedicalStaffBase) SetMemberType(v string)`

SetMemberType sets MemberType field to given value.

### HasMemberType

`func (o *MedicalStaffBase) HasMemberType() bool`

HasMemberType returns a boolean if a field has been set.

### GetQualifications

`func (o *MedicalStaffBase) GetQualifications() []string`

GetQualifications returns the Qualifications field if non-nil, zero value otherwise.

### GetQualificationsOk

`func (o *MedicalStaffBase) GetQualificationsOk() (*[]string, bool)`

GetQualificationsOk returns a tuple with the Qualifications field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQualifications

`func (o *MedicalStaffBase) SetQualifications(v []string)`

SetQualifications sets Qualifications field to given value.

### HasQualifications

`func (o *MedicalStaffBase) HasQualifications() bool`

HasQualifications returns a boolean if a field has been set.

### GetSpecialty

`func (o *MedicalStaffBase) GetSpecialty() MedicalSpecialty`

GetSpecialty returns the Specialty field if non-nil, zero value otherwise.

### GetSpecialtyOk

`func (o *MedicalStaffBase) GetSpecialtyOk() (*MedicalSpecialty, bool)`

GetSpecialtyOk returns a tuple with the Specialty field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSpecialty

`func (o *MedicalStaffBase) SetSpecialty(v MedicalSpecialty)`

SetSpecialty sets Specialty field to given value.


### GetTeamId

`func (o *MedicalStaffBase) GetTeamId() string`

GetTeamId returns the TeamId field if non-nil, zero value otherwise.

### GetTeamIdOk

`func (o *MedicalStaffBase) GetTeamIdOk() (*string, bool)`

GetTeamIdOk returns a tuple with the TeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamId

`func (o *MedicalStaffBase) SetTeamId(v string)`

SetTeamId sets TeamId field to given value.


### GetYearsWithTeam

`func (o *MedicalStaffBase) GetYearsWithTeam() int32`

GetYearsWithTeam returns the YearsWithTeam field if non-nil, zero value otherwise.

### GetYearsWithTeamOk

`func (o *MedicalStaffBase) GetYearsWithTeamOk() (*int32, bool)`

GetYearsWithTeamOk returns a tuple with the YearsWithTeam field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetYearsWithTeam

`func (o *MedicalStaffBase) SetYearsWithTeam(v int32)`

SetYearsWithTeam sets YearsWithTeam field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


