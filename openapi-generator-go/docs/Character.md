# Character

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Background** | **string** | Character background and history | 
**DateOfBirth** | Pointer to **NullableString** |  | [optional] 
**Email** | Pointer to **NullableString** |  | [optional] 
**EmotionalStats** | [**EmotionalStats**](EmotionalStats.md) | Emotional intelligence stats | 
**GrowthArcs** | Pointer to [**[]GrowthArc**](GrowthArc.md) | Character development across seasons | [optional] 
**HeightMeters** | Pointer to **NullableFloat32** |  | [optional] 
**Id** | **string** | Unique identifier | 
**Name** | **string** | Character&#39;s full name | 
**PersonalityTraits** | **[]string** | Key personality traits | 
**ProfileImageUrl** | Pointer to **NullableString** |  | [optional] 
**Role** | [**CharacterRole**](CharacterRole.md) | Character&#39;s role | 
**SalaryGbp** | Pointer to **NullableString** |  | [optional] 
**SignatureQuotes** | Pointer to **[]string** | Memorable quotes from this character | [optional] 
**TeamId** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewCharacter

`func NewCharacter(background string, emotionalStats EmotionalStats, id string, name string, personalityTraits []string, role CharacterRole, ) *Character`

NewCharacter instantiates a new Character object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCharacterWithDefaults

`func NewCharacterWithDefaults() *Character`

NewCharacterWithDefaults instantiates a new Character object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBackground

`func (o *Character) GetBackground() string`

GetBackground returns the Background field if non-nil, zero value otherwise.

### GetBackgroundOk

`func (o *Character) GetBackgroundOk() (*string, bool)`

GetBackgroundOk returns a tuple with the Background field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBackground

`func (o *Character) SetBackground(v string)`

SetBackground sets Background field to given value.


### GetDateOfBirth

`func (o *Character) GetDateOfBirth() string`

GetDateOfBirth returns the DateOfBirth field if non-nil, zero value otherwise.

### GetDateOfBirthOk

`func (o *Character) GetDateOfBirthOk() (*string, bool)`

GetDateOfBirthOk returns a tuple with the DateOfBirth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateOfBirth

`func (o *Character) SetDateOfBirth(v string)`

SetDateOfBirth sets DateOfBirth field to given value.

### HasDateOfBirth

`func (o *Character) HasDateOfBirth() bool`

HasDateOfBirth returns a boolean if a field has been set.

### SetDateOfBirthNil

`func (o *Character) SetDateOfBirthNil(b bool)`

 SetDateOfBirthNil sets the value for DateOfBirth to be an explicit nil

### UnsetDateOfBirth
`func (o *Character) UnsetDateOfBirth()`

UnsetDateOfBirth ensures that no value is present for DateOfBirth, not even an explicit nil
### GetEmail

