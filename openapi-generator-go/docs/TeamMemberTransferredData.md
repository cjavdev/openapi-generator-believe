# TeamMemberTransferredData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CharacterId** | **string** | ID of the character (links to /characters) | 
**CharacterName** | **string** | Name of the character | 
**MemberType** | **string** | Type of team member | 
**PreviousTeamId** | Pointer to **string** | Previous team ID (for joins from another team) | [optional] 
**PreviousTeamName** | Pointer to **string** | Previous team name (for joins from another team) | [optional] 
**TeamId** | **string** | ID of the team involved | 
**TeamMemberId** | **string** | ID of the team member | 
**TeamName** | **string** | Name of the team involved | 
**TedReaction** | **string** | Ted&#39;s reaction to the transfer | 
**TransferFeeGbp** | Pointer to **string** | Transfer fee in GBP (for players) | [optional] 
**TransferType** | **string** | Whether the member joined or departed | 
**YearsWithPreviousTeam** | Pointer to **int32** | Years spent with previous team | [optional] 

## Methods

### NewTeamMemberTransferredData

`func NewTeamMemberTransferredData(characterId string, characterName string, memberType string, teamId string, teamMemberId string, teamName string, tedReaction string, transferType string, ) *TeamMemberTransferredData`

NewTeamMemberTransferredData instantiates a new TeamMemberTransferredData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTeamMemberTransferredDataWithDefaults

`func NewTeamMemberTransferredDataWithDefaults() *TeamMemberTransferredData`

NewTeamMemberTransferredDataWithDefaults instantiates a new TeamMemberTransferredData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCharacterId

`func (o *TeamMemberTransferredData) GetCharacterId() string`

GetCharacterId returns the CharacterId field if non-nil, zero value otherwise.

### GetCharacterIdOk

`func (o *TeamMemberTransferredData) GetCharacterIdOk() (*string, bool)`

GetCharacterIdOk returns a tuple with the CharacterId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCharacterId

`func (o *TeamMemberTransferredData) SetCharacterId(v string)`

SetCharacterId sets CharacterId field to given value.


### GetCharacterName

`func (o *TeamMemberTransferredData) GetCharacterName() string`

GetCharacterName returns the CharacterName field if non-nil, zero value otherwise.

### GetCharacterNameOk

`func (o *TeamMemberTransferredData) GetCharacterNameOk() (*string, bool)`

GetCharacterNameOk returns a tuple with the CharacterName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCharacterName

`func (o *TeamMemberTransferredData) SetCharacterName(v string)`

SetCharacterName sets CharacterName field to given value.


### GetMemberType

`func (o *TeamMemberTransferredData) GetMemberType() string`

GetMemberType returns the MemberType field if non-nil, zero value otherwise.

### GetMemberTypeOk

`func (o *TeamMemberTransferredData) GetMemberTypeOk() (*string, bool)`

GetMemberTypeOk returns a tuple with the MemberType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMemberType

`func (o *TeamMemberTransferredData) SetMemberType(v string)`

SetMemberType sets MemberType field to given value.


### GetPreviousTeamId

`func (o *TeamMemberTransferredData) GetPreviousTeamId() string`

GetPreviousTeamId returns the PreviousTeamId field if non-nil, zero value otherwise.

### GetPreviousTeamIdOk

`func (o *TeamMemberTransferredData) GetPreviousTeamIdOk() (*string, bool)`

GetPreviousTeamIdOk returns a tuple with the PreviousTeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPreviousTeamId

`func (o *TeamMemberTransferredData) SetPreviousTeamId(v string)`

SetPreviousTeamId sets PreviousTeamId field to given value.

### HasPreviousTeamId

`func (o *TeamMemberTransferredData) HasPreviousTeamId() bool`

HasPreviousTeamId returns a boolean if a field has been set.

### GetPreviousTeamName

`func (o *TeamMemberTransferredData) GetPreviousTeamName() string`

GetPreviousTeamName returns the PreviousTeamName field if non-nil, zero value otherwise.

### GetPreviousTeamNameOk

`func (o *TeamMemberTransferredData) GetPreviousTeamNameOk() (*string, bool)`

GetPreviousTeamNameOk returns a tuple with the PreviousTeamName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPreviousTeamName

`func (o *TeamMemberTransferredData) SetPreviousTeamName(v string)`

