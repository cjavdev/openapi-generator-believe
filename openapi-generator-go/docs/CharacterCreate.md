# CharacterCreate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Background** | **string** | Character background and history | 
**DateOfBirth** | Pointer to **NullableString** |  | [optional] 
**Email** | Pointer to **NullableString** |  | [optional] 
**EmotionalStats** | [**EmotionalStats**](EmotionalStats.md) | Emotional intelligence stats | 
**GrowthArcs** | Pointer to [**[]GrowthArc**](GrowthArc.md) | Character development across seasons | [optional] 
**HeightMeters** | Pointer to **NullableFloat32** |  | [optional] 
**Name** | **string** | Character&#39;s full name | 
**PersonalityTraits** | **[]string** | Key personality traits | 
**ProfileImageUrl** | Pointer to **NullableString** |  | [optional] 
**Role** | [**CharacterRole**](CharacterRole.md) | Character&#39;s role | 
**SalaryGbp** | Pointer to [**NullableSalaryGbp**](SalaryGbp.md) |  | [optional] 
**SignatureQuotes** | Pointer to **[]string** | Memorable quotes from this character | [optional] 
**TeamId** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewCharacterCreate

`func NewCharacterCreate(background string, emotionalStats EmotionalStats, name string, personalityTraits []string, role CharacterRole, ) *CharacterCreate`

NewCharacterCreate instantiates a new CharacterCreate object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCharacterCreateWithDefaults

`func NewCharacterCreateWithDefaults() *CharacterCreate`

NewCharacterCreateWithDefaults instantiates a new CharacterCreate object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBackground

`func (o *CharacterCreate) GetBackground() string`

GetBackground returns the Background field if non-nil, zero value otherwise.

### GetBackgroundOk

`func (o *CharacterCreate) GetBackgroundOk() (*string, bool)`

GetBackgroundOk returns a tuple with the Background field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBackground

`func (o *CharacterCreate) SetBackground(v string)`

SetBackground sets Background field to given value.


### GetDateOfBirth

`func (o *CharacterCreate) GetDateOfBirth() string`

GetDateOfBirth returns the DateOfBirth field if non-nil, zero value otherwise.

### GetDateOfBirthOk

`func (o *CharacterCreate) GetDateOfBirthOk() (*string, bool)`

GetDateOfBirthOk returns a tuple with the DateOfBirth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateOfBirth

`func (o *CharacterCreate) SetDateOfBirth(v string)`

SetDateOfBirth sets DateOfBirth field to given value.

### HasDateOfBirth

`func (o *CharacterCreate) HasDateOfBirth() bool`

HasDateOfBirth returns a boolean if a field has been set.

### SetDateOfBirthNil

`func (o *CharacterCreate) SetDateOfBirthNil(b bool)`

 SetDateOfBirthNil sets the value for DateOfBirth to be an explicit nil

### UnsetDateOfBirth
`func (o *CharacterCreate) UnsetDateOfBirth()`

UnsetDateOfBirth ensures that no value is present for DateOfBirth, not even an explicit nil
### GetEmail

