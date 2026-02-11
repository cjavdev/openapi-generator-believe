# Team

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AnnualBudgetGbp** | Pointer to **NullableString** |  | [optional] 
**AverageAttendance** | Pointer to **NullableFloat32** |  | [optional] 
**ContactEmail** | Pointer to **NullableString** |  | [optional] 
**CultureScore** | **int32** | Team culture/morale score (0-100) | 
**FoundedYear** | **int32** | Year the club was founded | 
**Id** | **string** | Unique identifier | 
**IsActive** | Pointer to **bool** | Whether the team is currently active | [optional] [default to true]
**League** | [**League**](League.md) | Current league | 
**Name** | **string** | Team name | 
**Nickname** | Pointer to **NullableString** |  | [optional] 
**PrimaryColor** | Pointer to **NullableString** |  | [optional] 
**RivalTeams** | Pointer to **[]string** | List of rival team IDs | [optional] 
**SecondaryColor** | Pointer to **NullableString** |  | [optional] 
**Stadium** | **string** | Home stadium name | 
**StadiumLocation** | Pointer to [**NullableGeoLocation**](GeoLocation.md) |  | [optional] 
**Values** | [**TeamValues**](TeamValues.md) | Team&#39;s core values | 
**Website** | Pointer to **NullableString** |  | [optional] 
**WinPercentage** | Pointer to **NullableFloat32** |  | [optional] 

## Methods

### NewTeam

`func NewTeam(cultureScore int32, foundedYear int32, id string, league League, name string, stadium string, values TeamValues, ) *Team`

NewTeam instantiates a new Team object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTeamWithDefaults

`func NewTeamWithDefaults() *Team`

NewTeamWithDefaults instantiates a new Team object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAnnualBudgetGbp

`func (o *Team) GetAnnualBudgetGbp() string`

GetAnnualBudgetGbp returns the AnnualBudgetGbp field if non-nil, zero value otherwise.

### GetAnnualBudgetGbpOk

`func (o *Team) GetAnnualBudgetGbpOk() (*string, bool)`

GetAnnualBudgetGbpOk returns a tuple with the AnnualBudgetGbp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAnnualBudgetGbp

`func (o *Team) SetAnnualBudgetGbp(v string)`

SetAnnualBudgetGbp sets AnnualBudgetGbp field to given value.

### HasAnnualBudgetGbp

`func (o *Team) HasAnnualBudgetGbp() bool`

HasAnnualBudgetGbp returns a boolean if a field has been set.

### SetAnnualBudgetGbpNil

`func (o *Team) SetAnnualBudgetGbpNil(b bool)`

 SetAnnualBudgetGbpNil sets the value for AnnualBudgetGbp to be an explicit nil

### UnsetAnnualBudgetGbp
`func (o *Team) UnsetAnnualBudgetGbp()`

UnsetAnnualBudgetGbp ensures that no value is present for AnnualBudgetGbp, not even an explicit nil
### GetAverageAttendance

`func (o *Team) GetAverageAttendance() float32`

GetAverageAttendance returns the AverageAttendance field if non-nil, zero value otherwise.

### GetAverageAttendanceOk

`func (o *Team) GetAverageAttendanceOk() (*float32, bool)`

GetAverageAttendanceOk returns a tuple with the AverageAttendance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAverageAttendance

`func (o *Team) SetAverageAttendance(v float32)`

SetAverageAttendance sets AverageAttendance field to given value.

### HasAverageAttendance

`func (o *Team) HasAverageAttendance() bool`

HasAverageAttendance returns a boolean if a field has been set.

### SetAverageAttendanceNil

`func (o *Team) SetAverageAttendanceNil(b bool)`

 SetAverageAttendanceNil sets the value for AverageAttendance to be an explicit nil

### UnsetAverageAttendance
`func (o *Team) UnsetAverageAttendance()`

UnsetAverageAttendance ensures that no value is present for AverageAttendance, not even an explicit nil
### GetContactEmail

`func (o *Team) GetContactEmail() string`

GetContactEmail returns the ContactEmail field if non-nil, zero value otherwise.

### GetContactEmailOk

`func (o *Team) GetContactEmailOk() (*string, bool)`

GetContactEmailOk returns a tuple with the ContactEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContactEmail

`func (o *Team) SetContactEmail(v string)`

SetContactEmail sets ContactEmail field to given value.

### HasContactEmail

`func (o *Team) HasContactEmail() bool`

HasContactEmail returns a boolean if a field has been set.

### SetContactEmailNil