SetPreviousTeamName sets PreviousTeamName field to given value.

### HasPreviousTeamName

`func (o *TeamMemberTransferredData) HasPreviousTeamName() bool`

HasPreviousTeamName returns a boolean if a field has been set.

### GetTeamId

`func (o *TeamMemberTransferredData) GetTeamId() string`

GetTeamId returns the TeamId field if non-nil, zero value otherwise.

### GetTeamIdOk

`func (o *TeamMemberTransferredData) GetTeamIdOk() (*string, bool)`

GetTeamIdOk returns a tuple with the TeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamId

`func (o *TeamMemberTransferredData) SetTeamId(v string)`

SetTeamId sets TeamId field to given value.


### GetTeamMemberId

`func (o *TeamMemberTransferredData) GetTeamMemberId() string`

GetTeamMemberId returns the TeamMemberId field if non-nil, zero value otherwise.

### GetTeamMemberIdOk

`func (o *TeamMemberTransferredData) GetTeamMemberIdOk() (*string, bool)`

GetTeamMemberIdOk returns a tuple with the TeamMemberId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamMemberId

`func (o *TeamMemberTransferredData) SetTeamMemberId(v string)`

SetTeamMemberId sets TeamMemberId field to given value.


### GetTeamName

`func (o *TeamMemberTransferredData) GetTeamName() string`

GetTeamName returns the TeamName field if non-nil, zero value otherwise.

### GetTeamNameOk

`func (o *TeamMemberTransferredData) GetTeamNameOk() (*string, bool)`

GetTeamNameOk returns a tuple with the TeamName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamName

`func (o *TeamMemberTransferredData) SetTeamName(v string)`

SetTeamName sets TeamName field to given value.


### GetTedReaction

`func (o *TeamMemberTransferredData) GetTedReaction() string`

GetTedReaction returns the TedReaction field if non-nil, zero value otherwise.

### GetTedReactionOk

`func (o *TeamMemberTransferredData) GetTedReactionOk() (*string, bool)`

GetTedReactionOk returns a tuple with the TedReaction field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTedReaction

`func (o *TeamMemberTransferredData) SetTedReaction(v string)`

SetTedReaction sets TedReaction field to given value.


### GetTransferFeeGbp

`func (o *TeamMemberTransferredData) GetTransferFeeGbp() string`

GetTransferFeeGbp returns the TransferFeeGbp field if non-nil, zero value otherwise.

### GetTransferFeeGbpOk

`func (o *TeamMemberTransferredData) GetTransferFeeGbpOk() (*string, bool)`

GetTransferFeeGbpOk returns a tuple with the TransferFeeGbp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTransferFeeGbp

`func (o *TeamMemberTransferredData) SetTransferFeeGbp(v string)`

SetTransferFeeGbp sets TransferFeeGbp field to given value.

### HasTransferFeeGbp

`func (o *TeamMemberTransferredData) HasTransferFeeGbp() bool`

HasTransferFeeGbp returns a boolean if a field has been set.

### GetTransferType

`func (o *TeamMemberTransferredData) GetTransferType() string`

GetTransferType returns the TransferType field if non-nil, zero value otherwise.

### GetTransferTypeOk

`func (o *TeamMemberTransferredData) GetTransferTypeOk() (*string, bool)`

GetTransferTypeOk returns a tuple with the TransferType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTransferType

`func (o *TeamMemberTransferredData) SetTransferType(v string)`

SetTransferType sets TransferType field to given value.


### GetYearsWithPreviousTeam

`func (o *TeamMemberTransferredData) GetYearsWithPreviousTeam() int32`

GetYearsWithPreviousTeam returns the YearsWithPreviousTeam field if non-nil, zero value otherwise.

### GetYearsWithPreviousTeamOk

`func (o *TeamMemberTransferredData) GetYearsWithPreviousTeamOk() (*int32, bool)`

GetYearsWithPreviousTeamOk returns a tuple with the YearsWithPreviousTeam field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetYearsWithPreviousTeam

`func (o *TeamMemberTransferredData) SetYearsWithPreviousTeam(v int32)`

SetYearsWithPreviousTeam sets YearsWithPreviousTeam field to given value.

### HasYearsWithPreviousTeam

`func (o *TeamMemberTransferredData) HasYearsWithPreviousTeam() bool`

HasYearsWithPreviousTeam returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


