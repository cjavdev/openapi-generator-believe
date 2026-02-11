# TeamCreate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AnnualBudgetGbp** | Pointer to [**NullableAnnualBudgetGbp**](AnnualBudgetGbp.md) |  | [optional] 
**AverageAttendance** | Pointer to **NullableFloat32** |  | [optional] 
**ContactEmail** | Pointer to **NullableString** |  | [optional] 
**CultureScore** | **int32** | Team culture/morale score (0-100) | 
**FoundedYear** | **int32** | Year the club was founded | 
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

### NewTeamCreate

`func NewTeamCreate(cultureScore int32, foundedYear int32, league League, name string, stadium string, values TeamValues, ) *TeamCreate`

NewTeamCreate instantiates a new TeamCreate object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTeamCreateWithDefaults

`func NewTeamCreateWithDefaults() *TeamCreate`

NewTeamCreateWithDefaults instantiates a new TeamCreate object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAnnualBudgetGbp

`func (o *TeamCreate) GetAnnualBudgetGbp() AnnualBudgetGbp`

GetAnnualBudgetGbp returns the AnnualBudgetGbp field if non-nil, zero value otherwise.

### GetAnnualBudgetGbpOk

`func (o *TeamCreate) GetAnnualBudgetGbpOk() (*AnnualBudgetGbp, bool)`

GetAnnualBudgetGbpOk returns a tuple with the AnnualBudgetGbp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAnnualBudgetGbp

`func (o *TeamCreate) SetAnnualBudgetGbp(v AnnualBudgetGbp)`

SetAnnualBudgetGbp sets AnnualBudgetGbp field to given value.

### HasAnnualBudgetGbp

`func (o *TeamCreate) HasAnnualBudgetGbp() bool`

HasAnnualBudgetGbp returns a boolean if a field has been set.

### SetAnnualBudgetGbpNil

`func (o *TeamCreate) SetAnnualBudgetGbpNil(b bool)`

 SetAnnualBudgetGbpNil sets the value for AnnualBudgetGbp to be an explicit nil

### UnsetAnnualBudgetGbp
`func (o *TeamCreate) UnsetAnnualBudgetGbp()`

UnsetAnnualBudgetGbp ensures that no value is present for AnnualBudgetGbp, not even an explicit nil
### GetAverageAttendance

`func (o *TeamCreate) GetAverageAttendance() float32`

GetAverageAttendance returns the AverageAttendance field if non-nil, zero value otherwise.

### GetAverageAttendanceOk

`func (o *TeamCreate) GetAverageAttendanceOk() (*float32, bool)`

GetAverageAttendanceOk returns a tuple with the AverageAttendance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAverageAttendance

`func (o *TeamCreate) SetAverageAttendance(v float32)`

SetAverageAttendance sets AverageAttendance field to given value.

### HasAverageAttendance

`func (o *TeamCreate) HasAverageAttendance() bool`

HasAverageAttendance returns a boolean if a field has been set.

### SetAverageAttendanceNil

`func (o *TeamCreate) SetAverageAttendanceNil(b bool)`

 SetAverageAttendanceNil sets the value for AverageAttendance to be an explicit nil

### UnsetAverageAttendance
`func (o *TeamCreate) UnsetAverageAttendance()`

UnsetAverageAttendance ensures that no value is present for AverageAttendance, not even an explicit nil
### GetContactEmail

`func (o *TeamCreate) GetContactEmail() string`

GetContactEmail returns the ContactEmail field if non-nil, zero value otherwise.

### GetContactEmailOk

`func (o *TeamCreate) GetContactEmailOk() (*string, bool)`

GetContactEmailOk returns a tuple with the ContactEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContactEmail

`func (o *TeamCreate) SetContactEmail(v string)`

SetContactEmail sets ContactEmail field to given value.

### HasContactEmail

`func (o *TeamCreate) HasContactEmail() bool`

HasContactEmail returns a boolean if a field has been set.

### SetContactEmailNil

`func (o *TeamCreate) SetContactEmailNil(b bool)`

 SetContactEmailNil sets the value for ContactEmail to be an explicit nil

### UnsetContactEmail
`func (o *TeamCreate) UnsetContactEmail()`

UnsetContactEmail ensures that no value is present for ContactEmail, not even an explicit nil
### GetCultureScore

`func (o *TeamCreate) GetCultureScore() int32`

GetCultureScore returns the CultureScore field if non-nil, zero value otherwise.

### GetCultureScoreOk

`func (o *TeamCreate) GetCultureScoreOk() (*int32, bool)`

