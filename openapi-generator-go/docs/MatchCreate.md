# MatchCreate

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
**LessonLearned** | Pointer to **NullableString** |  | [optional] 
**MatchType** | [**MatchType**](MatchType.md) | Type of match | 
**PossessionPercentage** | Pointer to **NullableFloat32** |  | [optional] 
**Result** | Pointer to [**MatchResult**](MatchResult.md) | Match result from home team perspective | [optional] [default to PENDING]
**TedHalftimeSpeech** | Pointer to **NullableString** |  | [optional] 
**TicketRevenueGbp** | Pointer to [**NullableTicketRevenueGbp**](TicketRevenueGbp.md) |  | [optional] 
**TurningPoints** | Pointer to [**[]TurningPoint**](TurningPoint.md) | Key moments that changed the match | [optional] 
**WeatherTempCelsius** | Pointer to **NullableFloat32** |  | [optional] 

## Methods

### NewMatchCreate

`func NewMatchCreate(awayTeamId string, date time.Time, homeTeamId string, matchType MatchType, ) *MatchCreate`

NewMatchCreate instantiates a new MatchCreate object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMatchCreateWithDefaults

`func NewMatchCreateWithDefaults() *MatchCreate`

NewMatchCreateWithDefaults instantiates a new MatchCreate object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttendance

`func (o *MatchCreate) GetAttendance() int32`

GetAttendance returns the Attendance field if non-nil, zero value otherwise.

### GetAttendanceOk

`func (o *MatchCreate) GetAttendanceOk() (*int32, bool)`

GetAttendanceOk returns a tuple with the Attendance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttendance

`func (o *MatchCreate) SetAttendance(v int32)`

SetAttendance sets Attendance field to given value.

### HasAttendance

`func (o *MatchCreate) HasAttendance() bool`

HasAttendance returns a boolean if a field has been set.

### SetAttendanceNil

`func (o *MatchCreate) SetAttendanceNil(b bool)`

 SetAttendanceNil sets the value for Attendance to be an explicit nil

### UnsetAttendance
`func (o *MatchCreate) UnsetAttendance()`

UnsetAttendance ensures that no value is present for Attendance, not even an explicit nil
### GetAwayScore

`func (o *MatchCreate) GetAwayScore() int32`

GetAwayScore returns the AwayScore field if non-nil, zero value otherwise.

### GetAwayScoreOk

`func (o *MatchCreate) GetAwayScoreOk() (*int32, bool)`

GetAwayScoreOk returns a tuple with the AwayScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAwayScore

`func (o *MatchCreate) SetAwayScore(v int32)`

SetAwayScore sets AwayScore field to given value.

### HasAwayScore

`func (o *MatchCreate) HasAwayScore() bool`

HasAwayScore returns a boolean if a field has been set.

### GetAwayTeamId

`func (o *MatchCreate) GetAwayTeamId() string`

GetAwayTeamId returns the AwayTeamId field if non-nil, zero value otherwise.

### GetAwayTeamIdOk

`func (o *MatchCreate) GetAwayTeamIdOk() (*string, bool)`

GetAwayTeamIdOk returns a tuple with the AwayTeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAwayTeamId

`func (o *MatchCreate) SetAwayTeamId(v string)`

SetAwayTeamId sets AwayTeamId field to given value.


### GetDate

`func (o *MatchCreate) GetDate() time.Time`

GetDate returns the Date field if non-nil, zero value otherwise.

### GetDateOk

`func (o *MatchCreate) GetDateOk() (*time.Time, bool)`

GetDateOk returns a tuple with the Date field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDate

`func (o *MatchCreate) SetDate(v time.Time)`

SetDate sets Date field to given value.


### GetEpisodeId

`func (o *MatchCreate) GetEpisodeId() string`

GetEpisodeId returns the EpisodeId field if non-nil, zero value otherwise.

### GetEpisodeIdOk

`func (o *MatchCreate) GetEpisodeIdOk() (*string, bool)`

GetEpisodeIdOk returns a tuple with the EpisodeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEpisodeId

`func (o *MatchCreate) SetEpisodeId(v string)`

SetEpisodeId sets EpisodeId field to given value.

### HasEpisodeId

`func (o *MatchCreate) HasEpisodeId() bool`

HasEpisodeId returns a boolean if a field has been set.

### SetEpisodeIdNil

`func (o *MatchCreate) SetEpisodeIdNil(b bool)`

 SetEpisodeIdNil sets the value for EpisodeId to be an explicit nil

