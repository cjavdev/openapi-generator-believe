# MatchCompletedData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AwayScore** | **int32** | Final away team score | 
**AwayTeamId** | **string** | Away team ID | 
**CompletedAt** | **time.Time** | When the match completed | 
**HomeScore** | **int32** | Final home team score | 
**HomeTeamId** | **string** | Home team ID | 
**LessonLearned** | Pointer to **string** | Ted&#39;s lesson from the match | [optional] 
**ManOfTheMatch** | Pointer to **string** | Player of the match (if awarded) | [optional] 
**MatchId** | **string** | Unique match identifier | 
**MatchType** | **string** | Type of match | 
**Result** | **string** | Match result from home team perspective | 
**TedPostMatchQuote** | **string** | Ted&#39;s post-match wisdom | 

## Methods

### NewMatchCompletedData

`func NewMatchCompletedData(awayScore int32, awayTeamId string, completedAt time.Time, homeScore int32, homeTeamId string, matchId string, matchType string, result string, tedPostMatchQuote string, ) *MatchCompletedData`

NewMatchCompletedData instantiates a new MatchCompletedData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMatchCompletedDataWithDefaults

`func NewMatchCompletedDataWithDefaults() *MatchCompletedData`

NewMatchCompletedDataWithDefaults instantiates a new MatchCompletedData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAwayScore

`func (o *MatchCompletedData) GetAwayScore() int32`

GetAwayScore returns the AwayScore field if non-nil, zero value otherwise.

### GetAwayScoreOk

`func (o *MatchCompletedData) GetAwayScoreOk() (*int32, bool)`

GetAwayScoreOk returns a tuple with the AwayScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAwayScore

`func (o *MatchCompletedData) SetAwayScore(v int32)`

SetAwayScore sets AwayScore field to given value.


### GetAwayTeamId

`func (o *MatchCompletedData) GetAwayTeamId() string`

GetAwayTeamId returns the AwayTeamId field if non-nil, zero value otherwise.

### GetAwayTeamIdOk

`func (o *MatchCompletedData) GetAwayTeamIdOk() (*string, bool)`

GetAwayTeamIdOk returns a tuple with the AwayTeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAwayTeamId

`func (o *MatchCompletedData) SetAwayTeamId(v string)`

SetAwayTeamId sets AwayTeamId field to given value.


### GetCompletedAt

`func (o *MatchCompletedData) GetCompletedAt() time.Time`

GetCompletedAt returns the CompletedAt field if non-nil, zero value otherwise.

### GetCompletedAtOk

`func (o *MatchCompletedData) GetCompletedAtOk() (*time.Time, bool)`

GetCompletedAtOk returns a tuple with the CompletedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompletedAt

`func (o *MatchCompletedData) SetCompletedAt(v time.Time)`

SetCompletedAt sets CompletedAt field to given value.


### GetHomeScore

`func (o *MatchCompletedData) GetHomeScore() int32`

GetHomeScore returns the HomeScore field if non-nil, zero value otherwise.

### GetHomeScoreOk

`func (o *MatchCompletedData) GetHomeScoreOk() (*int32, bool)`

GetHomeScoreOk returns a tuple with the HomeScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHomeScore

`func (o *MatchCompletedData) SetHomeScore(v int32)`

SetHomeScore sets HomeScore field to given value.


### GetHomeTeamId

`func (o *MatchCompletedData) GetHomeTeamId() string`

GetHomeTeamId returns the HomeTeamId field if non-nil, zero value otherwise.

### GetHomeTeamIdOk

`func (o *MatchCompletedData) GetHomeTeamIdOk() (*string, bool)`

GetHomeTeamIdOk returns a tuple with the HomeTeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHomeTeamId

`func (o *MatchCompletedData) SetHomeTeamId(v string)`

SetHomeTeamId sets HomeTeamId field to given value.


### GetLessonLearned

`func (o *MatchCompletedData) GetLessonLearned() string`

GetLessonLearned returns the LessonLearned field if non-nil, zero value otherwise.

### GetLessonLearnedOk

`func (o *MatchCompletedData) GetLessonLearnedOk() (*string, bool)`

GetLessonLearnedOk returns a tuple with the LessonLearned field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLessonLearned

`func (o *MatchCompletedData) SetLessonLearned(v string)`

SetLessonLearned sets LessonLearned field to given value.

### HasLessonLearned

`func (o *MatchCompletedData) HasLessonLearned() bool`

HasLessonLearned returns a boolean if a field has been set.

### GetManOfTheMatch

`func (o *MatchCompletedData) GetManOfTheMatch() string`

GetManOfTheMatch returns the ManOfTheMatch field if non-nil, zero value otherwise.

### GetManOfTheMatchOk

`func (o *MatchCompletedData) GetManOfTheMatchOk() (*string, bool)`

GetManOfTheMatchOk returns a tuple with the ManOfTheMatch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetManOfTheMatch

`func (o *MatchCompletedData) SetManOfTheMatch(v string)`

SetManOfTheMatch sets ManOfTheMatch field to given value.

### HasManOfTheMatch

`func (o *MatchCompletedData) HasManOfTheMatch() bool`

HasManOfTheMatch returns a boolean if a field has been set.

### GetMatchId

`func (o *MatchCompletedData) GetMatchId() string`

GetMatchId returns the MatchId field if non-nil, zero value otherwise.

### GetMatchIdOk

`func (o *MatchCompletedData) GetMatchIdOk() (*string, bool)`

GetMatchIdOk returns a tuple with the MatchId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMatchId

`func (o *MatchCompletedData) SetMatchId(v string)`

SetMatchId sets MatchId field to given value.


### GetMatchType

`func (o *MatchCompletedData) GetMatchType() string`

GetMatchType returns the MatchType field if non-nil, zero value otherwise.

### GetMatchTypeOk

`func (o *MatchCompletedData) GetMatchTypeOk() (*string, bool)`

GetMatchTypeOk returns a tuple with the MatchType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMatchType

`func (o *MatchCompletedData) SetMatchType(v string)`

SetMatchType sets MatchType field to given value.


### GetResult

`func (o *MatchCompletedData) GetResult() string`

GetResult returns the Result field if non-nil, zero value otherwise.

### GetResultOk

`func (o *MatchCompletedData) GetResultOk() (*string, bool)`

GetResultOk returns a tuple with the Result field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResult

`func (o *MatchCompletedData) SetResult(v string)`

SetResult sets Result field to given value.


### GetTedPostMatchQuote

`func (o *MatchCompletedData) GetTedPostMatchQuote() string`

GetTedPostMatchQuote returns the TedPostMatchQuote field if non-nil, zero value otherwise.

### GetTedPostMatchQuoteOk

`func (o *MatchCompletedData) GetTedPostMatchQuoteOk() (*string, bool)`

GetTedPostMatchQuoteOk returns a tuple with the TedPostMatchQuote field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTedPostMatchQuote

`func (o *MatchCompletedData) SetTedPostMatchQuote(v string)`

SetTedPostMatchQuote sets TedPostMatchQuote field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


