# CharacterUpdate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Background** | Pointer to **NullableString** |  | [optional] 
**DateOfBirth** | Pointer to **NullableString** |  | [optional] 
**Email** | Pointer to **NullableString** |  | [optional] 
**EmotionalStats** | Pointer to [**NullableEmotionalStats**](EmotionalStats.md) |  | [optional] 
**GrowthArcs** | Pointer to [**[]GrowthArc**](GrowthArc.md) |  | [optional] 
**HeightMeters** | Pointer to **NullableFloat32** |  | [optional] 
**Name** | Pointer to **NullableString** |  | [optional] 
**PersonalityTraits** | Pointer to **[]string** |  | [optional] 
**ProfileImageUrl** | Pointer to **NullableString** |  | [optional] 
**Role** | Pointer to [**NullableCharacterRole**](CharacterRole.md) |  | [optional] 
**SalaryGbp** | Pointer to [**NullableSalaryGbp1**](SalaryGbp1.md) |  | [optional] 
**SignatureQuotes** | Pointer to **[]string** |  | [optional] 
**TeamId** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewCharacterUpdate

`func NewCharacterUpdate() *CharacterUpdate`

NewCharacterUpdate instantiates a new CharacterUpdate object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCharacterUpdateWithDefaults

`func NewCharacterUpdateWithDefaults() *CharacterUpdate`

NewCharacterUpdateWithDefaults instantiates a new CharacterUpdate object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBackground

`func (o *CharacterUpdate) GetBackground() string`

GetBackground returns the Background field if non-nil, zero value otherwise.

### GetBackgroundOk

`func (o *CharacterUpdate) GetBackgroundOk() (*string, bool)`

GetBackgroundOk returns a tuple with the Background field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBackground

`func (o *CharacterUpdate) SetBackground(v string)`

SetBackground sets Background field to given value.

### HasBackground

`func (o *CharacterUpdate) HasBackground() bool`

HasBackground returns a boolean if a field has been set.

### SetBackgroundNil

`func (o *CharacterUpdate) SetBackgroundNil(b bool)`

 SetBackgroundNil sets the value for Background to be an explicit nil

### UnsetBackground
`func (o *CharacterUpdate) UnsetBackground()`

UnsetBackground ensures that no value is present for Background, not even an explicit nil
### GetDateOfBirth

`func (o *CharacterUpdate) GetDateOfBirth() string`

GetDateOfBirth returns the DateOfBirth field if non-nil, zero value otherwise.

### GetDateOfBirthOk

`func (o *CharacterUpdate) GetDateOfBirthOk() (*string, bool)`

GetDateOfBirthOk returns a tuple with the DateOfBirth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateOfBirth

`func (o *CharacterUpdate) SetDateOfBirth(v string)`

SetDateOfBirth sets DateOfBirth field to given value.

### HasDateOfBirth

`func (o *CharacterUpdate) HasDateOfBirth() bool`

HasDateOfBirth returns a boolean if a field has been set.

### SetDateOfBirthNil

`func (o *CharacterUpdate) SetDateOfBirthNil(b bool)`

 SetDateOfBirthNil sets the value for DateOfBirth to be an explicit nil

### UnsetDateOfBirth
`func (o *CharacterUpdate) UnsetDateOfBirth()`

UnsetDateOfBirth ensures that no value is present for DateOfBirth, not even an explicit nil
### GetEmail

