# PlayerUpdate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Assists** | Pointer to **NullableInt32** |  | [optional] 
**GoalsScored** | Pointer to **NullableInt32** |  | [optional] 
**IsCaptain** | Pointer to **NullableBool** |  | [optional] 
**JerseyNumber** | Pointer to **NullableInt32** |  | [optional] 
**Position** | Pointer to [**NullablePosition**](Position.md) |  | [optional] 
**TeamId** | Pointer to **NullableString** |  | [optional] 
**YearsWithTeam** | Pointer to **NullableInt32** |  | [optional] 

## Methods

### NewPlayerUpdate

`func NewPlayerUpdate() *PlayerUpdate`

NewPlayerUpdate instantiates a new PlayerUpdate object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPlayerUpdateWithDefaults

`func NewPlayerUpdateWithDefaults() *PlayerUpdate`

NewPlayerUpdateWithDefaults instantiates a new PlayerUpdate object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAssists

`func (o *PlayerUpdate) GetAssists() int32`

GetAssists returns the Assists field if non-nil, zero value otherwise.

### GetAssistsOk

`func (o *PlayerUpdate) GetAssistsOk() (*int32, bool)`

GetAssistsOk returns a tuple with the Assists field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssists

`func (o *PlayerUpdate) SetAssists(v int32)`

SetAssists sets Assists field to given value.

### HasAssists

`func (o *PlayerUpdate) HasAssists() bool`

HasAssists returns a boolean if a field has been set.

### SetAssistsNil

`func (o *PlayerUpdate) SetAssistsNil(b bool)`

 SetAssistsNil sets the value for Assists to be an explicit nil

### UnsetAssists
`func (o *PlayerUpdate) UnsetAssists()`

UnsetAssists ensures that no value is present for Assists, not even an explicit nil
### GetGoalsScored

`func (o *PlayerUpdate) GetGoalsScored() int32`

GetGoalsScored returns the GoalsScored field if non-nil, zero value otherwise.

### GetGoalsScoredOk

`func (o *PlayerUpdate) GetGoalsScoredOk() (*int32, bool)`

GetGoalsScoredOk returns a tuple with the GoalsScored field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGoalsScored

`func (o *PlayerUpdate) SetGoalsScored(v int32)`

SetGoalsScored sets GoalsScored field to given value.

### HasGoalsScored

`func (o *PlayerUpdate) HasGoalsScored() bool`

HasGoalsScored returns a boolean if a field has been set.

### SetGoalsScoredNil

`func (o *PlayerUpdate) SetGoalsScoredNil(b bool)`

 SetGoalsScoredNil sets the value for GoalsScored to be an explicit nil

### UnsetGoalsScored
`func (o *PlayerUpdate) UnsetGoalsScored()`

UnsetGoalsScored ensures that no value is present for GoalsScored, not even an explicit nil
### GetIsCaptain

`func (o *PlayerUpdate) GetIsCaptain() bool`

GetIsCaptain returns the IsCaptain field if non-nil, zero value otherwise.

### GetIsCaptainOk

`func (o *PlayerUpdate) GetIsCaptainOk() (*bool, bool)`

GetIsCaptainOk returns a tuple with the IsCaptain field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsCaptain

`func (o *PlayerUpdate) SetIsCaptain(v bool)`

SetIsCaptain sets IsCaptain field to given value.

### HasIsCaptain

`func (o *PlayerUpdate) HasIsCaptain() bool`

HasIsCaptain returns a boolean if a field has been set.

### SetIsCaptainNil

`func (o *PlayerUpdate) SetIsCaptainNil(b bool)`

 SetIsCaptainNil sets the value for IsCaptain to be an explicit nil

### UnsetIsCaptain
`func (o *PlayerUpdate) UnsetIsCaptain()`

UnsetIsCaptain ensures that no value is present for IsCaptain, not even an explicit nil
### GetJerseyNumber

