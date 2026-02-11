# MatchUpdate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Attendance** | Pointer to **NullableInt32** |  | [optional] 
**AwayScore** | Pointer to **NullableInt32** |  | [optional] 
**AwayTeamId** | Pointer to **NullableString** |  | [optional] 
**Date** | Pointer to **NullableTime** |  | [optional] 
**EpisodeId** | Pointer to **NullableString** |  | [optional] 
**HomeScore** | Pointer to **NullableInt32** |  | [optional] 
**HomeTeamId** | Pointer to **NullableString** |  | [optional] 
**LessonLearned** | Pointer to **NullableString** |  | [optional] 
**MatchType** | Pointer to [**NullableMatchType**](MatchType.md) |  | [optional] 
**PossessionPercentage** | Pointer to **NullableFloat32** |  | [optional] 
**Result** | Pointer to [**NullableMatchResult**](MatchResult.md) |  | [optional] 
**TedHalftimeSpeech** | Pointer to **NullableString** |  | [optional] 
**TicketRevenueGbp** | Pointer to [**NullableTicketRevenueGbp1**](TicketRevenueGbp1.md) |  | [optional] 
**TurningPoints** | Pointer to [**[]TurningPoint**](TurningPoint.md) |  | [optional] 
**WeatherTempCelsius** | Pointer to **NullableFloat32** |  | [optional] 

## Methods

### NewMatchUpdate

`func NewMatchUpdate() *MatchUpdate`

NewMatchUpdate instantiates a new MatchUpdate object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMatchUpdateWithDefaults

`func NewMatchUpdateWithDefaults() *MatchUpdate`

NewMatchUpdateWithDefaults instantiates a new MatchUpdate object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttendance

`func (o *MatchUpdate) GetAttendance() int32`

GetAttendance returns the Attendance field if non-nil, zero value otherwise.

### GetAttendanceOk

`func (o *MatchUpdate) GetAttendanceOk() (*int32, bool)`

GetAttendanceOk returns a tuple with the Attendance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttendance

`func (o *MatchUpdate) SetAttendance(v int32)`

SetAttendance sets Attendance field to given value.

### HasAttendance

`func (o *MatchUpdate) HasAttendance() bool`

HasAttendance returns a boolean if a field has been set.

### SetAttendanceNil

`func (o *MatchUpdate) SetAttendanceNil(b bool)`

 SetAttendanceNil sets the value for Attendance to be an explicit nil

### UnsetAttendance
`func (o *MatchUpdate) UnsetAttendance()`

UnsetAttendance ensures that no value is present for Attendance, not even an explicit nil
### GetAwayScore

`func (o *MatchUpdate) GetAwayScore() int32`

GetAwayScore returns the AwayScore field if non-nil, zero value otherwise.

### GetAwayScoreOk

`func (o *MatchUpdate) GetAwayScoreOk() (*int32, bool)`

GetAwayScoreOk returns a tuple with the AwayScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAwayScore

`func (o *MatchUpdate) SetAwayScore(v int32)`

SetAwayScore sets AwayScore field to given value.

### HasAwayScore

`func (o *MatchUpdate) HasAwayScore() bool`

HasAwayScore returns a boolean if a field has been set.

### SetAwayScoreNil

`func (o *MatchUpdate) SetAwayScoreNil(b bool)`

 SetAwayScoreNil sets the value for AwayScore to be an explicit nil

### UnsetAwayScore
`func (o *MatchUpdate) UnsetAwayScore()`

UnsetAwayScore ensures that no value is present for AwayScore, not even an explicit nil
### GetAwayTeamId

`func (o *MatchUpdate) GetAwayTeamId() string`

GetAwayTeamId returns the AwayTeamId field if non-nil, zero value otherwise.

### GetAwayTeamIdOk

`func (o *MatchUpdate) GetAwayTeamIdOk() (*string, bool)`

GetAwayTeamIdOk returns a tuple with the AwayTeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAwayTeamId

`func (o *MatchUpdate) SetAwayTeamId(v string)`

SetAwayTeamId sets AwayTeamId field to given value.

### HasAwayTeamId

`func (o *MatchUpdate) HasAwayTeamId() bool`

HasAwayTeamId returns a boolean if a field has been set.

### SetAwayTeamIdNil

