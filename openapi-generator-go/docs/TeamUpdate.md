# TeamUpdate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AnnualBudgetGbp** | Pointer to [**NullableAnnualBudgetGbp1**](AnnualBudgetGbp1.md) |  | [optional] 
**AverageAttendance** | Pointer to **NullableFloat32** |  | [optional] 
**ContactEmail** | Pointer to **NullableString** |  | [optional] 
**CultureScore** | Pointer to **NullableInt32** |  | [optional] 
**FoundedYear** | Pointer to **NullableInt32** |  | [optional] 
**IsActive** | Pointer to **NullableBool** |  | [optional] 
**League** | Pointer to [**NullableLeague**](League.md) |  | [optional] 
**Name** | Pointer to **NullableString** |  | [optional] 
**Nickname** | Pointer to **NullableString** |  | [optional] 
**PrimaryColor** | Pointer to **NullableString** |  | [optional] 
**RivalTeams** | Pointer to **[]string** |  | [optional] 
**SecondaryColor** | Pointer to **NullableString** |  | [optional] 
**Stadium** | Pointer to **NullableString** |  | [optional] 
**StadiumLocation** | Pointer to [**NullableGeoLocation**](GeoLocation.md) |  | [optional] 
**Values** | Pointer to [**NullableTeamValues**](TeamValues.md) |  | [optional] 
**Website** | Pointer to **NullableString** |  | [optional] 
**WinPercentage** | Pointer to **NullableFloat32** |  | [optional] 

## Methods

### NewTeamUpdate

`func NewTeamUpdate() *TeamUpdate`

NewTeamUpdate instantiates a new TeamUpdate object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTeamUpdateWithDefaults

`func NewTeamUpdateWithDefaults() *TeamUpdate`

NewTeamUpdateWithDefaults instantiates a new TeamUpdate object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAnnualBudgetGbp

`func (o *TeamUpdate) GetAnnualBudgetGbp() AnnualBudgetGbp1`

GetAnnualBudgetGbp returns the AnnualBudgetGbp field if non-nil, zero value otherwise.

### GetAnnualBudgetGbpOk

`func (o *TeamUpdate) GetAnnualBudgetGbpOk() (*AnnualBudgetGbp1, bool)`

GetAnnualBudgetGbpOk returns a tuple with the AnnualBudgetGbp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAnnualBudgetGbp

`func (o *TeamUpdate) SetAnnualBudgetGbp(v AnnualBudgetGbp1)`

SetAnnualBudgetGbp sets AnnualBudgetGbp field to given value.

### HasAnnualBudgetGbp

`func (o *TeamUpdate) HasAnnualBudgetGbp() bool`

HasAnnualBudgetGbp returns a boolean if a field has been set.

### SetAnnualBudgetGbpNil

`func (o *TeamUpdate) SetAnnualBudgetGbpNil(b bool)`

 SetAnnualBudgetGbpNil sets the value for AnnualBudgetGbp to be an explicit nil

### UnsetAnnualBudgetGbp
`func (o *TeamUpdate) UnsetAnnualBudgetGbp()`

UnsetAnnualBudgetGbp ensures that no value is present for AnnualBudgetGbp, not even an explicit nil
### GetAverageAttendance

`func (o *TeamUpdate) GetAverageAttendance() float32`

GetAverageAttendance returns the AverageAttendance field if non-nil, zero value otherwise.

### GetAverageAttendanceOk

`func (o *TeamUpdate) GetAverageAttendanceOk() (*float32, bool)`

GetAverageAttendanceOk returns a tuple with the AverageAttendance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAverageAttendance

`func (o *TeamUpdate) SetAverageAttendance(v float32)`

SetAverageAttendance sets AverageAttendance field to given value.

### HasAverageAttendance

`func (o *TeamUpdate) HasAverageAttendance() bool`

HasAverageAttendance returns a boolean if a field has been set.

### SetAverageAttendanceNil

`func (o *TeamUpdate) SetAverageAttendanceNil(b bool)`

 SetAverageAttendanceNil sets the value for AverageAttendance to be an explicit nil

### UnsetAverageAttendance
`func (o *TeamUpdate) UnsetAverageAttendance()`

UnsetAverageAttendance ensures that no value is present for AverageAttendance, not even an explicit nil
### GetContactEmail

`func (o *TeamUpdate) GetContactEmail() string`

GetContactEmail returns the ContactEmail field if non-nil, zero value otherwise.

