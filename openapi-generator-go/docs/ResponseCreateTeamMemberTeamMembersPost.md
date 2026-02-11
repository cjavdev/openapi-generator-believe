# ResponseCreateTeamMemberTeamMembersPost

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

### NewResponseCreateTeamMemberTeamMembersPost

`func NewResponseCreateTeamMemberTeamMembersPost(characterId string, id string, jerseyNumber int32, position Position, teamId string, yearsWithTeam int32, specialty MedicalSpecialty, ) *ResponseCreateTeamMemberTeamMembersPost`

NewResponseCreateTeamMemberTeamMembersPost instantiates a new ResponseCreateTeamMemberTeamMembersPost object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewResponseCreateTeamMemberTeamMembersPostWithDefaults

`func NewResponseCreateTeamMemberTeamMembersPostWithDefaults() *ResponseCreateTeamMemberTeamMembersPost`

NewResponseCreateTeamMemberTeamMembersPostWithDefaults instantiates a new ResponseCreateTeamMemberTeamMembersPost object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAssists

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetAssists() int32`

GetAssists returns the Assists field if non-nil, zero value otherwise.

### GetAssistsOk

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetAssistsOk() (*int32, bool)`

GetAssistsOk returns a tuple with the Assists field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssists

`func (o *ResponseCreateTeamMemberTeamMembersPost) SetAssists(v int32)`

SetAssists sets Assists field to given value.

### HasAssists

`func (o *ResponseCreateTeamMemberTeamMembersPost) HasAssists() bool`

HasAssists returns a boolean if a field has been set.

### GetCharacterId

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetCharacterId() string`

GetCharacterId returns the CharacterId field if non-nil, zero value otherwise.

### GetCharacterIdOk

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetCharacterIdOk() (*string, bool)`

GetCharacterIdOk returns a tuple with the CharacterId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCharacterId

`func (o *ResponseCreateTeamMemberTeamMembersPost) SetCharacterId(v string)`

SetCharacterId sets CharacterId field to given value.


### GetGoalsScored

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetGoalsScored() int32`

GetGoalsScored returns the GoalsScored field if non-nil, zero value otherwise.

### GetGoalsScoredOk

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetGoalsScoredOk() (*int32, bool)`

GetGoalsScoredOk returns a tuple with the GoalsScored field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGoalsScored

`func (o *ResponseCreateTeamMemberTeamMembersPost) SetGoalsScored(v int32)`

SetGoalsScored sets GoalsScored field to given value.

### HasGoalsScored

`func (o *ResponseCreateTeamMemberTeamMembersPost) HasGoalsScored() bool`

HasGoalsScored returns a boolean if a field has been set.

### GetId

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ResponseCreateTeamMemberTeamMembersPost) SetId(v string)`

SetId sets Id field to given value.


### GetIsCaptain

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetIsCaptain() bool`

GetIsCaptain returns the IsCaptain field if non-nil, zero value otherwise.

### GetIsCaptainOk

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetIsCaptainOk() (*bool, bool)`

GetIsCaptainOk returns a tuple with the IsCaptain field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsCaptain

`func (o *ResponseCreateTeamMemberTeamMembersPost) SetIsCaptain(v bool)`

SetIsCaptain sets IsCaptain field to given value.

### HasIsCaptain

`func (o *ResponseCreateTeamMemberTeamMembersPost) HasIsCaptain() bool`

HasIsCaptain returns a boolean if a field has been set.

### GetJerseyNumber

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetJerseyNumber() int32`

GetJerseyNumber returns the JerseyNumber field if non-nil, zero value otherwise.

### GetJerseyNumberOk

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetJerseyNumberOk() (*int32, bool)`

GetJerseyNumberOk returns a tuple with the JerseyNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJerseyNumber

`func (o *ResponseCreateTeamMemberTeamMembersPost) SetJerseyNumber(v int32)`

SetJerseyNumber sets JerseyNumber field to given value.


### GetMemberType

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetMemberType() string`

GetMemberType returns the MemberType field if non-nil, zero value otherwise.

### GetMemberTypeOk

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetMemberTypeOk() (*string, bool)`

GetMemberTypeOk returns a tuple with the MemberType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMemberType

`func (o *ResponseCreateTeamMemberTeamMembersPost) SetMemberType(v string)`

SetMemberType sets MemberType field to given value.

### HasMemberType

`func (o *ResponseCreateTeamMemberTeamMembersPost) HasMemberType() bool`

HasMemberType returns a boolean if a field has been set.

### GetPosition

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetPosition() Position`

GetPosition returns the Position field if non-nil, zero value otherwise.

### GetPositionOk

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetPositionOk() (*Position, bool)`

GetPositionOk returns a tuple with the Position field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPosition

`func (o *ResponseCreateTeamMemberTeamMembersPost) SetPosition(v Position)`

SetPosition sets Position field to given value.


### GetTeamId

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetTeamId() string`

GetTeamId returns the TeamId field if non-nil, zero value otherwise.

