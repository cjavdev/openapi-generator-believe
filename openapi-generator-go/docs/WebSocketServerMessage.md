# WebSocketServerMessage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AwayTeam** | **string** | Away team name | 
**HomeTeam** | **string** | Home team name | 
**MatchId** | **string** | Match identifier | 
**Message** | **string** | Error description | 
**Type** | **string** | Message type | 
**Event** | [**WebSocketLiveMatchEvent**](WebSocketLiveMatchEvent.md) |  | 
**FinalScore** | [**WebSocketMatchScore**](WebSocketMatchScore.md) |  | 
**FinalStats** | [**WebSocketMatchStats**](WebSocketMatchStats.md) |  | 
**ManOfTheMatch** | **string** | Man of the match | 
**TedPostMatch** | **string** | Ted&#39;s post-match thoughts | 
**Code** | **string** | Error code | 

## Methods

### NewWebSocketServerMessage

`func NewWebSocketServerMessage(awayTeam string, homeTeam string, matchId string, message string, type_ string, event WebSocketLiveMatchEvent, finalScore WebSocketMatchScore, finalStats WebSocketMatchStats, manOfTheMatch string, tedPostMatch string, code string, ) *WebSocketServerMessage`

NewWebSocketServerMessage instantiates a new WebSocketServerMessage object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebSocketServerMessageWithDefaults

`func NewWebSocketServerMessageWithDefaults() *WebSocketServerMessage`

NewWebSocketServerMessageWithDefaults instantiates a new WebSocketServerMessage object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAwayTeam

`func (o *WebSocketServerMessage) GetAwayTeam() string`

GetAwayTeam returns the AwayTeam field if non-nil, zero value otherwise.

### GetAwayTeamOk

`func (o *WebSocketServerMessage) GetAwayTeamOk() (*string, bool)`

GetAwayTeamOk returns a tuple with the AwayTeam field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAwayTeam

`func (o *WebSocketServerMessage) SetAwayTeam(v string)`

SetAwayTeam sets AwayTeam field to given value.


### GetHomeTeam

`func (o *WebSocketServerMessage) GetHomeTeam() string`

GetHomeTeam returns the HomeTeam field if non-nil, zero value otherwise.

### GetHomeTeamOk

`func (o *WebSocketServerMessage) GetHomeTeamOk() (*string, bool)`

GetHomeTeamOk returns a tuple with the HomeTeam field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHomeTeam

`func (o *WebSocketServerMessage) SetHomeTeam(v string)`

SetHomeTeam sets HomeTeam field to given value.


### GetMatchId

`func (o *WebSocketServerMessage) GetMatchId() string`

GetMatchId returns the MatchId field if non-nil, zero value otherwise.

### GetMatchIdOk

`func (o *WebSocketServerMessage) GetMatchIdOk() (*string, bool)`

GetMatchIdOk returns a tuple with the MatchId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMatchId

`func (o *WebSocketServerMessage) SetMatchId(v string)`

SetMatchId sets MatchId field to given value.


### GetMessage

`func (o *WebSocketServerMessage) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *WebSocketServerMessage) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *WebSocketServerMessage) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetType

`func (o *WebSocketServerMessage) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *WebSocketServerMessage) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *WebSocketServerMessage) SetType(v string)`

SetType sets Type field to given value.


### GetEvent

`func (o *WebSocketServerMessage) GetEvent() WebSocketLiveMatchEvent`

GetEvent returns the Event field if non-nil, zero value otherwise.

### GetEventOk

`func (o *WebSocketServerMessage) GetEventOk() (*WebSocketLiveMatchEvent, bool)`

GetEventOk returns a tuple with the Event field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEvent

`func (o *WebSocketServerMessage) SetEvent(v WebSocketLiveMatchEvent)`

SetEvent sets Event field to given value.


### GetFinalScore

`func (o *WebSocketServerMessage) GetFinalScore() WebSocketMatchScore`

GetFinalScore returns the FinalScore field if non-nil, zero value otherwise.

### GetFinalScoreOk

`func (o *WebSocketServerMessage) GetFinalScoreOk() (*WebSocketMatchScore, bool)`

GetFinalScoreOk returns a tuple with the FinalScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFinalScore

`func (o *WebSocketServerMessage) SetFinalScore(v WebSocketMatchScore)`

SetFinalScore sets FinalScore field to given value.


### GetFinalStats

`func (o *WebSocketServerMessage) GetFinalStats() WebSocketMatchStats`

GetFinalStats returns the FinalStats field if non-nil, zero value otherwise.

### GetFinalStatsOk

`func (o *WebSocketServerMessage) GetFinalStatsOk() (*WebSocketMatchStats, bool)`

GetFinalStatsOk returns a tuple with the FinalStats field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFinalStats

`func (o *WebSocketServerMessage) SetFinalStats(v WebSocketMatchStats)`

SetFinalStats sets FinalStats field to given value.


### GetManOfTheMatch

`func (o *WebSocketServerMessage) GetManOfTheMatch() string`

GetManOfTheMatch returns the ManOfTheMatch field if non-nil, zero value otherwise.

### GetManOfTheMatchOk

`func (o *WebSocketServerMessage) GetManOfTheMatchOk() (*string, bool)`

GetManOfTheMatchOk returns a tuple with the ManOfTheMatch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetManOfTheMatch

`func (o *WebSocketServerMessage) SetManOfTheMatch(v string)`

SetManOfTheMatch sets ManOfTheMatch field to given value.


### GetTedPostMatch

`func (o *WebSocketServerMessage) GetTedPostMatch() string`

GetTedPostMatch returns the TedPostMatch field if non-nil, zero value otherwise.

### GetTedPostMatchOk

`func (o *WebSocketServerMessage) GetTedPostMatchOk() (*string, bool)`

GetTedPostMatchOk returns a tuple with the TedPostMatch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTedPostMatch

`func (o *WebSocketServerMessage) SetTedPostMatch(v string)`

SetTedPostMatch sets TedPostMatch field to given value.


### GetCode

`func (o *WebSocketServerMessage) GetCode() string`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *WebSocketServerMessage) GetCodeOk() (*string, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *WebSocketServerMessage) SetCode(v string)`

SetCode sets Code field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