GetCultureScoreOk returns a tuple with the CultureScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCultureScore

`func (o *TeamCreate) SetCultureScore(v int32)`

SetCultureScore sets CultureScore field to given value.


### GetFoundedYear

`func (o *TeamCreate) GetFoundedYear() int32`

GetFoundedYear returns the FoundedYear field if non-nil, zero value otherwise.

### GetFoundedYearOk

`func (o *TeamCreate) GetFoundedYearOk() (*int32, bool)`

GetFoundedYearOk returns a tuple with the FoundedYear field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFoundedYear

`func (o *TeamCreate) SetFoundedYear(v int32)`

SetFoundedYear sets FoundedYear field to given value.


### GetIsActive

`func (o *TeamCreate) GetIsActive() bool`

GetIsActive returns the IsActive field if non-nil, zero value otherwise.

### GetIsActiveOk

`func (o *TeamCreate) GetIsActiveOk() (*bool, bool)`

GetIsActiveOk returns a tuple with the IsActive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsActive

`func (o *TeamCreate) SetIsActive(v bool)`

SetIsActive sets IsActive field to given value.

### HasIsActive

`func (o *TeamCreate) HasIsActive() bool`

HasIsActive returns a boolean if a field has been set.

### GetLeague

`func (o *TeamCreate) GetLeague() League`

GetLeague returns the League field if non-nil, zero value otherwise.

### GetLeagueOk

`func (o *TeamCreate) GetLeagueOk() (*League, bool)`

GetLeagueOk returns a tuple with the League field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLeague

`func (o *TeamCreate) SetLeague(v League)`

SetLeague sets League field to given value.


### GetName

`func (o *TeamCreate) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *TeamCreate) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *TeamCreate) SetName(v string)`

SetName sets Name field to given value.


### GetNickname

`func (o *TeamCreate) GetNickname() string`

GetNickname returns the Nickname field if non-nil, zero value otherwise.

### GetNicknameOk

`func (o *TeamCreate) GetNicknameOk() (*string, bool)`

GetNicknameOk returns a tuple with the Nickname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNickname

`func (o *TeamCreate) SetNickname(v string)`

SetNickname sets Nickname field to given value.

### HasNickname

`func (o *TeamCreate) HasNickname() bool`

HasNickname returns a boolean if a field has been set.

### SetNicknameNil

`func (o *TeamCreate) SetNicknameNil(b bool)`

 SetNicknameNil sets the value for Nickname to be an explicit nil

### UnsetNickname
`func (o *TeamCreate) UnsetNickname()`

UnsetNickname ensures that no value is present for Nickname, not even an explicit nil
### GetPrimaryColor

`func (o *TeamCreate) GetPrimaryColor() string`

GetPrimaryColor returns the PrimaryColor field if non-nil, zero value otherwise.

### GetPrimaryColorOk

`func (o *TeamCreate) GetPrimaryColorOk() (*string, bool)`

GetPrimaryColorOk returns a tuple with the PrimaryColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrimaryColor

`func (o *TeamCreate) SetPrimaryColor(v string)`

SetPrimaryColor sets PrimaryColor field to given value.

### HasPrimaryColor

`func (o *TeamCreate) HasPrimaryColor() bool`

HasPrimaryColor returns a boolean if a field has been set.

### SetPrimaryColorNil

`func (o *TeamCreate) SetPrimaryColorNil(b bool)`

 SetPrimaryColorNil sets the value for PrimaryColor to be an explicit nil

### UnsetPrimaryColor
`func (o *TeamCreate) UnsetPrimaryColor()`

UnsetPrimaryColor ensures that no value is present for PrimaryColor, not even an explicit nil
### GetRivalTeams

`func (o *TeamCreate) GetRivalTeams() []string`

GetRivalTeams returns the RivalTeams field if non-nil, zero value otherwise.

### GetRivalTeamsOk

`func (o *TeamCreate) GetRivalTeamsOk() (*[]string, bool)`

GetRivalTeamsOk returns a tuple with the RivalTeams field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRivalTeams

`func (o *TeamCreate) SetRivalTeams(v []string)`

SetRivalTeams sets RivalTeams field to given value.

### HasRivalTeams

`func (o *TeamCreate) HasRivalTeams() bool`

HasRivalTeams returns a boolean if a field has been set.

### GetSecondaryColor

`func (o *TeamCreate) GetSecondaryColor() string`

GetSecondaryColor returns the SecondaryColor field if non-nil, zero value otherwise.

### GetSecondaryColorOk