### GetTeamIdOk

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetTeamIdOk() (*string, bool)`

GetTeamIdOk returns a tuple with the TeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamId

`func (o *ResponseCreateTeamMemberTeamMembersPost) SetTeamId(v string)`

SetTeamId sets TeamId field to given value.


### GetYearsWithTeam

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetYearsWithTeam() int32`

GetYearsWithTeam returns the YearsWithTeam field if non-nil, zero value otherwise.

### GetYearsWithTeamOk

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetYearsWithTeamOk() (*int32, bool)`

GetYearsWithTeamOk returns a tuple with the YearsWithTeam field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetYearsWithTeam

`func (o *ResponseCreateTeamMemberTeamMembersPost) SetYearsWithTeam(v int32)`

SetYearsWithTeam sets YearsWithTeam field to given value.


### GetCertifications

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetCertifications() []string`

GetCertifications returns the Certifications field if non-nil, zero value otherwise.

### GetCertificationsOk

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetCertificationsOk() (*[]string, bool)`

GetCertificationsOk returns a tuple with the Certifications field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCertifications

`func (o *ResponseCreateTeamMemberTeamMembersPost) SetCertifications(v []string)`

SetCertifications sets Certifications field to given value.

### HasCertifications

`func (o *ResponseCreateTeamMemberTeamMembersPost) HasCertifications() bool`

HasCertifications returns a boolean if a field has been set.

### GetSpecialty

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetSpecialty() MedicalSpecialty`

GetSpecialty returns the Specialty field if non-nil, zero value otherwise.

### GetSpecialtyOk

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetSpecialtyOk() (*MedicalSpecialty, bool)`

GetSpecialtyOk returns a tuple with the Specialty field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSpecialty

`func (o *ResponseCreateTeamMemberTeamMembersPost) SetSpecialty(v MedicalSpecialty)`

SetSpecialty sets Specialty field to given value.


### GetWinRate

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetWinRate() float32`

GetWinRate returns the WinRate field if non-nil, zero value otherwise.

### GetWinRateOk

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetWinRateOk() (*float32, bool)`

GetWinRateOk returns a tuple with the WinRate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWinRate

`func (o *ResponseCreateTeamMemberTeamMembersPost) SetWinRate(v float32)`

SetWinRate sets WinRate field to given value.

### HasWinRate

`func (o *ResponseCreateTeamMemberTeamMembersPost) HasWinRate() bool`

HasWinRate returns a boolean if a field has been set.

### GetLicenseNumber

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetLicenseNumber() string`

GetLicenseNumber returns the LicenseNumber field if non-nil, zero value otherwise.

### GetLicenseNumberOk

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetLicenseNumberOk() (*string, bool)`

GetLicenseNumberOk returns a tuple with the LicenseNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLicenseNumber

`func (o *ResponseCreateTeamMemberTeamMembersPost) SetLicenseNumber(v string)`

SetLicenseNumber sets LicenseNumber field to given value.

### HasLicenseNumber

`func (o *ResponseCreateTeamMemberTeamMembersPost) HasLicenseNumber() bool`

HasLicenseNumber returns a boolean if a field has been set.

### GetQualifications

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetQualifications() []string`

GetQualifications returns the Qualifications field if non-nil, zero value otherwise.

### GetQualificationsOk

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetQualificationsOk() (*[]string, bool)`

GetQualificationsOk returns a tuple with the Qualifications field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQualifications

`func (o *ResponseCreateTeamMemberTeamMembersPost) SetQualifications(v []string)`

SetQualifications sets Qualifications field to given value.

### HasQualifications

`func (o *ResponseCreateTeamMemberTeamMembersPost) HasQualifications() bool`

HasQualifications returns a boolean if a field has been set.

### GetIsHeadKitman

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetIsHeadKitman() bool`

GetIsHeadKitman returns the IsHeadKitman field if non-nil, zero value otherwise.

### GetIsHeadKitmanOk

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetIsHeadKitmanOk() (*bool, bool)`

GetIsHeadKitmanOk returns a tuple with the IsHeadKitman field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsHeadKitman

`func (o *ResponseCreateTeamMemberTeamMembersPost) SetIsHeadKitman(v bool)`

SetIsHeadKitman sets IsHeadKitman field to given value.

### HasIsHeadKitman

`func (o *ResponseCreateTeamMemberTeamMembersPost) HasIsHeadKitman() bool`

HasIsHeadKitman returns a boolean if a field has been set.

### GetResponsibilities

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetResponsibilities() []string`

GetResponsibilities returns the Responsibilities field if non-nil, zero value otherwise.

### GetResponsibilitiesOk

`func (o *ResponseCreateTeamMemberTeamMembersPost) GetResponsibilitiesOk() (*[]string, bool)`

GetResponsibilitiesOk returns a tuple with the Responsibilities field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponsibilities

`func (o *ResponseCreateTeamMemberTeamMembersPost) SetResponsibilities(v []string)`

SetResponsibilities sets Responsibilities field to given value.

### HasResponsibilities

`func (o *ResponseCreateTeamMemberTeamMembersPost) HasResponsibilities() bool`

HasResponsibilities returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