### UnsetEpisodeId
`func (o *MatchCreate) UnsetEpisodeId()`

UnsetEpisodeId ensures that no value is present for EpisodeId, not even an explicit nil
### GetHomeScore

`func (o *MatchCreate) GetHomeScore() int32`

GetHomeScore returns the HomeScore field if non-nil, zero value otherwise.

### GetHomeScoreOk

`func (o *MatchCreate) GetHomeScoreOk() (*int32, bool)`

GetHomeScoreOk returns a tuple with the HomeScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHomeScore

`func (o *MatchCreate) SetHomeScore(v int32)`

SetHomeScore sets HomeScore field to given value.

### HasHomeScore

`func (o *MatchCreate) HasHomeScore() bool`

HasHomeScore returns a boolean if a field has been set.

### GetHomeTeamId

`func (o *MatchCreate) GetHomeTeamId() string`

GetHomeTeamId returns the HomeTeamId field if non-nil, zero value otherwise.

### GetHomeTeamIdOk

`func (o *MatchCreate) GetHomeTeamIdOk() (*string, bool)`

GetHomeTeamIdOk returns a tuple with the HomeTeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHomeTeamId

`func (o *MatchCreate) SetHomeTeamId(v string)`

SetHomeTeamId sets HomeTeamId field to given value.


### GetLessonLearned

`func (o *MatchCreate) GetLessonLearned() string`

GetLessonLearned returns the LessonLearned field if non-nil, zero value otherwise.

### GetLessonLearnedOk

`func (o *MatchCreate) GetLessonLearnedOk() (*string, bool)`

GetLessonLearnedOk returns a tuple with the LessonLearned field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLessonLearned

`func (o *MatchCreate) SetLessonLearned(v string)`

SetLessonLearned sets LessonLearned field to given value.

### HasLessonLearned

`func (o *MatchCreate) HasLessonLearned() bool`

HasLessonLearned returns a boolean if a field has been set.

### SetLessonLearnedNil

`func (o *MatchCreate) SetLessonLearnedNil(b bool)`

 SetLessonLearnedNil sets the value for LessonLearned to be an explicit nil

### UnsetLessonLearned
`func (o *MatchCreate) UnsetLessonLearned()`

UnsetLessonLearned ensures that no value is present for LessonLearned, not even an explicit nil
### GetMatchType

`func (o *MatchCreate) GetMatchType() MatchType`

GetMatchType returns the MatchType field if non-nil, zero value otherwise.

### GetMatchTypeOk

`func (o *MatchCreate) GetMatchTypeOk() (*MatchType, bool)`

GetMatchTypeOk returns a tuple with the MatchType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMatchType

`func (o *MatchCreate) SetMatchType(v MatchType)`

SetMatchType sets MatchType field to given value.


### GetPossessionPercentage

`func (o *MatchCreate) GetPossessionPercentage() float32`

GetPossessionPercentage returns the PossessionPercentage field if non-nil, zero value otherwise.

### GetPossessionPercentageOk

`func (o *MatchCreate) GetPossessionPercentageOk() (*float32, bool)`

GetPossessionPercentageOk returns a tuple with the PossessionPercentage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPossessionPercentage

`func (o *MatchCreate) SetPossessionPercentage(v float32)`

SetPossessionPercentage sets PossessionPercentage field to given value.

### HasPossessionPercentage

`func (o *MatchCreate) HasPossessionPercentage() bool`

HasPossessionPercentage returns a boolean if a field has been set.

### SetPossessionPercentageNil

`func (o *MatchCreate) SetPossessionPercentageNil(b bool)`

 SetPossessionPercentageNil sets the value for PossessionPercentage to be an explicit nil

### UnsetPossessionPercentage
`func (o *MatchCreate) UnsetPossessionPercentage()`

UnsetPossessionPercentage ensures that no value is present for PossessionPercentage, not even an explicit nil
### GetResult

`func (o *MatchCreate) GetResult() MatchResult`

GetResult returns the Result field if non-nil, zero value otherwise.

### GetResultOk

`func (o *MatchCreate) GetResultOk() (*MatchResult, bool)`

GetResultOk returns a tuple with the Result field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResult

`func (o *MatchCreate) SetResult(v MatchResult)`

SetResult sets Result field to given value.

### HasResult

`func (o *MatchCreate) HasResult() bool`

HasResult returns a boolean if a field has been set.

### GetTedHalftimeSpeech