`func (o *TeamCreate) GetSecondaryColorOk() (*string, bool)`

GetSecondaryColorOk returns a tuple with the SecondaryColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecondaryColor

`func (o *TeamCreate) SetSecondaryColor(v string)`

SetSecondaryColor sets SecondaryColor field to given value.

### HasSecondaryColor

`func (o *TeamCreate) HasSecondaryColor() bool`

HasSecondaryColor returns a boolean if a field has been set.

### SetSecondaryColorNil

`func (o *TeamCreate) SetSecondaryColorNil(b bool)`

 SetSecondaryColorNil sets the value for SecondaryColor to be an explicit nil

### UnsetSecondaryColor
`func (o *TeamCreate) UnsetSecondaryColor()`

UnsetSecondaryColor ensures that no value is present for SecondaryColor, not even an explicit nil
### GetStadium

`func (o *TeamCreate) GetStadium() string`

GetStadium returns the Stadium field if non-nil, zero value otherwise.

### GetStadiumOk

`func (o *TeamCreate) GetStadiumOk() (*string, bool)`

GetStadiumOk returns a tuple with the Stadium field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStadium

`func (o *TeamCreate) SetStadium(v string)`

SetStadium sets Stadium field to given value.


### GetStadiumLocation

`func (o *TeamCreate) GetStadiumLocation() GeoLocation`

GetStadiumLocation returns the StadiumLocation field if non-nil, zero value otherwise.

### GetStadiumLocationOk

`func (o *TeamCreate) GetStadiumLocationOk() (*GeoLocation, bool)`

GetStadiumLocationOk returns a tuple with the StadiumLocation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStadiumLocation

`func (o *TeamCreate) SetStadiumLocation(v GeoLocation)`

SetStadiumLocation sets StadiumLocation field to given value.

### HasStadiumLocation

`func (o *TeamCreate) HasStadiumLocation() bool`

HasStadiumLocation returns a boolean if a field has been set.

### SetStadiumLocationNil

`func (o *TeamCreate) SetStadiumLocationNil(b bool)`

 SetStadiumLocationNil sets the value for StadiumLocation to be an explicit nil

### UnsetStadiumLocation
`func (o *TeamCreate) UnsetStadiumLocation()`

UnsetStadiumLocation ensures that no value is present for StadiumLocation, not even an explicit nil
### GetValues

`func (o *TeamCreate) GetValues() TeamValues`

GetValues returns the Values field if non-nil, zero value otherwise.

### GetValuesOk

`func (o *TeamCreate) GetValuesOk() (*TeamValues, bool)`

GetValuesOk returns a tuple with the Values field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValues

`func (o *TeamCreate) SetValues(v TeamValues)`

SetValues sets Values field to given value.


### GetWebsite

`func (o *TeamCreate) GetWebsite() string`

GetWebsite returns the Website field if non-nil, zero value otherwise.

### GetWebsiteOk

`func (o *TeamCreate) GetWebsiteOk() (*string, bool)`

GetWebsiteOk returns a tuple with the Website field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebsite

`func (o *TeamCreate) SetWebsite(v string)`

SetWebsite sets Website field to given value.

### HasWebsite

`func (o *TeamCreate) HasWebsite() bool`

HasWebsite returns a boolean if a field has been set.

### SetWebsiteNil

`func (o *TeamCreate) SetWebsiteNil(b bool)`

 SetWebsiteNil sets the value for Website to be an explicit nil

### UnsetWebsite
`func (o *TeamCreate) UnsetWebsite()`

UnsetWebsite ensures that no value is present for Website, not even an explicit nil
### GetWinPercentage

`func (o *TeamCreate) GetWinPercentage() float32`

GetWinPercentage returns the WinPercentage field if non-nil, zero value otherwise.

### GetWinPercentageOk

`func (o *TeamCreate) GetWinPercentageOk() (*float32, bool)`

GetWinPercentageOk returns a tuple with the WinPercentage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWinPercentage

`func (o *TeamCreate) SetWinPercentage(v float32)`

SetWinPercentage sets WinPercentage field to given value.

### HasWinPercentage

`func (o *TeamCreate) HasWinPercentage() bool`

HasWinPercentage returns a boolean if a field has been set.

### SetWinPercentageNil

`func (o *TeamCreate) SetWinPercentageNil(b bool)`

 SetWinPercentageNil sets the value for WinPercentage to be an explicit nil

### UnsetWinPercentage
`func (o *TeamCreate) UnsetWinPercentage()`

UnsetWinPercentage ensures that no value is present for WinPercentage, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