`func (o *PlayerUpdate) GetJerseyNumber() int32`

GetJerseyNumber returns the JerseyNumber field if non-nil, zero value otherwise.

### GetJerseyNumberOk

`func (o *PlayerUpdate) GetJerseyNumberOk() (*int32, bool)`

GetJerseyNumberOk returns a tuple with the JerseyNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJerseyNumber

`func (o *PlayerUpdate) SetJerseyNumber(v int32)`

SetJerseyNumber sets JerseyNumber field to given value.

### HasJerseyNumber

`func (o *PlayerUpdate) HasJerseyNumber() bool`

HasJerseyNumber returns a boolean if a field has been set.

### SetJerseyNumberNil

`func (o *PlayerUpdate) SetJerseyNumberNil(b bool)`

 SetJerseyNumberNil sets the value for JerseyNumber to be an explicit nil

### UnsetJerseyNumber
`func (o *PlayerUpdate) UnsetJerseyNumber()`

UnsetJerseyNumber ensures that no value is present for JerseyNumber, not even an explicit nil
### GetPosition

`func (o *PlayerUpdate) GetPosition() Position`

GetPosition returns the Position field if non-nil, zero value otherwise.

### GetPositionOk

`func (o *PlayerUpdate) GetPositionOk() (*Position, bool)`

GetPositionOk returns a tuple with the Position field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPosition

`func (o *PlayerUpdate) SetPosition(v Position)`

SetPosition sets Position field to given value.

### HasPosition

`func (o *PlayerUpdate) HasPosition() bool`

HasPosition returns a boolean if a field has been set.

### SetPositionNil

`func (o *PlayerUpdate) SetPositionNil(b bool)`

 SetPositionNil sets the value for Position to be an explicit nil

### UnsetPosition
`func (o *PlayerUpdate) UnsetPosition()`

UnsetPosition ensures that no value is present for Position, not even an explicit nil
### GetTeamId

`func (o *PlayerUpdate) GetTeamId() string`

GetTeamId returns the TeamId field if non-nil, zero value otherwise.

### GetTeamIdOk

`func (o *PlayerUpdate) GetTeamIdOk() (*string, bool)`

GetTeamIdOk returns a tuple with the TeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamId

`func (o *PlayerUpdate) SetTeamId(v string)`

SetTeamId sets TeamId field to given value.

### HasTeamId

`func (o *PlayerUpdate) HasTeamId() bool`

HasTeamId returns a boolean if a field has been set.

### SetTeamIdNil

`func (o *PlayerUpdate) SetTeamIdNil(b bool)`

 SetTeamIdNil sets the value for TeamId to be an explicit nil

### UnsetTeamId
`func (o *PlayerUpdate) UnsetTeamId()`

UnsetTeamId ensures that no value is present for TeamId, not even an explicit nil
### GetYearsWithTeam

`func (o *PlayerUpdate) GetYearsWithTeam() int32`

GetYearsWithTeam returns the YearsWithTeam field if non-nil, zero value otherwise.

### GetYearsWithTeamOk

`func (o *PlayerUpdate) GetYearsWithTeamOk() (*int32, bool)`

GetYearsWithTeamOk returns a tuple with the YearsWithTeam field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetYearsWithTeam

`func (o *PlayerUpdate) SetYearsWithTeam(v int32)`

SetYearsWithTeam sets YearsWithTeam field to given value.

### HasYearsWithTeam

`func (o *PlayerUpdate) HasYearsWithTeam() bool`

HasYearsWithTeam returns a boolean if a field has been set.

### SetYearsWithTeamNil

`func (o *PlayerUpdate) SetYearsWithTeamNil(b bool)`

 SetYearsWithTeamNil sets the value for YearsWithTeam to be an explicit nil

### UnsetYearsWithTeam
`func (o *PlayerUpdate) UnsetYearsWithTeam()`

UnsetYearsWithTeam ensures that no value is present for YearsWithTeam, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


