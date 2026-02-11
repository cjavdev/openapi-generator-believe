# Player

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Assists** | Pointer to **int32** | Total assists for the team | [optional] [default to 0]
**CharacterId** | **string** | ID of the character (references /characters/{id}) | 
**GoalsScored** | Pointer to **int32** | Total goals scored for the team | [optional] [default to 0]
**Id** | **string** | Unique identifier for this team membership | 
**IsCaptain** | Pointer to **bool** | Whether this player is team captain | [optional] [default to false]
**JerseyNumber** | **int32** | Jersey/shirt number | 
**MemberType** | Pointer to **string** | Discriminator field indicating this is a player | [optional] [default to "player"]
**Position** | [**Position**](Position.md) | Playing position on the field | 
**TeamId** | **string** | ID of the team they belong to | 
**YearsWithTeam** | **int32** | Number of years with the current team | 

## Methods

### NewPlayer

`func NewPlayer(characterId string, id string, jerseyNumber int32, position Position, teamId string, yearsWithTeam int32, ) *Player`

NewPlayer instantiates a new Player object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPlayerWithDefaults

`func NewPlayerWithDefaults() *Player`

NewPlayerWithDefaults instantiates a new Player object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAssists

`func (o *Player) GetAssists() int32`

GetAssists returns the Assists field if non-nil, zero value otherwise.

### GetAssistsOk

`func (o *Player) GetAssistsOk() (*int32, bool)`

GetAssistsOk returns a tuple with the Assists field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssists

`func (o *Player) SetAssists(v int32)`

SetAssists sets Assists field to given value.

### HasAssists

`func (o *Player) HasAssists() bool`

HasAssists returns a boolean if a field has been set.

### GetCharacterId

`func (o *Player) GetCharacterId() string`

GetCharacterId returns the CharacterId field if non-nil, zero value otherwise.

### GetCharacterIdOk

`func (o *Player) GetCharacterIdOk() (*string, bool)`

GetCharacterIdOk returns a tuple with the CharacterId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCharacterId

`func (o *Player) SetCharacterId(v string)`

SetCharacterId sets CharacterId field to given value.


### GetGoalsScored

`func (o *Player) GetGoalsScored() int32`

GetGoalsScored returns the GoalsScored field if non-nil, zero value otherwise.

### GetGoalsScoredOk

`func (o *Player) GetGoalsScoredOk() (*int32, bool)`

GetGoalsScoredOk returns a tuple with the GoalsScored field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGoalsScored

`func (o *Player) SetGoalsScored(v int32)`

SetGoalsScored sets GoalsScored field to given value.

### HasGoalsScored

`func (o *Player) HasGoalsScored() bool`

HasGoalsScored returns a boolean if a field has been set.

### GetId

`func (o *Player) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Player) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Player) SetId(v string)`

SetId sets Id field to given value.


### GetIsCaptain

`func (o *Player) GetIsCaptain() bool`

GetIsCaptain returns the IsCaptain field if non-nil, zero value otherwise.

### GetIsCaptainOk

`func (o *Player) GetIsCaptainOk() (*bool, bool)`

GetIsCaptainOk returns a tuple with the IsCaptain field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsCaptain

`func (o *Player) SetIsCaptain(v bool)`

SetIsCaptain sets IsCaptain field to given value.

### HasIsCaptain

`func (o *Player) HasIsCaptain() bool`

HasIsCaptain returns a boolean if a field has been set.

### GetJerseyNumber

`func (o *Player) GetJerseyNumber() int32`

GetJerseyNumber returns the JerseyNumber field if non-nil, zero value otherwise.

### GetJerseyNumberOk

`func (o *Player) GetJerseyNumberOk() (*int32, bool)`

GetJerseyNumberOk returns a tuple with the JerseyNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJerseyNumber

`func (o *Player) SetJerseyNumber(v int32)`

SetJerseyNumber sets JerseyNumber field to given value.


### GetMemberType

`func (o *Player) GetMemberType() string`

GetMemberType returns the MemberType field if non-nil, zero value otherwise.

### GetMemberTypeOk

`func (o *Player) GetMemberTypeOk() (*string, bool)`

GetMemberTypeOk returns a tuple with the MemberType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMemberType

`func (o *Player) SetMemberType(v string)`

SetMemberType sets MemberType field to given value.

### HasMemberType

`func (o *Player) HasMemberType() bool`

HasMemberType returns a boolean if a field has been set.

### GetPosition

`func (o *Player) GetPosition() Position`

GetPosition returns the Position field if non-nil, zero value otherwise.

### GetPositionOk

`func (o *Player) GetPositionOk() (*Position, bool)`

GetPositionOk returns a tuple with the Position field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPosition

`func (o *Player) SetPosition(v Position)`

SetPosition sets Position field to given value.


### GetTeamId

`func (o *Player) GetTeamId() string`

GetTeamId returns the TeamId field if non-nil, zero value otherwise.

### GetTeamIdOk

`func (o *Player) GetTeamIdOk() (*string, bool)`

GetTeamIdOk returns a tuple with the TeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamId

`func (o *Player) SetTeamId(v string)`

SetTeamId sets TeamId field to given value.


### GetYearsWithTeam

`func (o *Player) GetYearsWithTeam() int32`

GetYearsWithTeam returns the YearsWithTeam field if non-nil, zero value otherwise.

### GetYearsWithTeamOk

`func (o *Player) GetYearsWithTeamOk() (*int32, bool)`

GetYearsWithTeamOk returns a tuple with the YearsWithTeam field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetYearsWithTeam

`func (o *Player) SetYearsWithTeam(v int32)`

SetYearsWithTeam sets YearsWithTeam field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


