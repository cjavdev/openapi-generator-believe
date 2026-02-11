# MedicalStaffUpdate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**LicenseNumber** | Pointer to **NullableString** |  | [optional] 
**Qualifications** | Pointer to **[]string** |  | [optional] 
**Specialty** | Pointer to [**NullableMedicalSpecialty**](MedicalSpecialty.md) |  | [optional] 
**TeamId** | Pointer to **NullableString** |  | [optional] 
**YearsWithTeam** | Pointer to **NullableInt32** |  | [optional] 

## Methods

### NewMedicalStaffUpdate

`func NewMedicalStaffUpdate() *MedicalStaffUpdate`

NewMedicalStaffUpdate instantiates a new MedicalStaffUpdate object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMedicalStaffUpdateWithDefaults

`func NewMedicalStaffUpdateWithDefaults() *MedicalStaffUpdate`

NewMedicalStaffUpdateWithDefaults instantiates a new MedicalStaffUpdate object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLicenseNumber

`func (o *MedicalStaffUpdate) GetLicenseNumber() string`

GetLicenseNumber returns the LicenseNumber field if non-nil, zero value otherwise.

### GetLicenseNumberOk

`func (o *MedicalStaffUpdate) GetLicenseNumberOk() (*string, bool)`

GetLicenseNumberOk returns a tuple with the LicenseNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLicenseNumber

`func (o *MedicalStaffUpdate) SetLicenseNumber(v string)`

SetLicenseNumber sets LicenseNumber field to given value.

### HasLicenseNumber

`func (o *MedicalStaffUpdate) HasLicenseNumber() bool`

HasLicenseNumber returns a boolean if a field has been set.

### SetLicenseNumberNil

`func (o *MedicalStaffUpdate) SetLicenseNumberNil(b bool)`

 SetLicenseNumberNil sets the value for LicenseNumber to be an explicit nil

### UnsetLicenseNumber
`func (o *MedicalStaffUpdate) UnsetLicenseNumber()`

UnsetLicenseNumber ensures that no value is present for LicenseNumber, not even an explicit nil
### GetQualifications

`func (o *MedicalStaffUpdate) GetQualifications() []string`

GetQualifications returns the Qualifications field if non-nil, zero value otherwise.

### GetQualificationsOk

`func (o *MedicalStaffUpdate) GetQualificationsOk() (*[]string, bool)`

GetQualificationsOk returns a tuple with the Qualifications field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQualifications

`func (o *MedicalStaffUpdate) SetQualifications(v []string)`

SetQualifications sets Qualifications field to given value.

### HasQualifications

`func (o *MedicalStaffUpdate) HasQualifications() bool`

HasQualifications returns a boolean if a field has been set.

### SetQualificationsNil

`func (o *MedicalStaffUpdate) SetQualificationsNil(b bool)`

 SetQualificationsNil sets the value for Qualifications to be an explicit nil

### UnsetQualifications
`func (o *MedicalStaffUpdate) UnsetQualifications()`

UnsetQualifications ensures that no value is present for Qualifications, not even an explicit nil
### GetSpecialty

`func (o *MedicalStaffUpdate) GetSpecialty() MedicalSpecialty`

GetSpecialty returns the Specialty field if non-nil, zero value otherwise.

### GetSpecialtyOk

`func (o *MedicalStaffUpdate) GetSpecialtyOk() (*MedicalSpecialty, bool)`

GetSpecialtyOk returns a tuple with the Specialty field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSpecialty

`func (o *MedicalStaffUpdate) SetSpecialty(v MedicalSpecialty)`

SetSpecialty sets Specialty field to given value.

### HasSpecialty

`func (o *MedicalStaffUpdate) HasSpecialty() bool`

HasSpecialty returns a boolean if a field has been set.

### SetSpecialtyNil

`func (o *MedicalStaffUpdate) SetSpecialtyNil(b bool)`

 SetSpecialtyNil sets the value for Specialty to be an explicit nil

### UnsetSpecialty
`func (o *MedicalStaffUpdate) UnsetSpecialty()`

UnsetSpecialty ensures that no value is present for Specialty, not even an explicit nil
### GetTeamId

`func (o *MedicalStaffUpdate) GetTeamId() string`

GetTeamId returns the TeamId field if non-nil, zero value otherwise.

### GetTeamIdOk

`func (o *MedicalStaffUpdate) GetTeamIdOk() (*string, bool)`

GetTeamIdOk returns a tuple with the TeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamId

`func (o *MedicalStaffUpdate) SetTeamId(v string)`

SetTeamId sets TeamId field to given value.

### HasTeamId

`func (o *MedicalStaffUpdate) HasTeamId() bool`

HasTeamId returns a boolean if a field has been set.

### SetTeamIdNil

`func (o *MedicalStaffUpdate) SetTeamIdNil(b bool)`

 SetTeamIdNil sets the value for TeamId to be an explicit nil

### UnsetTeamId
`func (o *MedicalStaffUpdate) UnsetTeamId()`

UnsetTeamId ensures that no value is present for TeamId, not even an explicit nil
### GetYearsWithTeam

`func (o *MedicalStaffUpdate) GetYearsWithTeam() int32`

GetYearsWithTeam returns the YearsWithTeam field if non-nil, zero value otherwise.

### GetYearsWithTeamOk

`func (o *MedicalStaffUpdate) GetYearsWithTeamOk() (*int32, bool)`

GetYearsWithTeamOk returns a tuple with the YearsWithTeam field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetYearsWithTeam

`func (o *MedicalStaffUpdate) SetYearsWithTeam(v int32)`

SetYearsWithTeam sets YearsWithTeam field to given value.

### HasYearsWithTeam

`func (o *MedicalStaffUpdate) HasYearsWithTeam() bool`

HasYearsWithTeam returns a boolean if a field has been set.

### SetYearsWithTeamNil

`func (o *MedicalStaffUpdate) SetYearsWithTeamNil(b bool)`

 SetYearsWithTeamNil sets the value for YearsWithTeam to be an explicit nil

### UnsetYearsWithTeam
`func (o *MedicalStaffUpdate) UnsetYearsWithTeam()`

UnsetYearsWithTeam ensures that no value is present for YearsWithTeam, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