### GetContactEmailOk

`func (o *TeamUpdate) GetContactEmailOk() (*string, bool)`

GetContactEmailOk returns a tuple with the ContactEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContactEmail

`func (o *TeamUpdate) SetContactEmail(v string)`

SetContactEmail sets ContactEmail field to given value.

### HasContactEmail

`func (o *TeamUpdate) HasContactEmail() bool`

HasContactEmail returns a boolean if a field has been set.

### SetContactEmailNil

`func (o *TeamUpdate) SetContactEmailNil(b bool)`

 SetContactEmailNil sets the value for ContactEmail to be an explicit nil

### UnsetContactEmail
`func (o *TeamUpdate) UnsetContactEmail()`

UnsetContactEmail ensures that no value is present for ContactEmail, not even an explicit nil
### GetCultureScore

`func (o *TeamUpdate) GetCultureScore() int32`

GetCultureScore returns the CultureScore field if non-nil, zero value otherwise.

### GetCultureScoreOk

`func (o *TeamUpdate) GetCultureScoreOk() (*int32, bool)`

GetCultureScoreOk returns a tuple with the CultureScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCultureScore

`func (o *TeamUpdate) SetCultureScore(v int32)`

SetCultureScore sets CultureScore field to given value.

### HasCultureScore

`func (o *TeamUpdate) HasCultureScore() bool`

HasCultureScore returns a boolean if a field has been set.

### SetCultureScoreNil

`func (o *TeamUpdate) SetCultureScoreNil(b bool)`

 SetCultureScoreNil sets the value for CultureScore to be an explicit nil

### UnsetCultureScore
`func (o *TeamUpdate) UnsetCultureScore()`

UnsetCultureScore ensures that no value is present for CultureScore, not even an explicit nil
### GetFoundedYear

`func (o *TeamUpdate) GetFoundedYear() int32`

GetFoundedYear returns the FoundedYear field if non-nil, zero value otherwise.

### GetFoundedYearOk

`func (o *TeamUpdate) GetFoundedYearOk() (*int32, bool)`

GetFoundedYearOk returns a tuple with the FoundedYear field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFoundedYear

`func (o *TeamUpdate) SetFoundedYear(v int32)`

SetFoundedYear sets FoundedYear field to given value.

### HasFoundedYear

`func (o *TeamUpdate) HasFoundedYear() bool`

HasFoundedYear returns a boolean if a field has been set.

### SetFoundedYearNil

`func (o *TeamUpdate) SetFoundedYearNil(b bool)`

 SetFoundedYearNil sets the value for FoundedYear to be an explicit nil

### UnsetFoundedYear
`func (o *TeamUpdate) UnsetFoundedYear()`

UnsetFoundedYear ensures that no value is present for FoundedYear, not even an explicit nil
### GetIsActive

`func (o *TeamUpdate) GetIsActive() bool`

GetIsActive returns the IsActive field if non-nil, zero value otherwise.

### GetIsActiveOk

`func (o *TeamUpdate) GetIsActiveOk() (*bool, bool)`

GetIsActiveOk returns a tuple with the IsActive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsActive

`func (o *TeamUpdate) SetIsActive(v bool)`

SetIsActive sets IsActive field to given value.

### HasIsActive

`func (o *TeamUpdate) HasIsActive() bool`

HasIsActive returns a boolean if a field has been set.

### SetIsActiveNil

`func (o *TeamUpdate) SetIsActiveNil(b bool)`

 SetIsActiveNil sets the value for IsActive to be an explicit nil

### UnsetIsActive
`func (o *TeamUpdate) UnsetIsActive()`

UnsetIsActive ensures that no value is present for IsActive, not even an explicit nil
### GetLeague

`func (o *TeamUpdate) GetLeague() League`

GetLeague returns the League field if non-nil, zero value otherwise.

### GetLeagueOk

`func (o *TeamUpdate) GetLeagueOk() (*League, bool)`

GetLeagueOk returns a tuple with the League field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLeague

`func (o *TeamUpdate) SetLeague(v League)`

SetLeague sets League field to given value.

### HasLeague

`func (o *TeamUpdate) HasLeague() bool`

HasLeague returns a boolean if a field has been set.

### SetLeagueNil

`func (o *TeamUpdate) SetLeagueNil(b bool)`

 SetLeagueNil sets the value for League to be an explicit nil

### UnsetLeague
`func (o *TeamUpdate) UnsetLeague()`