`func (o *MatchUpdate) SetAwayTeamIdNil(b bool)`

 SetAwayTeamIdNil sets the value for AwayTeamId to be an explicit nil

### UnsetAwayTeamId
`func (o *MatchUpdate) UnsetAwayTeamId()`

UnsetAwayTeamId ensures that no value is present for AwayTeamId, not even an explicit nil
### GetDate

`func (o *MatchUpdate) GetDate() time.Time`

GetDate returns the Date field if non-nil, zero value otherwise.

### GetDateOk

`func (o *MatchUpdate) GetDateOk() (*time.Time, bool)`

GetDateOk returns a tuple with the Date field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDate

`func (o *MatchUpdate) SetDate(v time.Time)`

SetDate sets Date field to given value.

### HasDate

`func (o *MatchUpdate) HasDate() bool`

HasDate returns a boolean if a field has been set.

### SetDateNil

`func (o *MatchUpdate) SetDateNil(b bool)`

 SetDateNil sets the value for Date to be an explicit nil

### UnsetDate
`func (o *MatchUpdate) UnsetDate()`

UnsetDate ensures that no value is present for Date, not even an explicit nil
### GetEpisodeId

`func (o *MatchUpdate) GetEpisodeId() string`

GetEpisodeId returns the EpisodeId field if non-nil, zero value otherwise.

### GetEpisodeIdOk

`func (o *MatchUpdate) GetEpisodeIdOk() (*string, bool)`

GetEpisodeIdOk returns a tuple with the EpisodeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEpisodeId

`func (o *MatchUpdate) SetEpisodeId(v string)`

SetEpisodeId sets EpisodeId field to given value.

### HasEpisodeId

`func (o *MatchUpdate) HasEpisodeId() bool`

HasEpisodeId returns a boolean if a field has been set.

### SetEpisodeIdNil

`func (o *MatchUpdate) SetEpisodeIdNil(b bool)`

 SetEpisodeIdNil sets the value for EpisodeId to be an explicit nil

### UnsetEpisodeId
`func (o *MatchUpdate) UnsetEpisodeId()`

UnsetEpisodeId ensures that no value is present for EpisodeId, not even an explicit nil
### GetHomeScore

`func (o *MatchUpdate) GetHomeScore() int32`

GetHomeScore returns the HomeScore field if non-nil, zero value otherwise.

### GetHomeScoreOk

`func (o *MatchUpdate) GetHomeScoreOk() (*int32, bool)`

GetHomeScoreOk returns a tuple with the HomeScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHomeScore

`func (o *MatchUpdate) SetHomeScore(v int32)`

SetHomeScore sets HomeScore field to given value.

### HasHomeScore

`func (o *MatchUpdate) HasHomeScore() bool`

HasHomeScore returns a boolean if a field has been set.

### SetHomeScoreNil

`func (o *MatchUpdate) SetHomeScoreNil(b bool)`

 SetHomeScoreNil sets the value for HomeScore to be an explicit nil

### UnsetHomeScore
`func (o *MatchUpdate) UnsetHomeScore()`

UnsetHomeScore ensures that no value is present for HomeScore, not even an explicit nil
### GetHomeTeamId

`func (o *MatchUpdate) GetHomeTeamId() string`

GetHomeTeamId returns the HomeTeamId field if non-nil, zero value otherwise.

### GetHomeTeamIdOk

`func (o *MatchUpdate) GetHomeTeamIdOk() (*string, bool)`

GetHomeTeamIdOk returns a tuple with the HomeTeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHomeTeamId

`func (o *MatchUpdate) SetHomeTeamId(v string)`

SetHomeTeamId sets HomeTeamId field to given value.

### HasHomeTeamId

`func (o *MatchUpdate) HasHomeTeamId() bool`

HasHomeTeamId returns a boolean if a field has been set.

### SetHomeTeamIdNil

`func (o *MatchUpdate) SetHomeTeamIdNil(b bool)`

 SetHomeTeamIdNil sets the value for HomeTeamId to be an explicit nil

### UnsetHomeTeamId
`func (o *MatchUpdate) UnsetHomeTeamId()`

UnsetHomeTeamId ensures that no value is present for HomeTeamId, not even an explicit nil
### GetLessonLearned

`func (o *MatchUpdate) GetLessonLearned() string`

GetLessonLearned returns the LessonLearned field if non-nil, zero value otherwise.