`func (o *Team) SetContactEmailNil(b bool)`

 SetContactEmailNil sets the value for ContactEmail to be an explicit nil

### UnsetContactEmail
`func (o *Team) UnsetContactEmail()`

UnsetContactEmail ensures that no value is present for ContactEmail, not even an explicit nil
### GetCultureScore

`func (o *Team) GetCultureScore() int32`

GetCultureScore returns the CultureScore field if non-nil, zero value otherwise.

### GetCultureScoreOk

`func (o *Team) GetCultureScoreOk() (*int32, bool)`

GetCultureScoreOk returns a tuple with the CultureScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCultureScore

`func (o *Team) SetCultureScore(v int32)`

SetCultureScore sets CultureScore field to given value.


### GetFoundedYear

`func (o *Team) GetFoundedYear() int32`

GetFoundedYear returns the FoundedYear field if non-nil, zero value otherwise.

### GetFoundedYearOk

`func (o *Team) GetFoundedYearOk() (*int32, bool)`

GetFoundedYearOk returns a tuple with the FoundedYear field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFoundedYear

`func (o *Team) SetFoundedYear(v int32)`

SetFoundedYear sets FoundedYear field to given value.


### GetId

`func (o *Team) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Team) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Team) SetId(v string)`

SetId sets Id field to given value.


### GetIsActive

`func (o *Team) GetIsActive() bool`

GetIsActive returns the IsActive field if non-nil, zero value otherwise.

### GetIsActiveOk

`func (o *Team) GetIsActiveOk() (*bool, bool)`

GetIsActiveOk returns a tuple with the IsActive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsActive

`func (o *Team) SetIsActive(v bool)`

SetIsActive sets IsActive field to given value.

### HasIsActive

`func (o *Team) HasIsActive() bool`

HasIsActive returns a boolean if a field has been set.

### GetLeague

`func (o *Team) GetLeague() League`

GetLeague returns the League field if non-nil, zero value otherwise.

### GetLeagueOk

`func (o *Team) GetLeagueOk() (*League, bool)`

GetLeagueOk returns a tuple with the League field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLeague

`func (o *Team) SetLeague(v League)`

SetLeague sets League field to given value.


### GetName

`func (o *Team) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Team) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Team) SetName(v string)`

SetName sets Name field to given value.


### GetNickname

`func (o *Team) GetNickname() string`

GetNickname returns the Nickname field if non-nil, zero value otherwise.

### GetNicknameOk

`func (o *Team) GetNicknameOk() (*string, bool)`

GetNicknameOk returns a tuple with the Nickname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNickname

`func (o *Team) SetNickname(v string)`

SetNickname sets Nickname field to given value.

### HasNickname

`func (o *Team) HasNickname() bool`

HasNickname returns a boolean if a field has been set.

### SetNicknameNil

`func (o *Team) SetNicknameNil(b bool)`

 SetNicknameNil sets the value for Nickname to be an explicit nil

### UnsetNickname
`func (o *Team) UnsetNickname()`

UnsetNickname ensures that no value is present for Nickname, not even an explicit nil
### GetPrimaryColor

`func (o *Team) GetPrimaryColor() string`

GetPrimaryColor returns the PrimaryColor field if non-nil, zero value otherwise.

### GetPrimaryColorOk

`func (o *Team) GetPrimaryColorOk() (*string, bool)`

GetPrimaryColorOk returns a tuple with the PrimaryColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrimaryColor

`func (o *Team) SetPrimaryColor(v string)`

SetPrimaryColor sets PrimaryColor field to given value.

### HasPrimaryColor

`func (o *Team) HasPrimaryColor() bool`

HasPrimaryColor returns a boolean if a field has been set.

### SetPrimaryColorNil

`func (o *Team) SetPrimaryColorNil(b bool)`

 SetPrimaryColorNil sets the value for PrimaryColor to be an explicit nil

### UnsetPrimaryColor
`func (o *Team) UnsetPrimaryColor()`

UnsetPrimaryColor ensures that no value is present for PrimaryColor, not even an explicit nil
### GetRivalTeams

`func (o *Team) GetRivalTeams() []string`

GetRivalTeams returns the RivalTeams field if non-nil, zero value otherwise.

### GetRivalTeamsOk

`func (o *Team) GetRivalTeamsOk() (*[]string, bool)`

GetRivalTeamsOk returns a tuple with the RivalTeams field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRivalTeams

`func (o *Team) SetRivalTeams(v []string)`

SetRivalTeams sets RivalTeams field to given value.

### HasRivalTeams

`func (o *Team) HasRivalTeams() bool`