UnsetLeague ensures that no value is present for League, not even an explicit nil
### GetName

`func (o *TeamUpdate) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *TeamUpdate) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *TeamUpdate) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *TeamUpdate) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *TeamUpdate) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *TeamUpdate) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetNickname

`func (o *TeamUpdate) GetNickname() string`

GetNickname returns the Nickname field if non-nil, zero value otherwise.

### GetNicknameOk

`func (o *TeamUpdate) GetNicknameOk() (*string, bool)`

GetNicknameOk returns a tuple with the Nickname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNickname

`func (o *TeamUpdate) SetNickname(v string)`

SetNickname sets Nickname field to given value.

### HasNickname

`func (o *TeamUpdate) HasNickname() bool`

HasNickname returns a boolean if a field has been set.

### SetNicknameNil

`func (o *TeamUpdate) SetNicknameNil(b bool)`

 SetNicknameNil sets the value for Nickname to be an explicit nil

### UnsetNickname
`func (o *TeamUpdate) UnsetNickname()`

UnsetNickname ensures that no value is present for Nickname, not even an explicit nil
### GetPrimaryColor

`func (o *TeamUpdate) GetPrimaryColor() string`

GetPrimaryColor returns the PrimaryColor field if non-nil, zero value otherwise.

### GetPrimaryColorOk

`func (o *TeamUpdate) GetPrimaryColorOk() (*string, bool)`

GetPrimaryColorOk returns a tuple with the PrimaryColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrimaryColor

`func (o *TeamUpdate) SetPrimaryColor(v string)`

SetPrimaryColor sets PrimaryColor field to given value.

### HasPrimaryColor

`func (o *TeamUpdate) HasPrimaryColor() bool`

HasPrimaryColor returns a boolean if a field has been set.

### SetPrimaryColorNil

`func (o *TeamUpdate) SetPrimaryColorNil(b bool)`

 SetPrimaryColorNil sets the value for PrimaryColor to be an explicit nil

### UnsetPrimaryColor
`func (o *TeamUpdate) UnsetPrimaryColor()`

UnsetPrimaryColor ensures that no value is present for PrimaryColor, not even an explicit nil
### GetRivalTeams

`func (o *TeamUpdate) GetRivalTeams() []string`

GetRivalTeams returns the RivalTeams field if non-nil, zero value otherwise.

### GetRivalTeamsOk

`func (o *TeamUpdate) GetRivalTeamsOk() (*[]string, bool)`

GetRivalTeamsOk returns a tuple with the RivalTeams field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRivalTeams

`func (o *TeamUpdate) SetRivalTeams(v []string)`

SetRivalTeams sets RivalTeams field to given value.

### HasRivalTeams

`func (o *TeamUpdate) HasRivalTeams() bool`

HasRivalTeams returns a boolean if a field has been set.

### SetRivalTeamsNil

`func (o *TeamUpdate) SetRivalTeamsNil(b bool)`

 SetRivalTeamsNil sets the value for RivalTeams to be an explicit nil

### UnsetRivalTeams
`func (o *TeamUpdate) UnsetRivalTeams()`

UnsetRivalTeams ensures that no value is present for RivalTeams, not even an explicit nil
### GetSecondaryColor

`func (o *TeamUpdate) GetSecondaryColor() string`

GetSecondaryColor returns the SecondaryColor field if non-nil, zero value otherwise.

### GetSecondaryColorOk

`func (o *TeamUpdate) GetSecondaryColorOk() (*string, bool)`

GetSecondaryColorOk returns a tuple with the SecondaryColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecondaryColor

`func (o *TeamUpdate) SetSecondaryColor(v string)`

SetSecondaryColor sets SecondaryColor field to given value.

### HasSecondaryColor

`func (o *TeamUpdate) HasSecondaryColor() bool`

HasSecondaryColor returns a boolean if a field has been set.

### SetSecondaryColorNil

`func (o *TeamUpdate) SetSecondaryColorNil(b bool)`

 SetSecondaryColorNil sets the value for SecondaryColor to be an explicit nil

### UnsetSecondaryColor
`func (o *TeamUpdate) UnsetSecondaryColor()`

UnsetSecondaryColor ensures that no value is present for SecondaryColor, not even an explicit nil
### GetStadium

`func (o *TeamUpdate) GetStadium() string`

GetStadium returns the Stadium field if non-nil, zero value otherwise.

### GetStadiumOk

`func (o *TeamUpdate) GetStadiumOk() (*string, bool)`

GetStadiumOk returns a tuple with the Stadium field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStadium

`func (o *TeamUpdate) SetStadium(v string)`

SetStadium sets Stadium field to given value.

### HasStadium

`func (o *TeamUpdate) HasStadium() bool`

HasStadium returns a boolean if a field has been set.

### SetStadiumNil

`func (o *TeamUpdate) SetStadiumNil(b bool)`

 SetStadiumNil sets the value for Stadium to be an explicit nil

### UnsetStadium
`func (o *TeamUpdate) UnsetStadium()`

UnsetStadium ensures that no value is present for Stadium, not even an explicit nil
### GetStadiumLocation

`func (o *TeamUpdate) GetStadiumLocation() GeoLocation`

GetStadiumLocation returns the StadiumLocation field if non-nil, zero value otherwise.

### GetStadiumLocationOk

`func (o *TeamUpdate) GetStadiumLocationOk() (*GeoLocation, bool)`

GetStadiumLocationOk returns a tuple with the StadiumLocation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStadiumLocation

`func (o *TeamUpdate) SetStadiumLocation(v GeoLocation)`

SetStadiumLocation sets StadiumLocation field to given value.

### HasStadiumLocation

`func (o *TeamUpdate) HasStadiumLocation() bool`

HasStadiumLocation returns a boolean if a field has been set.

### SetStadiumLocationNil

`func (o *TeamUpdate) SetStadiumLocationNil(b bool)`

 SetStadiumLocationNil sets the value for StadiumLocation to be an explicit nil

### UnsetStadiumLocation
`func (o *TeamUpdate) UnsetStadiumLocation()`

UnsetStadiumLocation ensures that no value is present for StadiumLocation, not even an explicit nil
### GetValues

`func (o *TeamUpdate) GetValues() TeamValues`

GetValues returns the Values field if non-nil, zero value otherwise.

### GetValuesOk

`func (o *TeamUpdate) GetValuesOk() (*TeamValues, bool)`

GetValuesOk returns a tuple with the Values field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValues

`func (o *TeamUpdate) SetValues(v TeamValues)`

SetValues sets Values field to given value.

### HasValues

`func (o *TeamUpdate) HasValues() bool`

HasValues returns a boolean if a field has been set.

### SetValuesNil

`func (o *TeamUpdate) SetValuesNil(b bool)`

 SetValuesNil sets the value for Values to be an explicit nil

### UnsetValues
`func (o *TeamUpdate) UnsetValues()`

UnsetValues ensures that no value is present for Values, not even an explicit nil
### GetWebsite

`func (o *TeamUpdate) GetWebsite() string`

GetWebsite returns the Website field if non-nil, zero value otherwise.

### GetWebsiteOk

`func (o *TeamUpdate) GetWebsiteOk() (*string, bool)`

GetWebsiteOk returns a tuple with the Website field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebsite

`func (o *TeamUpdate) SetWebsite(v string)`

SetWebsite sets Website field to given value.

### HasWebsite

`func (o *TeamUpdate) HasWebsite() bool`

HasWebsite returns a boolean if a field has been set.

### SetWebsiteNil

`func (o *TeamUpdate) SetWebsiteNil(b bool)`

 SetWebsiteNil sets the value for Website to be an explicit nil

### UnsetWebsite
`func (o *TeamUpdate) UnsetWebsite()`

UnsetWebsite ensures that no value is present for Website, not even an explicit nil
### GetWinPercentage

`func (o *TeamUpdate) GetWinPercentage() float32`

GetWinPercentage returns the WinPercentage field if non-nil, zero value otherwise.

### GetWinPercentageOk

`func (o *TeamUpdate) GetWinPercentageOk() (*float32, bool)`

GetWinPercentageOk returns a tuple with the WinPercentage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWinPercentage

`func (o *TeamUpdate) SetWinPercentage(v float32)`

SetWinPercentage sets WinPercentage field to given value.

### HasWinPercentage

`func (o *TeamUpdate) HasWinPercentage() bool`

HasWinPercentage returns a boolean if a field has been set.

### SetWinPercentageNil

`func (o *TeamUpdate) SetWinPercentageNil(b bool)`

 SetWinPercentageNil sets the value for WinPercentage to be an explicit nil

### UnsetWinPercentage
`func (o *TeamUpdate) UnsetWinPercentage()`

UnsetWinPercentage ensures that no value is present for WinPercentage, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


