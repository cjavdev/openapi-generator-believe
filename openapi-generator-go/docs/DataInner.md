# DataInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Assists** | Pointer to **int32** | Total assists for the team | [optional] [default to 0]
**CharacterId** | **string** | ID of the character (references /characters/{id}) | 
**GoalsScored** | Pointer to **int32** | Total goals scored for the team | [optional] [default to 0]
**Id** | **string** | Unique identifier for this team membership | 
**IsCaptain** | Pointer to **bool** | Whether this player is team captain | [optional] [default to false]
**JerseyNumber** | **int32** | Jersey/shirt number | 
**MemberType** | Pointer to **string** | Discriminator field indicating this is an equipment manager | [optional] [default to "equipment_manager"]
**Position** | [**Position**](Position.md) | Playing position on the field | 
**TeamId** | **string** | ID of the team they belong to | 
**YearsWithTeam** | **int32** | Number of years with the current team | 
**Certifications** | Pointer to **[]string** | Coaching certifications and licenses | [optional] 
**Specialty** | [**MedicalSpecialty**](MedicalSpecialty.md) | Medical specialty | 
**WinRate** | Pointer to **float32** |  | [optional] 
**LicenseNumber** | Pointer to **string** |  | [optional] 
**Qualifications** | Pointer to **[]string** | Medical qualifications and degrees | [optional] 
**IsHeadKitman** | Pointer to **bool** | Whether this is the head equipment manager | [optional] [default to false]
**Responsibilities** | Pointer to **[]string** | List of responsibilities | [optional] 

## Methods

### NewDataInner

`func NewDataInner(characterId string, id string, jerseyNumber int32, position Position, teamId string, yearsWithTeam int32, specialty MedicalSpecialty, ) *DataInner`

NewDataInner instantiates a new DataInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDataInnerWithDefaults

`func NewDataInnerWithDefaults() *DataInner`

NewDataInnerWithDefaults instantiates a new DataInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAssists

`func (o *DataInner) GetAssists() int32`

GetAssists returns the Assists field if non-nil, zero value otherwise.

### GetAssistsOk

`func (o *DataInner) GetAssistsOk() (*int32, bool)`

GetAssistsOk returns a tuple with the Assists field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssists

`func (o *DataInner) SetAssists(v int32)`

SetAssists sets Assists field to given value.

### HasAssists

`func (o *DataInner) HasAssists() bool`

HasAssists returns a boolean if a field has been set.

### GetCharacterId

`func (o *DataInner) GetCharacterId() string`

GetCharacterId returns the CharacterId field if non-nil, zero value otherwise.

### GetCharacterIdOk

`func (o *DataInner) GetCharacterIdOk() (*string, bool)`

GetCharacterIdOk returns a tuple with the CharacterId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCharacterId

`func (o *DataInner) SetCharacterId(v string)`

SetCharacterId sets CharacterId field to given value.


### GetGoalsScored

`func (o *DataInner) GetGoalsScored() int32`

GetGoalsScored returns the GoalsScored field if non-nil, zero value otherwise.

### GetGoalsScoredOk

`func (o *DataInner) GetGoalsScoredOk() (*int32, bool)`

GetGoalsScoredOk returns a tuple with the GoalsScored field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGoalsScored

`func (o *DataInner) SetGoalsScored(v int32)`

SetGoalsScored sets GoalsScored field to given value.

### HasGoalsScored

`func (o *DataInner) HasGoalsScored() bool`

HasGoalsScored returns a boolean if a field has been set.

### GetId

`func (o *DataInner) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *DataInner) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *DataInner) SetId(v string)`

SetId sets Id field to given value.


### GetIsCaptain

`func (o *DataInner) GetIsCaptain() bool`

GetIsCaptain returns the IsCaptain field if non-nil, zero value otherwise.

### GetIsCaptainOk

`func (o *DataInner) GetIsCaptainOk() (*bool, bool)`

GetIsCaptainOk returns a tuple with the IsCaptain field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsCaptain

`func (o *DataInner) SetIsCaptain(v bool)`

SetIsCaptain sets IsCaptain field to given value.

### HasIsCaptain

`func (o *DataInner) HasIsCaptain() bool`

HasIsCaptain returns a boolean if a field has been set.

### GetJerseyNumber

`func (o *DataInner) GetJerseyNumber() int32`

GetJerseyNumber returns the JerseyNumber field if non-nil, zero value otherwise.

### GetJerseyNumberOk

`func (o *DataInner) GetJerseyNumberOk() (*int32, bool)`

GetJerseyNumberOk returns a tuple with the JerseyNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJerseyNumber

`func (o *DataInner) SetJerseyNumber(v int32)`

SetJerseyNumber sets JerseyNumber field to given value.


### GetMemberType

`func (o *DataInner) GetMemberType() string`

GetMemberType returns the MemberType field if non-nil, zero value otherwise.

### GetMemberTypeOk

`func (o *DataInner) GetMemberTypeOk() (*string, bool)`

GetMemberTypeOk returns a tuple with the MemberType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMemberType

`func (o *DataInner) SetMemberType(v string)`

SetMemberType sets MemberType field to given value.

### HasMemberType

`func (o *DataInner) HasMemberType() bool`

HasMemberType returns a boolean if a field has been set.

### GetPosition

`func (o *DataInner) GetPosition() Position`