### GetLessonLearnedOk

`func (o *MatchUpdate) GetLessonLearnedOk() (*string, bool)`

GetLessonLearnedOk returns a tuple with the LessonLearned field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLessonLearned

`func (o *MatchUpdate) SetLessonLearned(v string)`

SetLessonLearned sets LessonLearned field to given value.

### HasLessonLearned

`func (o *MatchUpdate) HasLessonLearned() bool`

HasLessonLearned returns a boolean if a field has been set.

### SetLessonLearnedNil

`func (o *MatchUpdate) SetLessonLearnedNil(b bool)`

 SetLessonLearnedNil sets the value for LessonLearned to be an explicit nil

### UnsetLessonLearned
`func (o *MatchUpdate) UnsetLessonLearned()`

UnsetLessonLearned ensures that no value is present for LessonLearned, not even an explicit nil
### GetMatchType

`func (o *MatchUpdate) GetMatchType() MatchType`

GetMatchType returns the MatchType field if non-nil, zero value otherwise.

### GetMatchTypeOk

`func (o *MatchUpdate) GetMatchTypeOk() (*MatchType, bool)`

GetMatchTypeOk returns a tuple with the MatchType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMatchType

`func (o *MatchUpdate) SetMatchType(v MatchType)`

SetMatchType sets MatchType field to given value.

### HasMatchType

`func (o *MatchUpdate) HasMatchType() bool`

HasMatchType returns a boolean if a field has been set.

### SetMatchTypeNil

`func (o *MatchUpdate) SetMatchTypeNil(b bool)`

 SetMatchTypeNil sets the value for MatchType to be an explicit nil

### UnsetMatchType
`func (o *MatchUpdate) UnsetMatchType()`

UnsetMatchType ensures that no value is present for MatchType, not even an explicit nil
### GetPossessionPercentage

`func (o *MatchUpdate) GetPossessionPercentage() float32`

GetPossessionPercentage returns the PossessionPercentage field if non-nil, zero value otherwise.

### GetPossessionPercentageOk

`func (o *MatchUpdate) GetPossessionPercentageOk() (*float32, bool)`

GetPossessionPercentageOk returns a tuple with the PossessionPercentage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPossessionPercentage

`func (o *MatchUpdate) SetPossessionPercentage(v float32)`

SetPossessionPercentage sets PossessionPercentage field to given value.

### HasPossessionPercentage

`func (o *MatchUpdate) HasPossessionPercentage() bool`

HasPossessionPercentage returns a boolean if a field has been set.

### SetPossessionPercentageNil

`func (o *MatchUpdate) SetPossessionPercentageNil(b bool)`

 SetPossessionPercentageNil sets the value for PossessionPercentage to be an explicit nil

### UnsetPossessionPercentage
`func (o *MatchUpdate) UnsetPossessionPercentage()`

UnsetPossessionPercentage ensures that no value is present for PossessionPercentage, not even an explicit nil
### GetResult

`func (o *MatchUpdate) GetResult() MatchResult`

GetResult returns the Result field if non-nil, zero value otherwise.

### GetResultOk

`func (o *MatchUpdate) GetResultOk() (*MatchResult, bool)`

GetResultOk returns a tuple with the Result field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResult

`func (o *MatchUpdate) SetResult(v MatchResult)`

SetResult sets Result field to given value.

### HasResult

`func (o *MatchUpdate) HasResult() bool`

HasResult returns a boolean if a field has been set.

### SetResultNil

`func (o *MatchUpdate) SetResultNil(b bool)`

 SetResultNil sets the value for Result to be an explicit nil

### UnsetResult
`func (o *MatchUpdate) UnsetResult()`

UnsetResult ensures that no value is present for Result, not even an explicit nil
### GetTedHalftimeSpeech

`func (o *MatchUpdate) GetTedHalftimeSpeech() string`

GetTedHalftimeSpeech returns the TedHalftimeSpeech field if non-nil, zero value otherwise.

### GetTedHalftimeSpeechOk

`func (o *MatchUpdate) GetTedHalftimeSpeechOk() (*string, bool)`

GetTedHalftimeSpeechOk returns a tuple with the TedHalftimeSpeech field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTedHalftimeSpeech

`func (o *MatchUpdate) SetTedHalftimeSpeech(v string)`