`func (o *MatchCreate) GetTedHalftimeSpeech() string`

GetTedHalftimeSpeech returns the TedHalftimeSpeech field if non-nil, zero value otherwise.

### GetTedHalftimeSpeechOk

`func (o *MatchCreate) GetTedHalftimeSpeechOk() (*string, bool)`

GetTedHalftimeSpeechOk returns a tuple with the TedHalftimeSpeech field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTedHalftimeSpeech

`func (o *MatchCreate) SetTedHalftimeSpeech(v string)`

SetTedHalftimeSpeech sets TedHalftimeSpeech field to given value.

### HasTedHalftimeSpeech

`func (o *MatchCreate) HasTedHalftimeSpeech() bool`

HasTedHalftimeSpeech returns a boolean if a field has been set.

### SetTedHalftimeSpeechNil

`func (o *MatchCreate) SetTedHalftimeSpeechNil(b bool)`

 SetTedHalftimeSpeechNil sets the value for TedHalftimeSpeech to be an explicit nil

### UnsetTedHalftimeSpeech
`func (o *MatchCreate) UnsetTedHalftimeSpeech()`

UnsetTedHalftimeSpeech ensures that no value is present for TedHalftimeSpeech, not even an explicit nil
### GetTicketRevenueGbp

`func (o *MatchCreate) GetTicketRevenueGbp() TicketRevenueGbp`

GetTicketRevenueGbp returns the TicketRevenueGbp field if non-nil, zero value otherwise.

### GetTicketRevenueGbpOk

`func (o *MatchCreate) GetTicketRevenueGbpOk() (*TicketRevenueGbp, bool)`

GetTicketRevenueGbpOk returns a tuple with the TicketRevenueGbp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTicketRevenueGbp

`func (o *MatchCreate) SetTicketRevenueGbp(v TicketRevenueGbp)`

SetTicketRevenueGbp sets TicketRevenueGbp field to given value.

### HasTicketRevenueGbp

`func (o *MatchCreate) HasTicketRevenueGbp() bool`

HasTicketRevenueGbp returns a boolean if a field has been set.

### SetTicketRevenueGbpNil

`func (o *MatchCreate) SetTicketRevenueGbpNil(b bool)`

 SetTicketRevenueGbpNil sets the value for TicketRevenueGbp to be an explicit nil

### UnsetTicketRevenueGbp
`func (o *MatchCreate) UnsetTicketRevenueGbp()`

UnsetTicketRevenueGbp ensures that no value is present for TicketRevenueGbp, not even an explicit nil
### GetTurningPoints

`func (o *MatchCreate) GetTurningPoints() []TurningPoint`

GetTurningPoints returns the TurningPoints field if non-nil, zero value otherwise.

### GetTurningPointsOk

`func (o *MatchCreate) GetTurningPointsOk() (*[]TurningPoint, bool)`

GetTurningPointsOk returns a tuple with the TurningPoints field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTurningPoints

`func (o *MatchCreate) SetTurningPoints(v []TurningPoint)`

SetTurningPoints sets TurningPoints field to given value.

### HasTurningPoints

`func (o *MatchCreate) HasTurningPoints() bool`

HasTurningPoints returns a boolean if a field has been set.

### GetWeatherTempCelsius

`func (o *MatchCreate) GetWeatherTempCelsius() float32`

GetWeatherTempCelsius returns the WeatherTempCelsius field if non-nil, zero value otherwise.

### GetWeatherTempCelsiusOk

`func (o *MatchCreate) GetWeatherTempCelsiusOk() (*float32, bool)`

GetWeatherTempCelsiusOk returns a tuple with the WeatherTempCelsius field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWeatherTempCelsius

`func (o *MatchCreate) SetWeatherTempCelsius(v float32)`

SetWeatherTempCelsius sets WeatherTempCelsius field to given value.

### HasWeatherTempCelsius

`func (o *MatchCreate) HasWeatherTempCelsius() bool`

HasWeatherTempCelsius returns a boolean if a field has been set.

### SetWeatherTempCelsiusNil

`func (o *MatchCreate) SetWeatherTempCelsiusNil(b bool)`

 SetWeatherTempCelsiusNil sets the value for WeatherTempCelsius to be an explicit nil

### UnsetWeatherTempCelsius
`func (o *MatchCreate) UnsetWeatherTempCelsius()`

UnsetWeatherTempCelsius ensures that no value is present for WeatherTempCelsius, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


