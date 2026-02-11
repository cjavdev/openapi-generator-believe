# Updates

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Assists** | Pointer to **int32** |  | [optional] 
**GoalsScored** | Pointer to **int32** |  | [optional] 
**IsCaptain** | Pointer to **bool** |  | [optional] 
**JerseyNumber** | Pointer to **int32** |  | [optional] 
**Position** | Pointer to [**Position**](Position.md) |  | [optional] 
**TeamId** | Pointer to **string** |  | [optional] 
**YearsWithTeam** | Pointer to **int32** |  | [optional] 
**Certifications** | Pointer to **[]string** |  | [optional] 
**Specialty** | Pointer to [**MedicalSpecialty**](MedicalSpecialty.md) |  | [optional] 
**WinRate** | Pointer to **float32** |  | [optional] 
**LicenseNumber** | Pointer to **string** |  | [optional] 
**Qualifications** | Pointer to **[]string** |  | [optional] 
**IsHeadKitman** | Pointer to **bool** |  | [optional] 
**Responsibilities** | Pointer to **[]string** |  | [optional] 

## Methods

### NewUpdates

`func NewUpdates() *Updates`

NewUpdates instantiates a new Updates object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdatesWithDefaults

`func NewUpdatesWithDefaults() *Updates`

NewUpdatesWithDefaults instantiates a new Updates object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAssists

`func (o *Updates) GetAssists() int32`

GetAssists returns the Assists field if non-nil, zero value otherwise.

### GetAssistsOk

`func (o *Updates) GetAssistsOk() (*int32, bool)`

GetAssistsOk returns a tuple with the Assists field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssists

`func (o *Updates) SetAssists(v int32)`

SetAssists sets Assists field to given value.

### HasAssists

`func (o *Updates) HasAssists() bool`

HasAssists returns a boolean if a field has been set.

### GetGoalsScored

`func (o *Updates) GetGoalsScored() int32`

GetGoalsScored returns the GoalsScored field if non-nil, zero value otherwise.

### GetGoalsScoredOk

`func (o *Updates) GetGoalsScoredOk() (*int32, bool)`

GetGoalsScoredOk returns a tuple with the GoalsScored field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGoalsScored

`func (o *Updates) SetGoalsScored(v int32)`

SetGoalsScored sets GoalsScored field to given value.

### HasGoalsScored

`func (o *Updates) HasGoalsScored() bool`

HasGoalsScored returns a boolean if a field has been set.

### GetIsCaptain

`func (o *Updates) GetIsCaptain() bool`

GetIsCaptain returns the IsCaptain field if non-nil, zero value otherwise.

### GetIsCaptainOk

`func (o *Updates) GetIsCaptainOk() (*bool, bool)`

GetIsCaptainOk returns a tuple with the IsCaptain field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsCaptain

`func (o *Updates) SetIsCaptain(v bool)`

SetIsCaptain sets IsCaptain field to given value.

### HasIsCaptain

`func (o *Updates) HasIsCaptain() bool`

HasIsCaptain returns a boolean if a field has been set.

### GetJerseyNumber

`func (o *Updates) GetJerseyNumber() int32`

GetJerseyNumber returns the JerseyNumber field if non-nil, zero value otherwise.

### GetJerseyNumberOk

`func (o *Updates) GetJerseyNumberOk() (*int32, bool)`

GetJerseyNumberOk returns a tuple with the JerseyNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJerseyNumber

`func (o *Updates) SetJerseyNumber(v int32)`

SetJerseyNumber sets JerseyNumber field to given value.

### HasJerseyNumber

`func (o *Updates) HasJerseyNumber() bool`

HasJerseyNumber returns a boolean if a field has been set.

### GetPosition

`func (o *Updates) GetPosition() Position`

GetPosition returns the Position field if non-nil, zero value otherwise.

### GetPositionOk

`func (o *Updates) GetPositionOk() (*Position, bool)`

GetPositionOk returns a tuple with the Position field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPosition

`func (o *Updates) SetPosition(v Position)`

SetPosition sets Position field to given value.

### HasPosition

`func (o *Updates) HasPosition() bool`

HasPosition returns a boolean if a field has been set.

### GetTeamId

`func (o *Updates) GetTeamId() string`

GetTeamId returns the TeamId field if non-nil, zero value otherwise.

### GetTeamIdOk

`func (o *Updates) GetTeamIdOk() (*string, bool)`

GetTeamIdOk returns a tuple with the TeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamId

`func (o *Updates) SetTeamId(v string)`

SetTeamId sets TeamId field to given value.

### HasTeamId

`func (o *Updates) HasTeamId() bool`

HasTeamId returns a boolean if a field has been set.

### GetYearsWithTeam

`func (o *Updates) GetYearsWithTeam() int32`

