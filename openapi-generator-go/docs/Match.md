# Match

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Attendance** | Pointer to **NullableInt32** |  | [optional] 
**AwayScore** | Pointer to **int32** | Away team score | [optional] [default to 0]
**AwayTeamId** | **string** | Away team ID | 
**Date** | **time.Time** | Match date and time | 
**EpisodeId** | Pointer to **NullableString** |  | [optional] 
**HomeScore** | Pointer to **int32** | Home team score | [optional] [default to 0]
**HomeTeamId** | **string** | Home team ID | 
**Id** | **string** | Unique identifier | 
**LessonLearned** | Pointer to **NullableString** |  | [optional] 
**MatchType** | [**MatchType**](MatchType.md) | Type of match | 
**PossessionPercentage** | Pointer to **NullableFloat32** |  | [optional] 
**Result** | Pointer to [**MatchResult**](MatchResult.md) | Match result from home team perspective | [optional] [default to PENDING]
**TedHalftimeSpeech** | Pointer to **NullableString** |  | [optional] 
**TicketRevenueGbp** | Pointer to **NullableString** |  | [optional] 
**TurningPoints** | Pointer to [**[]TurningPoint**](TurningPoint.md) | Key moments that changed the match | [optional] 
**WeatherTempCelsius** | Pointer to **NullableFloat32** |  | [optional] 

## Methods

### NewMatch

`func NewMatch(awayTeamId string, date time.Time, homeTeamId string, id string, matchType MatchType, ) *Match`

NewMatch instantiates a new Match object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMatchWithDefaults

`func NewMatchWithDefaults() *Match`

NewMatchWithDefaults instantiates a new Match object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttendance

`func (o *Match) GetAttendance() int32`

GetAttendance returns the Attendance field if non-nil, zero value otherwise.

### GetAttendanceOk

`func (o *Match) GetAttendanceOk() (*int32, bool)`

GetAttendanceOk returns a tuple with the Attendance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttendance

`func (o *Match) SetAttendance(v int32)`

SetAttendance sets Attendance field to given value.

### HasAttendance

`func (o *Match) HasAttendance() bool`

HasAttendance returns a boolean if a field has been set.

### SetAttendanceNil

`func (o *Match) SetAttendanceNil(b bool)`

 SetAttendanceNil sets the value for Attendance to be an explicit nil

### UnsetAttendance
`func (o *Match) UnsetAttendance()`

UnsetAttendance ensures that no value is present for Attendance, not even an explicit nil
### GetAwayScore

`func (o *Match) GetAwayScore() int32`

GetAwayScore returns the AwayScore field if non-nil, zero value otherwise.

### GetAwayScoreOk

`func (o *Match) GetAwayScoreOk() (*int32, bool)`

GetAwayScoreOk returns a tuple with the AwayScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAwayScore

`func (o *Match) SetAwayScore(v int32)`

SetAwayScore sets AwayScore field to given value.

### HasAwayScore

`func (o *Match) HasAwayScore() bool`

HasAwayScore returns a boolean if a field has been set.

### GetAwayTeamId

`func (o *Match) GetAwayTeamId() string`

GetAwayTeamId returns the AwayTeamId field if non-nil, zero value otherwise.

### GetAwayTeamIdOk

`func (o *Match) GetAwayTeamIdOk() (*string, bool)`

GetAwayTeamIdOk returns a tuple with the AwayTeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAwayTeamId

`func (o *Match) SetAwayTeamId(v string)`

SetAwayTeamId sets AwayTeamId field to given value.


### GetDate

`func (o *Match) GetDate() time.Time`

GetDate returns the Date field if non-nil, zero value otherwise.

### GetDateOk

`func (o *Match) GetDateOk() (*time.Time, bool)`

GetDateOk returns a tuple with the Date field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDate

`func (o *Match) SetDate(v time.Time)`

SetDate sets Date field to given value.


### GetEpisodeId

`func (o *Match) GetEpisodeId() string`

GetEpisodeId returns the EpisodeId field if non-nil, zero value otherwise.

### GetEpisodeIdOk

`func (o *Match) GetEpisodeIdOk() (*string, bool)`

GetEpisodeIdOk returns a tuple with the EpisodeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEpisodeId

`func (o *Match) SetEpisodeId(v string)`

SetEpisodeId sets EpisodeId field to given value.

### HasEpisodeId