`func (o *Character) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *Character) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *Character) SetEmail(v string)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *Character) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### SetEmailNil

`func (o *Character) SetEmailNil(b bool)`

 SetEmailNil sets the value for Email to be an explicit nil

### UnsetEmail
`func (o *Character) UnsetEmail()`

UnsetEmail ensures that no value is present for Email, not even an explicit nil
### GetEmotionalStats

`func (o *Character) GetEmotionalStats() EmotionalStats`

GetEmotionalStats returns the EmotionalStats field if non-nil, zero value otherwise.

### GetEmotionalStatsOk

`func (o *Character) GetEmotionalStatsOk() (*EmotionalStats, bool)`

GetEmotionalStatsOk returns a tuple with the EmotionalStats field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmotionalStats

`func (o *Character) SetEmotionalStats(v EmotionalStats)`

SetEmotionalStats sets EmotionalStats field to given value.


### GetGrowthArcs

`func (o *Character) GetGrowthArcs() []GrowthArc`

GetGrowthArcs returns the GrowthArcs field if non-nil, zero value otherwise.

### GetGrowthArcsOk

`func (o *Character) GetGrowthArcsOk() (*[]GrowthArc, bool)`

GetGrowthArcsOk returns a tuple with the GrowthArcs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGrowthArcs

`func (o *Character) SetGrowthArcs(v []GrowthArc)`

SetGrowthArcs sets GrowthArcs field to given value.

### HasGrowthArcs

`func (o *Character) HasGrowthArcs() bool`

HasGrowthArcs returns a boolean if a field has been set.

### GetHeightMeters

`func (o *Character) GetHeightMeters() float32`

GetHeightMeters returns the HeightMeters field if non-nil, zero value otherwise.

### GetHeightMetersOk

`func (o *Character) GetHeightMetersOk() (*float32, bool)`

GetHeightMetersOk returns a tuple with the HeightMeters field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeightMeters

`func (o *Character) SetHeightMeters(v float32)`

SetHeightMeters sets HeightMeters field to given value.

### HasHeightMeters

`func (o *Character) HasHeightMeters() bool`

HasHeightMeters returns a boolean if a field has been set.

### SetHeightMetersNil

`func (o *Character) SetHeightMetersNil(b bool)`

 SetHeightMetersNil sets the value for HeightMeters to be an explicit nil

### UnsetHeightMeters
`func (o *Character) UnsetHeightMeters()`

UnsetHeightMeters ensures that no value is present for HeightMeters, not even an explicit nil
### GetId

`func (o *Character) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Character) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Character) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *Character) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Character) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Character) SetName(v string)`

SetName sets Name field to given value.


### GetPersonalityTraits

`func (o *Character) GetPersonalityTraits() []string`

GetPersonalityTraits returns the PersonalityTraits field if non-nil, zero value otherwise.

### GetPersonalityTraitsOk

`func (o *Character) GetPersonalityTraitsOk() (*[]string, bool)`

GetPersonalityTraitsOk returns a tuple with the PersonalityTraits field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPersonalityTraits

`func (o *Character) SetPersonalityTraits(v []string)`

SetPersonalityTraits sets PersonalityTraits field to given value.


### GetProfileImageUrl

`func (o *Character) GetProfileImageUrl() string`

GetProfileImageUrl returns the ProfileImageUrl field if non-nil, zero value otherwise.

### GetProfileImageUrlOk

`func (o *Character) GetProfileImageUrlOk() (*string, bool)`

GetProfileImageUrlOk returns a tuple with the ProfileImageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProfileImageUrl

`func (o *Character) SetProfileImageUrl(v string)`

SetProfileImageUrl sets ProfileImageUrl field to given value.

### HasProfileImageUrl

`func (o *Character) HasProfileImageUrl() bool`

HasProfileImageUrl returns a boolean if a field has been set.

### SetProfileImageUrlNil

`func (o *Character) SetProfileImageUrlNil(b bool)`

 SetProfileImageUrlNil sets the value for ProfileImageUrl to be an explicit nil

### UnsetProfileImageUrl
`func (o *Character) UnsetProfileImageUrl()`

UnsetProfileImageUrl ensures that no value is present for ProfileImageUrl, not even an explicit nil
### GetRole

`func (o *Character) GetRole() CharacterRole`

GetRole returns the Role field if non-nil, zero value otherwise.

### GetRoleOk

`func (o *Character) GetRoleOk() (*CharacterRole, bool)`

GetRoleOk returns a tuple with the Role field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRole

`func (o *Character) SetRole(v CharacterRole)`

SetRole sets Role field to given value.


### GetSalaryGbp

`func (o *Character) GetSalaryGbp() string`

GetSalaryGbp returns the SalaryGbp field if non-nil, zero value otherwise.

### GetSalaryGbpOk

`func (o *Character) GetSalaryGbpOk() (*string, bool)`

GetSalaryGbpOk returns a tuple with the SalaryGbp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSalaryGbp

`func (o *Character) SetSalaryGbp(v string)`

SetSalaryGbp sets SalaryGbp field to given value.

### HasSalaryGbp

`func (o *Character) HasSalaryGbp() bool`

HasSalaryGbp returns a boolean if a field has been set.

### SetSalaryGbpNil

`func (o *Character) SetSalaryGbpNil(b bool)`

 SetSalaryGbpNil sets the value for SalaryGbp to be an explicit nil

### UnsetSalaryGbp
`func (o *Character) UnsetSalaryGbp()`

UnsetSalaryGbp ensures that no value is present for SalaryGbp, not even an explicit nil
### GetSignatureQuotes

`func (o *Character) GetSignatureQuotes() []string`

GetSignatureQuotes returns the SignatureQuotes field if non-nil, zero value otherwise.

### GetSignatureQuotesOk

`func (o *Character) GetSignatureQuotesOk() (*[]string, bool)`

GetSignatureQuotesOk returns a tuple with the SignatureQuotes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSignatureQuotes

`func (o *Character) SetSignatureQuotes(v []string)`

SetSignatureQuotes sets SignatureQuotes field to given value.

### HasSignatureQuotes

`func (o *Character) HasSignatureQuotes() bool`

HasSignatureQuotes returns a boolean if a field has been set.

### GetTeamId

`func (o *Character) GetTeamId() string`

GetTeamId returns the TeamId field if non-nil, zero value otherwise.

### GetTeamIdOk

`func (o *Character) GetTeamIdOk() (*string, bool)`

GetTeamIdOk returns a tuple with the TeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamId

`func (o *Character) SetTeamId(v string)`

SetTeamId sets TeamId field to given value.

### HasTeamId

`func (o *Character) HasTeamId() bool`

HasTeamId returns a boolean if a field has been set.

### SetTeamIdNil

`func (o *Character) SetTeamIdNil(b bool)`

 SetTeamIdNil sets the value for TeamId to be an explicit nil

### UnsetTeamId
`func (o *Character) UnsetTeamId()`

UnsetTeamId ensures that no value is present for TeamId, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