GetYearsWithTeam returns the YearsWithTeam field if non-nil, zero value otherwise.

### GetYearsWithTeamOk

`func (o *Updates) GetYearsWithTeamOk() (*int32, bool)`

GetYearsWithTeamOk returns a tuple with the YearsWithTeam field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetYearsWithTeam

`func (o *Updates) SetYearsWithTeam(v int32)`

SetYearsWithTeam sets YearsWithTeam field to given value.

### HasYearsWithTeam

`func (o *Updates) HasYearsWithTeam() bool`

HasYearsWithTeam returns a boolean if a field has been set.

### GetCertifications

`func (o *Updates) GetCertifications() []string`

GetCertifications returns the Certifications field if non-nil, zero value otherwise.

### GetCertificationsOk

`func (o *Updates) GetCertificationsOk() (*[]string, bool)`

GetCertificationsOk returns a tuple with the Certifications field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCertifications

`func (o *Updates) SetCertifications(v []string)`

SetCertifications sets Certifications field to given value.

### HasCertifications

`func (o *Updates) HasCertifications() bool`

HasCertifications returns a boolean if a field has been set.

### GetSpecialty

`func (o *Updates) GetSpecialty() MedicalSpecialty`

GetSpecialty returns the Specialty field if non-nil, zero value otherwise.

### GetSpecialtyOk

`func (o *Updates) GetSpecialtyOk() (*MedicalSpecialty, bool)`

GetSpecialtyOk returns a tuple with the Specialty field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSpecialty

`func (o *Updates) SetSpecialty(v MedicalSpecialty)`

SetSpecialty sets Specialty field to given value.

### HasSpecialty

`func (o *Updates) HasSpecialty() bool`

HasSpecialty returns a boolean if a field has been set.

### GetWinRate

`func (o *Updates) GetWinRate() float32`

GetWinRate returns the WinRate field if non-nil, zero value otherwise.

### GetWinRateOk

`func (o *Updates) GetWinRateOk() (*float32, bool)`

GetWinRateOk returns a tuple with the WinRate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWinRate

`func (o *Updates) SetWinRate(v float32)`

SetWinRate sets WinRate field to given value.

### HasWinRate

`func (o *Updates) HasWinRate() bool`

HasWinRate returns a boolean if a field has been set.

### GetLicenseNumber

`func (o *Updates) GetLicenseNumber() string`

GetLicenseNumber returns the LicenseNumber field if non-nil, zero value otherwise.

### GetLicenseNumberOk

`func (o *Updates) GetLicenseNumberOk() (*string, bool)`

GetLicenseNumberOk returns a tuple with the LicenseNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLicenseNumber

`func (o *Updates) SetLicenseNumber(v string)`

SetLicenseNumber sets LicenseNumber field to given value.

### HasLicenseNumber

`func (o *Updates) HasLicenseNumber() bool`

HasLicenseNumber returns a boolean if a field has been set.

### GetQualifications

`func (o *Updates) GetQualifications() []string`

GetQualifications returns the Qualifications field if non-nil, zero value otherwise.

### GetQualificationsOk

`func (o *Updates) GetQualificationsOk() (*[]string, bool)`

GetQualificationsOk returns a tuple with the Qualifications field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQualifications

`func (o *Updates) SetQualifications(v []string)`

SetQualifications sets Qualifications field to given value.

### HasQualifications

`func (o *Updates) HasQualifications() bool`

HasQualifications returns a boolean if a field has been set.

### GetIsHeadKitman

`func (o *Updates) GetIsHeadKitman() bool`

GetIsHeadKitman returns the IsHeadKitman field if non-nil, zero value otherwise.

### GetIsHeadKitmanOk

`func (o *Updates) GetIsHeadKitmanOk() (*bool, bool)`

GetIsHeadKitmanOk returns a tuple with the IsHeadKitman field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsHeadKitman

`func (o *Updates) SetIsHeadKitman(v bool)`

SetIsHeadKitman sets IsHeadKitman field to given value.

### HasIsHeadKitman

`func (o *Updates) HasIsHeadKitman() bool`

HasIsHeadKitman returns a boolean if a field has been set.

### GetResponsibilities

`func (o *Updates) GetResponsibilities() []string`

GetResponsibilities returns the Responsibilities field if non-nil, zero value otherwise.

### GetResponsibilitiesOk

`func (o *Updates) GetResponsibilitiesOk() (*[]string, bool)`

GetResponsibilitiesOk returns a tuple with the Responsibilities field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponsibilities

`func (o *Updates) SetResponsibilities(v []string)`

SetResponsibilities sets Responsibilities field to given value.

### HasResponsibilities

`func (o *Updates) HasResponsibilities() bool`

HasResponsibilities returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