`func (o *Match) HasEpisodeId() bool`

HasEpisodeId returns a boolean if a field has been set.

### SetEpisodeIdNil

`func (o *Match) SetEpisodeIdNil(b bool)`

 SetEpisodeIdNil sets the value for EpisodeId to be an explicit nil

### UnsetEpisodeId
`func (o *Match) UnsetEpisodeId()`

UnsetEpisodeId ensures that no value is present for EpisodeId, not even an explicit nil
### GetHomeScore

`func (o *Match) GetHomeScore() int32`

GetHomeScore returns the HomeScore field if non-nil, zero value otherwise.

### GetHomeScoreOk

`func (o *Match) GetHomeScoreOk() (*int32, bool)`

GetHomeScoreOk returns a tuple with the HomeScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHomeScore

`func (o *Match) SetHomeScore(v int32)`

SetHomeScore sets HomeScore field to given value.

### HasHomeScore

`func (o *Match) HasHomeScore() bool`

HasHomeScore returns a boolean if a field has been set.

### GetHomeTeamId

`func (o *Match) GetHomeTeamId() string`

GetHomeTeamId returns the HomeTeamId field if non-nil, zero value otherwise.

### GetHomeTeamIdOk

`func (o *Match) GetHomeTeamIdOk() (*string, bool)`

GetHomeTeamIdOk returns a tuple with the HomeTeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHomeTeamId

`func (o *Match) SetHomeTeamId(v string)`

SetHomeTeamId sets HomeTeamId field to given value.


### GetId

`func (o *Match) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Match) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Match) SetId(v string)`

SetId sets Id field to given value.


### GetLessonLearned

`func (o *Match) GetLessonLearned() string`

GetLessonLearned returns the LessonLearned field if non-nil, zero value otherwise.

### GetLessonLearnedOk

`func (o *Match) GetLessonLearnedOk() (*string, bool)`

GetLessonLearnedOk returns a tuple with the LessonLearned field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLessonLearned

`func (o *Match) SetLessonLearned(v string)`

SetLessonLearned sets LessonLearned field to given value.

### HasLessonLearned

`func (o *Match) HasLessonLearned() bool`

HasLessonLearned returns a boolean if a field has been set.

### SetLessonLearnedNil

`func (o *Match) SetLessonLearnedNil(b bool)`

 SetLessonLearnedNil sets the value for LessonLearned to be an explicit nil

### UnsetLessonLearned
`func (o *Match) UnsetLessonLearned()`

UnsetLessonLearned ensures that no value is present for LessonLearned, not even an explicit nil
### GetMatchType

`func (o *Match) GetMatchType() MatchType`

GetMatchType returns the MatchType field if non-nil, zero value otherwise.

### GetMatchTypeOk

`func (o *Match) GetMatchTypeOk() (*MatchType, bool)`

GetMatchTypeOk returns a tuple with the MatchType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMatchType

`func (o *Match) SetMatchType(v MatchType)`

SetMatchType sets MatchType field to given value.


### GetPossessionPercentage

`func (o *Match) GetPossessionPercentage() float32`

GetPossessionPercentage returns the PossessionPercentage field if non-nil, zero value otherwise.

### GetPossessionPercentageOk

`func (o *Match) GetPossessionPercentageOk() (*float32, bool)`

GetPossessionPercentageOk returns a tuple with the PossessionPercentage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPossessionPercentage

`func (o *Match) SetPossessionPercentage(v float32)`

SetPossessionPercentage sets PossessionPercentage field to given value.

### HasPossessionPercentage

`func (o *Match) HasPossessionPercentage() bool`

HasPossessionPercentage returns a boolean if a field has been set.

### SetPossessionPercentageNil

`func (o *Match) SetPossessionPercentageNil(b bool)`

 SetPossessionPercentageNil sets the value for PossessionPercentage to be an explicit nil

### UnsetPossessionPercentage
`func (o *Match) UnsetPossessionPercentage()`

UnsetPossessionPercentage ensures that no value is present for PossessionPercentage, not even an explicit nil
### GetResult

`func (o *Match) GetResult() MatchResult`

GetResult returns the Result field if non-nil, zero value otherwise.

### GetResultOk

`func (o *Match) GetResultOk() (*MatchResult, bool)`

GetResultOk returns a tuple with the Result field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResult

`func (o *Match) SetResult(v MatchResult)`

SetResult sets Result field to given value.

### HasResult

`func (o *Match) HasResult() bool`

HasResult returns a boolean if a field has been set.

### GetTedHalftimeSpeech

`func (o *Match) GetTedHalftimeSpeech() string`

GetTedHalftimeSpeech returns the TedHalftimeSpeech field if non-nil, zero value otherwise.

### GetTedHalftimeSpeechOk

`func (o *Match) GetTedHalftimeSpeechOk() (*string, bool)`

GetTedHalftimeSpeechOk returns a tuple with the TedHalftimeSpeech field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTedHalftimeSpeech

`func (o *Match) SetTedHalftimeSpeech(v string)`

SetTedHalftimeSpeech sets TedHalftimeSpeech field to given value.

### HasTedHalftimeSpeech

`func (o *Match) HasTedHalftimeSpeech() bool`

HasTedHalftimeSpeech returns a boolean if a field has been set.

### SetTedHalftimeSpeechNil

`func (o *Match) SetTedHalftimeSpeechNil(b bool)`

 SetTedHalftimeSpeechNil sets the value for TedHalftimeSpeech to be an explicit nil

### UnsetTedHalftimeSpeech
`func (o *Match) UnsetTedHalftimeSpeech()`

UnsetTedHalftimeSpeech ensures that no value is present for TedHalftimeSpeech, not even an explicit nil
### GetTicketRevenueGbp

`func (o *Match) GetTicketRevenueGbp() string`

GetTicketRevenueGbp returns the TicketRevenueGbp field if non-nil, zero value otherwise.

### GetTicketRevenueGbpOk

`func (o *Match) GetTicketRevenueGbpOk() (*string, bool)`

GetTicketRevenueGbpOk returns a tuple with the TicketRevenueGbp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTicketRevenueGbp

`func (o *Match) SetTicketRevenueGbp(v string)`

SetTicketRevenueGbp sets TicketRevenueGbp field to given value.

### HasTicketRevenueGbp

`func (o *Match) HasTicketRevenueGbp() bool`

HasTicketRevenueGbp returns a boolean if a field has been set.

### SetTicketRevenueGbpNil

`func (o *Match) SetTicketRevenueGbpNil(b bool)`

 SetTicketRevenueGbpNil sets the value for TicketRevenueGbp to be an explicit nil

### UnsetTicketRevenueGbp
`func (o *Match) UnsetTicketRevenueGbp()`

UnsetTicketRevenueGbp ensures that no value is present for TicketRevenueGbp, not even an explicit nil
### GetTurningPoints

`func (o *Match) GetTurningPoints() []TurningPoint`

GetTurningPoints returns the TurningPoints field if non-nil, zero value otherwise.

### GetTurningPointsOk

`func (o *Match) GetTurningPointsOk() (*[]TurningPoint, bool)`

GetTurningPointsOk returns a tuple with the TurningPoints field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTurningPoints

`func (o *Match) SetTurningPoints(v []TurningPoint)`

SetTurningPoints sets TurningPoints field to given value.

### HasTurningPoints

`func (o *Match) HasTurningPoints() bool`

HasTurningPoints returns a boolean if a field has been set.

### GetWeatherTempCelsius

`func (o *Match) GetWeatherTempCelsius() float32`

GetWeatherTempCelsius returns the WeatherTempCelsius field if non-nil, zero value otherwise.

### GetWeatherTempCelsiusOk

`func (o *Match) GetWeatherTempCelsiusOk() (*float32, bool)`

GetWeatherTempCelsiusOk returns a tuple with the WeatherTempCelsius field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWeatherTempCelsius

`func (o *Match) SetWeatherTempCelsius(v float32)`

SetWeatherTempCelsius sets WeatherTempCelsius field to given value.

### HasWeatherTempCelsius

`func (o *Match) HasWeatherTempCelsius() bool`

HasWeatherTempCelsius returns a boolean if a field has been set.

### SetWeatherTempCelsiusNil

`func (o *Match) SetWeatherTempCelsiusNil(b bool)`

 SetWeatherTempCelsiusNil sets the value for WeatherTempCelsius to be an explicit nil

### UnsetWeatherTempCelsius
`func (o *Match) UnsetWeatherTempCelsius()`

UnsetWeatherTempCelsius ensures that no value is present for WeatherTempCelsius, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