HasRivalTeams returns a boolean if a field has been set.

### GetSecondaryColor

`func (o *Team) GetSecondaryColor() string`

GetSecondaryColor returns the SecondaryColor field if non-nil, zero value otherwise.

### GetSecondaryColorOk

`func (o *Team) GetSecondaryColorOk() (*string, bool)`

GetSecondaryColorOk returns a tuple with the SecondaryColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecondaryColor

`func (o *Team) SetSecondaryColor(v string)`

SetSecondaryColor sets SecondaryColor field to given value.

### HasSecondaryColor

`func (o *Team) HasSecondaryColor() bool`

HasSecondaryColor returns a boolean if a field has been set.

### SetSecondaryColorNil

`func (o *Team) SetSecondaryColorNil(b bool)`

 SetSecondaryColorNil sets the value for SecondaryColor to be an explicit nil

### UnsetSecondaryColor
`func (o *Team) UnsetSecondaryColor()`

UnsetSecondaryColor ensures that no value is present for SecondaryColor, not even an explicit nil
### GetStadium

`func (o *Team) GetStadium() string`

GetStadium returns the Stadium field if non-nil, zero value otherwise.

### GetStadiumOk

`func (o *Team) GetStadiumOk() (*string, bool)`

GetStadiumOk returns a tuple with the Stadium field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStadium

`func (o *Team) SetStadium(v string)`

SetStadium sets Stadium field to given value.


### GetStadiumLocation

`func (o *Team) GetStadiumLocation() GeoLocation`

GetStadiumLocation returns the StadiumLocation field if non-nil, zero value otherwise.

### GetStadiumLocationOk

`func (o *Team) GetStadiumLocationOk() (*GeoLocation, bool)`

GetStadiumLocationOk returns a tuple with the StadiumLocation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStadiumLocation

`func (o *Team) SetStadiumLocation(v GeoLocation)`

SetStadiumLocation sets StadiumLocation field to given value.

### HasStadiumLocation

`func (o *Team) HasStadiumLocation() bool`

HasStadiumLocation returns a boolean if a field has been set.

### SetStadiumLocationNil

`func (o *Team) SetStadiumLocationNil(b bool)`

 SetStadiumLocationNil sets the value for StadiumLocation to be an explicit nil

### UnsetStadiumLocation
`func (o *Team) UnsetStadiumLocation()`

UnsetStadiumLocation ensures that no value is present for StadiumLocation, not even an explicit nil
### GetValues

`func (o *Team) GetValues() TeamValues`

GetValues returns the Values field if non-nil, zero value otherwise.

### GetValuesOk

`func (o *Team) GetValuesOk() (*TeamValues, bool)`

GetValuesOk returns a tuple with the Values field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValues

`func (o *Team) SetValues(v TeamValues)`

SetValues sets Values field to given value.


### GetWebsite

`func (o *Team) GetWebsite() string`

GetWebsite returns the Website field if non-nil, zero value otherwise.

### GetWebsiteOk

`func (o *Team) GetWebsiteOk() (*string, bool)`

GetWebsiteOk returns a tuple with the Website field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebsite

`func (o *Team) SetWebsite(v string)`

SetWebsite sets Website field to given value.

### HasWebsite

`func (o *Team) HasWebsite() bool`

HasWebsite returns a boolean if a field has been set.

### SetWebsiteNil

`func (o *Team) SetWebsiteNil(b bool)`

 SetWebsiteNil sets the value for Website to be an explicit nil

### UnsetWebsite
`func (o *Team) UnsetWebsite()`

UnsetWebsite ensures that no value is present for Website, not even an explicit nil
### GetWinPercentage

`func (o *Team) GetWinPercentage() float32`

GetWinPercentage returns the WinPercentage field if non-nil, zero value otherwise.

### GetWinPercentageOk

`func (o *Team) GetWinPercentageOk() (*float32, bool)`

GetWinPercentageOk returns a tuple with the WinPercentage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWinPercentage

`func (o *Team) SetWinPercentage(v float32)`

SetWinPercentage sets WinPercentage field to given value.

### HasWinPercentage

`func (o *Team) HasWinPercentage() bool`

HasWinPercentage returns a boolean if a field has been set.

### SetWinPercentageNil

`func (o *Team) SetWinPercentageNil(b bool)`

 SetWinPercentageNil sets the value for WinPercentage to be an explicit nil

### UnsetWinPercentage
`func (o *Team) UnsetWinPercentage()`

UnsetWinPercentage ensures that no value is present for WinPercentage, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