`func (o *CharacterUpdate) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *CharacterUpdate) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *CharacterUpdate) SetEmail(v string)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *CharacterUpdate) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### SetEmailNil

`func (o *CharacterUpdate) SetEmailNil(b bool)`

 SetEmailNil sets the value for Email to be an explicit nil

### UnsetEmail
`func (o *CharacterUpdate) UnsetEmail()`

UnsetEmail ensures that no value is present for Email, not even an explicit nil
### GetEmotionalStats

`func (o *CharacterUpdate) GetEmotionalStats() EmotionalStats`

GetEmotionalStats returns the EmotionalStats field if non-nil, zero value otherwise.

### GetEmotionalStatsOk

`func (o *CharacterUpdate) GetEmotionalStatsOk() (*EmotionalStats, bool)`

GetEmotionalStatsOk returns a tuple with the EmotionalStats field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmotionalStats

`func (o *CharacterUpdate) SetEmotionalStats(v EmotionalStats)`

SetEmotionalStats sets EmotionalStats field to given value.

### HasEmotionalStats

`func (o *CharacterUpdate) HasEmotionalStats() bool`

HasEmotionalStats returns a boolean if a field has been set.

### SetEmotionalStatsNil

`func (o *CharacterUpdate) SetEmotionalStatsNil(b bool)`

 SetEmotionalStatsNil sets the value for EmotionalStats to be an explicit nil

### UnsetEmotionalStats
`func (o *CharacterUpdate) UnsetEmotionalStats()`

UnsetEmotionalStats ensures that no value is present for EmotionalStats, not even an explicit nil
### GetGrowthArcs

`func (o *CharacterUpdate) GetGrowthArcs() []GrowthArc`

GetGrowthArcs returns the GrowthArcs field if non-nil, zero value otherwise.

### GetGrowthArcsOk

`func (o *CharacterUpdate) GetGrowthArcsOk() (*[]GrowthArc, bool)`

GetGrowthArcsOk returns a tuple with the GrowthArcs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGrowthArcs

`func (o *CharacterUpdate) SetGrowthArcs(v []GrowthArc)`

SetGrowthArcs sets GrowthArcs field to given value.

### HasGrowthArcs

`func (o *CharacterUpdate) HasGrowthArcs() bool`

HasGrowthArcs returns a boolean if a field has been set.

### SetGrowthArcsNil

`func (o *CharacterUpdate) SetGrowthArcsNil(b bool)`

 SetGrowthArcsNil sets the value for GrowthArcs to be an explicit nil

### UnsetGrowthArcs
`func (o *CharacterUpdate) UnsetGrowthArcs()`

UnsetGrowthArcs ensures that no value is present for GrowthArcs, not even an explicit nil
### GetHeightMeters

`func (o *CharacterUpdate) GetHeightMeters() float32`

GetHeightMeters returns the HeightMeters field if non-nil, zero value otherwise.

### GetHeightMetersOk

`func (o *CharacterUpdate) GetHeightMetersOk() (*float32, bool)`

GetHeightMetersOk returns a tuple with the HeightMeters field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeightMeters

`func (o *CharacterUpdate) SetHeightMeters(v float32)`

SetHeightMeters sets HeightMeters field to given value.

### HasHeightMeters

`func (o *CharacterUpdate) HasHeightMeters() bool`

HasHeightMeters returns a boolean if a field has been set.

### SetHeightMetersNil

`func (o *CharacterUpdate) SetHeightMetersNil(b bool)`

 SetHeightMetersNil sets the value for HeightMeters to be an explicit nil

### UnsetHeightMeters
`func (o *CharacterUpdate) UnsetHeightMeters()`

UnsetHeightMeters ensures that no value is present for HeightMeters, not even an explicit nil
### GetName

`func (o *CharacterUpdate) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CharacterUpdate) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CharacterUpdate) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *CharacterUpdate) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *CharacterUpdate) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *CharacterUpdate) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetPersonalityTraits

`func (o *CharacterUpdate) GetPersonalityTraits() []string`

GetPersonalityTraits returns the PersonalityTraits field if non-nil, zero value otherwise.

### GetPersonalityTraitsOk

`func (o *CharacterUpdate) GetPersonalityTraitsOk() (*[]string, bool)`

GetPersonalityTraitsOk returns a tuple with the PersonalityTraits field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPersonalityTraits

`func (o *CharacterUpdate) SetPersonalityTraits(v []string)`

SetPersonalityTraits sets PersonalityTraits field to given value.

### HasPersonalityTraits

`func (o *CharacterUpdate) HasPersonalityTraits() bool`

HasPersonalityTraits returns a boolean if a field has been set.

### SetPersonalityTraitsNil

`func (o *CharacterUpdate) SetPersonalityTraitsNil(b bool)`

 SetPersonalityTraitsNil sets the value for PersonalityTraits to be an explicit nil

### UnsetPersonalityTraits
`func (o *CharacterUpdate) UnsetPersonalityTraits()`

UnsetPersonalityTraits ensures that no value is present for PersonalityTraits, not even an explicit nil
### GetProfileImageUrl

`func (o *CharacterUpdate) GetProfileImageUrl() string`

GetProfileImageUrl returns the ProfileImageUrl field if non-nil, zero value otherwise.

### GetProfileImageUrlOk

`func (o *CharacterUpdate) GetProfileImageUrlOk() (*string, bool)`

GetProfileImageUrlOk returns a tuple with the ProfileImageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProfileImageUrl

`func (o *CharacterUpdate) SetProfileImageUrl(v string)`

SetProfileImageUrl sets ProfileImageUrl field to given value.

### HasProfileImageUrl

