# WebSocketMatchEndMessage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**FinalScore** | [**WebSocketMatchScore**](WebSocketMatchScore.md) |  | 
**FinalStats** | [**WebSocketMatchStats**](WebSocketMatchStats.md) |  | 
**ManOfTheMatch** | **string** | Man of the match | 
**MatchId** | **string** | Match identifier | 
**TedPostMatch** | **string** | Ted&#39;s post-match thoughts | 
**Type** | **string** | Message type | 

## Methods

### NewWebSocketMatchEndMessage

`func NewWebSocketMatchEndMessage(finalScore WebSocketMatchScore, finalStats WebSocketMatchStats, manOfTheMatch string, matchId string, tedPostMatch string, type_ string, ) *WebSocketMatchEndMessage`

NewWebSocketMatchEndMessage instantiates a new WebSocketMatchEndMessage object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebSocketMatchEndMessageWithDefaults

`func NewWebSocketMatchEndMessageWithDefaults() *WebSocketMatchEndMessage`

NewWebSocketMatchEndMessageWithDefaults instantiates a new WebSocketMatchEndMessage object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFinalScore

`func (o *WebSocketMatchEndMessage) GetFinalScore() WebSocketMatchScore`

GetFinalScore returns the FinalScore field if non-nil, zero value otherwise.

### GetFinalScoreOk

`func (o *WebSocketMatchEndMessage) GetFinalScoreOk() (*WebSocketMatchScore, bool)`

GetFinalScoreOk returns a tuple with the FinalScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFinalScore

`func (o *WebSocketMatchEndMessage) SetFinalScore(v WebSocketMatchScore)`

SetFinalScore sets FinalScore field to given value.


### GetFinalStats

`func (o *WebSocketMatchEndMessage) GetFinalStats() WebSocketMatchStats`

GetFinalStats returns the FinalStats field if non-nil, zero value otherwise.

### GetFinalStatsOk

`func (o *WebSocketMatchEndMessage) GetFinalStatsOk() (*WebSocketMatchStats, bool)`

GetFinalStatsOk returns a tuple with the FinalStats field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFinalStats

`func (o *WebSocketMatchEndMessage) SetFinalStats(v WebSocketMatchStats)`

SetFinalStats sets FinalStats field to given value.


### GetManOfTheMatch

`func (o *WebSocketMatchEndMessage) GetManOfTheMatch() string`

GetManOfTheMatch returns the ManOfTheMatch field if non-nil, zero value otherwise.

### GetManOfTheMatchOk

`func (o *WebSocketMatchEndMessage) GetManOfTheMatchOk() (*string, bool)`

GetManOfTheMatchOk returns a tuple with the ManOfTheMatch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetManOfTheMatch

`func (o *WebSocketMatchEndMessage) SetManOfTheMatch(v string)`

SetManOfTheMatch sets ManOfTheMatch field to given value.


### GetMatchId

`func (o *WebSocketMatchEndMessage) GetMatchId() string`

GetMatchId returns the MatchId field if non-nil, zero value otherwise.

### GetMatchIdOk

`func (o *WebSocketMatchEndMessage) GetMatchIdOk() (*string, bool)`

GetMatchIdOk returns a tuple with the MatchId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMatchId

`func (o *WebSocketMatchEndMessage) SetMatchId(v string)`

SetMatchId sets MatchId field to given value.


### GetTedPostMatch

`func (o *WebSocketMatchEndMessage) GetTedPostMatch() string`

GetTedPostMatch returns the TedPostMatch field if non-nil, zero value otherwise.

### GetTedPostMatchOk

`func (o *WebSocketMatchEndMessage) GetTedPostMatchOk() (*string, bool)`

GetTedPostMatchOk returns a tuple with the TedPostMatch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTedPostMatch

`func (o *WebSocketMatchEndMessage) SetTedPostMatch(v string)`

SetTedPostMatch sets TedPostMatch field to given value.


### GetType

`func (o *WebSocketMatchEndMessage) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *WebSocketMatchEndMessage) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *WebSocketMatchEndMessage) SetType(v string)`

SetType sets Type field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