SetTedHalftimeSpeech sets TedHalftimeSpeech field to given value.

### HasTedHalftimeSpeech

`func (o *MatchUpdate) HasTedHalftimeSpeech() bool`

HasTedHalftimeSpeech returns a boolean if a field has been set.

### SetTedHalftimeSpeechNil

`func (o *MatchUpdate) SetTedHalftimeSpeechNil(b bool)`

 SetTedHalftimeSpeechNil sets the value for TedHalftimeSpeech to be an explicit nil

### UnsetTedHalftimeSpeech
`func (o *MatchUpdate) UnsetTedHalftimeSpeech()`

UnsetTedHalftimeSpeech ensures that no value is present for TedHalftimeSpeech, not even an explicit nil
### GetTicketRevenueGbp

`func (o *MatchUpdate) GetTicketRevenueGbp() TicketRevenueGbp1`

GetTicketRevenueGbp returns the TicketRevenueGbp field if non-nil, zero value otherwise.

### GetTicketRevenueGbpOk

`func (o *MatchUpdate) GetTicketRevenueGbpOk() (*TicketRevenueGbp1, bool)`

GetTicketRevenueGbpOk returns a tuple with the TicketRevenueGbp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTicketRevenueGbp

`func (o *MatchUpdate) SetTicketRevenueGbp(v TicketRevenueGbp1)`

SetTicketRevenueGbp sets TicketRevenueGbp field to given value.

### HasTicketRevenueGbp

`func (o *MatchUpdate) HasTicketRevenueGbp() bool`

HasTicketRevenueGbp returns a boolean if a field has been set.

### SetTicketRevenueGbpNil

`func (o *MatchUpdate) SetTicketRevenueGbpNil(b bool)`

 SetTicketRevenueGbpNil sets the value for TicketRevenueGbp to be an explicit nil

### UnsetTicketRevenueGbp
`func (o *MatchUpdate) UnsetTicketRevenueGbp()`

UnsetTicketRevenueGbp ensures that no value is present for TicketRevenueGbp, not even an explicit nil
### GetTurningPoints

`func (o *MatchUpdate) GetTurningPoints() []TurningPoint`

GetTurningPoints returns the TurningPoints field if non-nil, zero value otherwise.

### GetTurningPointsOk

`func (o *MatchUpdate) GetTurningPointsOk() (*[]TurningPoint, bool)`

GetTurningPointsOk returns a tuple with the TurningPoints field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTurningPoints

`func (o *MatchUpdate) SetTurningPoints(v []TurningPoint)`

SetTurningPoints sets TurningPoints field to given value.

### HasTurningPoints

`func (o *MatchUpdate) HasTurningPoints() bool`

HasTurningPoints returns a boolean if a field has been set.

### SetTurningPointsNil

`func (o *MatchUpdate) SetTurningPointsNil(b bool)`

 SetTurningPointsNil sets the value for TurningPoints to be an explicit nil

### UnsetTurningPoints
`func (o *MatchUpdate) UnsetTurningPoints()`

UnsetTurningPoints ensures that no value is present for TurningPoints, not even an explicit nil
### GetWeatherTempCelsius

`func (o *MatchUpdate) GetWeatherTempCelsius() float32`

GetWeatherTempCelsius returns the WeatherTempCelsius field if non-nil, zero value otherwise.

### GetWeatherTempCelsiusOk

`func (o *MatchUpdate) GetWeatherTempCelsiusOk() (*float32, bool)`

GetWeatherTempCelsiusOk returns a tuple with the WeatherTempCelsius field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWeatherTempCelsius

`func (o *MatchUpdate) SetWeatherTempCelsius(v float32)`

SetWeatherTempCelsius sets WeatherTempCelsius field to given value.

### HasWeatherTempCelsius

`func (o *MatchUpdate) HasWeatherTempCelsius() bool`

HasWeatherTempCelsius returns a boolean if a field has been set.

### SetWeatherTempCelsiusNil

`func (o *MatchUpdate) SetWeatherTempCelsiusNil(b bool)`

 SetWeatherTempCelsiusNil sets the value for WeatherTempCelsius to be an explicit nil

### UnsetWeatherTempCelsius
`func (o *MatchUpdate) UnsetWeatherTempCelsius()`

UnsetWeatherTempCelsius ensures that no value is present for WeatherTempCelsius, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