`func (o *CharacterUpdate) HasProfileImageUrl() bool`

HasProfileImageUrl returns a boolean if a field has been set.

### SetProfileImageUrlNil

`func (o *CharacterUpdate) SetProfileImageUrlNil(b bool)`

 SetProfileImageUrlNil sets the value for ProfileImageUrl to be an explicit nil

### UnsetProfileImageUrl
`func (o *CharacterUpdate) UnsetProfileImageUrl()`

UnsetProfileImageUrl ensures that no value is present for ProfileImageUrl, not even an explicit nil
### GetRole

`func (o *CharacterUpdate) GetRole() CharacterRole`

GetRole returns the Role field if non-nil, zero value otherwise.

### GetRoleOk

`func (o *CharacterUpdate) GetRoleOk() (*CharacterRole, bool)`

GetRoleOk returns a tuple with the Role field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRole

`func (o *CharacterUpdate) SetRole(v CharacterRole)`

SetRole sets Role field to given value.

### HasRole

`func (o *CharacterUpdate) HasRole() bool`

HasRole returns a boolean if a field has been set.

### SetRoleNil

`func (o *CharacterUpdate) SetRoleNil(b bool)`

 SetRoleNil sets the value for Role to be an explicit nil

### UnsetRole
`func (o *CharacterUpdate) UnsetRole()`

UnsetRole ensures that no value is present for Role, not even an explicit nil
### GetSalaryGbp

`func (o *CharacterUpdate) GetSalaryGbp() SalaryGbp1`

GetSalaryGbp returns the SalaryGbp field if non-nil, zero value otherwise.

### GetSalaryGbpOk

`func (o *CharacterUpdate) GetSalaryGbpOk() (*SalaryGbp1, bool)`

GetSalaryGbpOk returns a tuple with the SalaryGbp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSalaryGbp

`func (o *CharacterUpdate) SetSalaryGbp(v SalaryGbp1)`

SetSalaryGbp sets SalaryGbp field to given value.

### HasSalaryGbp

`func (o *CharacterUpdate) HasSalaryGbp() bool`

HasSalaryGbp returns a boolean if a field has been set.

### SetSalaryGbpNil

`func (o *CharacterUpdate) SetSalaryGbpNil(b bool)`

 SetSalaryGbpNil sets the value for SalaryGbp to be an explicit nil

### UnsetSalaryGbp
`func (o *CharacterUpdate) UnsetSalaryGbp()`

UnsetSalaryGbp ensures that no value is present for SalaryGbp, not even an explicit nil
### GetSignatureQuotes

`func (o *CharacterUpdate) GetSignatureQuotes() []string`

GetSignatureQuotes returns the SignatureQuotes field if non-nil, zero value otherwise.

### GetSignatureQuotesOk

`func (o *CharacterUpdate) GetSignatureQuotesOk() (*[]string, bool)`

GetSignatureQuotesOk returns a tuple with the SignatureQuotes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSignatureQuotes

`func (o *CharacterUpdate) SetSignatureQuotes(v []string)`

SetSignatureQuotes sets SignatureQuotes field to given value.

### HasSignatureQuotes

`func (o *CharacterUpdate) HasSignatureQuotes() bool`

HasSignatureQuotes returns a boolean if a field has been set.

### SetSignatureQuotesNil

`func (o *CharacterUpdate) SetSignatureQuotesNil(b bool)`

 SetSignatureQuotesNil sets the value for SignatureQuotes to be an explicit nil

### UnsetSignatureQuotes
`func (o *CharacterUpdate) UnsetSignatureQuotes()`

UnsetSignatureQuotes ensures that no value is present for SignatureQuotes, not even an explicit nil
### GetTeamId

`func (o *CharacterUpdate) GetTeamId() string`

GetTeamId returns the TeamId field if non-nil, zero value otherwise.

### GetTeamIdOk

`func (o *CharacterUpdate) GetTeamIdOk() (*string, bool)`

GetTeamIdOk returns a tuple with the TeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamId

`func (o *CharacterUpdate) SetTeamId(v string)`

SetTeamId sets TeamId field to given value.

### HasTeamId

`func (o *CharacterUpdate) HasTeamId() bool`

HasTeamId returns a boolean if a field has been set.

### SetTeamIdNil

`func (o *CharacterUpdate) SetTeamIdNil(b bool)`

 SetTeamIdNil sets the value for TeamId to be an explicit nil

### UnsetTeamId
`func (o *CharacterUpdate) UnsetTeamId()`

UnsetTeamId ensures that no value is present for TeamId, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