GetPosition returns the Position field if non-nil, zero value otherwise.

### GetPositionOk

`func (o *DataInner) GetPositionOk() (*Position, bool)`

GetPositionOk returns a tuple with the Position field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPosition

`func (o *DataInner) SetPosition(v Position)`

SetPosition sets Position field to given value.


### GetTeamId

`func (o *DataInner) GetTeamId() string`

GetTeamId returns the TeamId field if non-nil, zero value otherwise.

### GetTeamIdOk

`func (o *DataInner) GetTeamIdOk() (*string, bool)`

GetTeamIdOk returns a tuple with the TeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamId

`func (o *DataInner) SetTeamId(v string)`

SetTeamId sets TeamId field to given value.


### GetYearsWithTeam

`func (o *DataInner) GetYearsWithTeam() int32`

GetYearsWithTeam returns the YearsWithTeam field if non-nil, zero value otherwise.

### GetYearsWithTeamOk

`func (o *DataInner) GetYearsWithTeamOk() (*int32, bool)`

GetYearsWithTeamOk returns a tuple with the YearsWithTeam field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetYearsWithTeam

`func (o *DataInner) SetYearsWithTeam(v int32)`

SetYearsWithTeam sets YearsWithTeam field to given value.


### GetCertifications

`func (o *DataInner) GetCertifications() []string`

GetCertifications returns the Certifications field if non-nil, zero value otherwise.

### GetCertificationsOk

`func (o *DataInner) GetCertificationsOk() (*[]string, bool)`

GetCertificationsOk returns a tuple with the Certifications field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCertifications

`func (o *DataInner) SetCertifications(v []string)`

SetCertifications sets Certifications field to given value.

### HasCertifications

`func (o *DataInner) HasCertifications() bool`

HasCertifications returns a boolean if a field has been set.

### GetSpecialty

`func (o *DataInner) GetSpecialty() MedicalSpecialty`

GetSpecialty returns the Specialty field if non-nil, zero value otherwise.

### GetSpecialtyOk

`func (o *DataInner) GetSpecialtyOk() (*MedicalSpecialty, bool)`

GetSpecialtyOk returns a tuple with the Specialty field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSpecialty

`func (o *DataInner) SetSpecialty(v MedicalSpecialty)`

SetSpecialty sets Specialty field to given value.


### GetWinRate

`func (o *DataInner) GetWinRate() float32`

GetWinRate returns the WinRate field if non-nil, zero value otherwise.

### GetWinRateOk

`func (o *DataInner) GetWinRateOk() (*float32, bool)`

GetWinRateOk returns a tuple with the WinRate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWinRate

`func (o *DataInner) SetWinRate(v float32)`

SetWinRate sets WinRate field to given value.

### HasWinRate

`func (o *DataInner) HasWinRate() bool`

HasWinRate returns a boolean if a field has been set.

### GetLicenseNumber

`func (o *DataInner) GetLicenseNumber() string`

GetLicenseNumber returns the LicenseNumber field if non-nil, zero value otherwise.

### GetLicenseNumberOk

`func (o *DataInner) GetLicenseNumberOk() (*string, bool)`

GetLicenseNumberOk returns a tuple with the LicenseNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLicenseNumber

`func (o *DataInner) SetLicenseNumber(v string)`

SetLicenseNumber sets LicenseNumber field to given value.

### HasLicenseNumber

`func (o *DataInner) HasLicenseNumber() bool`

HasLicenseNumber returns a boolean if a field has been set.

### GetQualifications

`func (o *DataInner) GetQualifications() []string`

GetQualifications returns the Qualifications field if non-nil, zero value otherwise.

### GetQualificationsOk

`func (o *DataInner) GetQualificationsOk() (*[]string, bool)`

GetQualificationsOk returns a tuple with the Qualifications field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQualifications

`func (o *DataInner) SetQualifications(v []string)`

SetQualifications sets Qualifications field to given value.

### HasQualifications

`func (o *DataInner) HasQualifications() bool`

HasQualifications returns a boolean if a field has been set.

### GetIsHeadKitman

`func (o *DataInner) GetIsHeadKitman() bool`

GetIsHeadKitman returns the IsHeadKitman field if non-nil, zero value otherwise.

### GetIsHeadKitmanOk

`func (o *DataInner) GetIsHeadKitmanOk() (*bool, bool)`

GetIsHeadKitmanOk returns a tuple with the IsHeadKitman field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsHeadKitman

`func (o *DataInner) SetIsHeadKitman(v bool)`

SetIsHeadKitman sets IsHeadKitman field to given value.

### HasIsHeadKitman

`func (o *DataInner) HasIsHeadKitman() bool`

HasIsHeadKitman returns a boolean if a field has been set.

### GetResponsibilities

`func (o *DataInner) GetResponsibilities() []string`

GetResponsibilities returns the Responsibilities field if non-nil, zero value otherwise.

### GetResponsibilitiesOk

`func (o *DataInner) GetResponsibilitiesOk() (*[]string, bool)`

GetResponsibilitiesOk returns a tuple with the Responsibilities field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponsibilities

`func (o *DataInner) SetResponsibilities(v []string)`

SetResponsibilities sets Responsibilities field to given value.

### HasResponsibilities

`func (o *DataInner) HasResponsibilities() bool`

HasResponsibilities returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