`func (o *CharacterCreate) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *CharacterCreate) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *CharacterCreate) SetEmail(v string)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *CharacterCreate) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### SetEmailNil

`func (o *CharacterCreate) SetEmailNil(b bool)`

 SetEmailNil sets the value for Email to be an explicit nil

### UnsetEmail
`func (o *CharacterCreate) UnsetEmail()`

UnsetEmail ensures that no value is present for Email, not even an explicit nil
### GetEmotionalStats

`func (o *CharacterCreate) GetEmotionalStats() EmotionalStats`

GetEmotionalStats returns the EmotionalStats field if non-nil, zero value otherwise.

### GetEmotionalStatsOk

`func (o *CharacterCreate) GetEmotionalStatsOk() (*EmotionalStats, bool)`

GetEmotionalStatsOk returns a tuple with the EmotionalStats field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmotionalStats

`func (o *CharacterCreate) SetEmotionalStats(v EmotionalStats)`

SetEmotionalStats sets EmotionalStats field to given value.


### GetGrowthArcs

`func (o *CharacterCreate) GetGrowthArcs() []GrowthArc`

GetGrowthArcs returns the GrowthArcs field if non-nil, zero value otherwise.

### GetGrowthArcsOk

`func (o *CharacterCreate) GetGrowthArcsOk() (*[]GrowthArc, bool)`

GetGrowthArcsOk returns a tuple with the GrowthArcs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGrowthArcs

`func (o *CharacterCreate) SetGrowthArcs(v []GrowthArc)`

SetGrowthArcs sets GrowthArcs field to given value.

### HasGrowthArcs

`func (o *CharacterCreate) HasGrowthArcs() bool`

HasGrowthArcs returns a boolean if a field has been set.

### GetHeightMeters

`func (o *CharacterCreate) GetHeightMeters() float32`

GetHeightMeters returns the HeightMeters field if non-nil, zero value otherwise.

### GetHeightMetersOk

`func (o *CharacterCreate) GetHeightMetersOk() (*float32, bool)`

GetHeightMetersOk returns a tuple with the HeightMeters field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeightMeters

`func (o *CharacterCreate) SetHeightMeters(v float32)`

SetHeightMeters sets HeightMeters field to given value.

### HasHeightMeters

`func (o *CharacterCreate) HasHeightMeters() bool`

HasHeightMeters returns a boolean if a field has been set.

### SetHeightMetersNil

`func (o *CharacterCreate) SetHeightMetersNil(b bool)`

 SetHeightMetersNil sets the value for HeightMeters to be an explicit nil

### UnsetHeightMeters
`func (o *CharacterCreate) UnsetHeightMeters()`

UnsetHeightMeters ensures that no value is present for HeightMeters, not even an explicit nil
### GetName

`func (o *CharacterCreate) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CharacterCreate) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CharacterCreate) SetName(v string)`

SetName sets Name field to given value.


### GetPersonalityTraits

`func (o *CharacterCreate) GetPersonalityTraits() []string`

GetPersonalityTraits returns the PersonalityTraits field if non-nil, zero value otherwise.

### GetPersonalityTraitsOk

`func (o *CharacterCreate) GetPersonalityTraitsOk() (*[]string, bool)`

GetPersonalityTraitsOk returns a tuple with the PersonalityTraits field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPersonalityTraits

`func (o *CharacterCreate) SetPersonalityTraits(v []string)`

SetPersonalityTraits sets PersonalityTraits field to given value.


### GetProfileImageUrl

`func (o *CharacterCreate) GetProfileImageUrl() string`

GetProfileImageUrl returns the ProfileImageUrl field if non-nil, zero value otherwise.

### GetProfileImageUrlOk

`func (o *CharacterCreate) GetProfileImageUrlOk() (*string, bool)`

GetProfileImageUrlOk returns a tuple with the ProfileImageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProfileImageUrl

`func (o *CharacterCreate) SetProfileImageUrl(v string)`

SetProfileImageUrl sets ProfileImageUrl field to given value.

### HasProfileImageUrl

`func (o *CharacterCreate) HasProfileImageUrl() bool`

HasProfileImageUrl returns a boolean if a field has been set.

### SetProfileImageUrlNil

`func (o *CharacterCreate) SetProfileImageUrlNil(b bool)`

 SetProfileImageUrlNil sets the value for ProfileImageUrl to be an explicit nil

### UnsetProfileImageUrl
`func (o *CharacterCreate) UnsetProfileImageUrl()`

UnsetProfileImageUrl ensures that no value is present for ProfileImageUrl, not even an explicit nil
### GetRole

`func (o *CharacterCreate) GetRole() CharacterRole`

GetRole returns the Role field if non-nil, zero value otherwise.

### GetRoleOk

`func (o *CharacterCreate) GetRoleOk() (*CharacterRole, bool)`

GetRoleOk returns a tuple with the Role field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRole

`func (o *CharacterCreate) SetRole(v CharacterRole)`

SetRole sets Role field to given value.


### GetSalaryGbp

`func (o *CharacterCreate) GetSalaryGbp() SalaryGbp`

GetSalaryGbp returns the SalaryGbp field if non-nil, zero value otherwise.

### GetSalaryGbpOk

`func (o *CharacterCreate) GetSalaryGbpOk() (*SalaryGbp, bool)`

GetSalaryGbpOk returns a tuple with the SalaryGbp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSalaryGbp

`func (o *CharacterCreate) SetSalaryGbp(v SalaryGbp)`

SetSalaryGbp sets SalaryGbp field to given value.

### HasSalaryGbp

`func (o *CharacterCreate) HasSalaryGbp() bool`

HasSalaryGbp returns a boolean if a field has been set.

### SetSalaryGbpNil

`func (o *CharacterCreate) SetSalaryGbpNil(b bool)`

 SetSalaryGbpNil sets the value for SalaryGbp to be an explicit nil

### UnsetSalaryGbp
`func (o *CharacterCreate) UnsetSalaryGbp()`

UnsetSalaryGbp ensures that no value is present for SalaryGbp, not even an explicit nil
### GetSignatureQuotes

`func (o *CharacterCreate) GetSignatureQuotes() []string`

GetSignatureQuotes returns the SignatureQuotes field if non-nil, zero value otherwise.

### GetSignatureQuotesOk

`func (o *CharacterCreate) GetSignatureQuotesOk() (*[]string, bool)`

GetSignatureQuotesOk returns a tuple with the SignatureQuotes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSignatureQuotes

`func (o *CharacterCreate) SetSignatureQuotes(v []string)`

SetSignatureQuotes sets SignatureQuotes field to given value.

### HasSignatureQuotes

`func (o *CharacterCreate) HasSignatureQuotes() bool`

HasSignatureQuotes returns a boolean if a field has been set.

### GetTeamId

`func (o *CharacterCreate) GetTeamId() string`

GetTeamId returns the TeamId field if non-nil, zero value otherwise.

### GetTeamIdOk

`func (o *CharacterCreate) GetTeamIdOk() (*string, bool)`

GetTeamIdOk returns a tuple with the TeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamId

`func (o *CharacterCreate) SetTeamId(v string)`

SetTeamId sets TeamId field to given value.

### HasTeamId

`func (o *CharacterCreate) HasTeamId() bool`

HasTeamId returns a boolean if a field has been set.

### SetTeamIdNil

`func (o *CharacterCreate) SetTeamIdNil(b bool)`

 SetTeamIdNil sets the value for TeamId to be an explicit nil

### UnsetTeamId
`func (o *CharacterCreate) UnsetTeamId()`

UnsetTeamId ensures that no value is present for TeamId, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


