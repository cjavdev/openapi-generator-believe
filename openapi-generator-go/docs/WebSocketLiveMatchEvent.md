# WebSocketLiveMatchEvent

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AddedTime** | Pointer to **int32** | Added/injury time minutes | [optional] 
**Commentary** | **string** | Match commentary for this event | 
**CrowdReaction** | Pointer to **string** | Crowd reaction to the event | [optional] 
**Description** | **string** | Human-readable event description | 
**EventId** | **int32** | Unique event sequence number | 
**EventType** | **string** | Type of match event | 
**Minute** | **int32** | Match minute | 
**Player** | Pointer to [**WebSocketPlayerInfo**](WebSocketPlayerInfo.md) |  | [optional] 
**Score** | [**WebSocketMatchScore**](WebSocketMatchScore.md) |  | 
**SecondaryPlayer** | Pointer to [**WebSocketPlayerInfo**](WebSocketPlayerInfo.md) | Second player involved (e.g., assist, replaced player) | [optional] 
**Stats** | [**WebSocketMatchStats**](WebSocketMatchStats.md) |  | 
**Team** | Pointer to **string** | Which team the event relates to | [optional] 
**TedReaction** | Pointer to **string** | Ted Lasso&#39;s sideline reaction | [optional] 

## Methods

### NewWebSocketLiveMatchEvent

`func NewWebSocketLiveMatchEvent(commentary string, description string, eventId int32, eventType string, minute int32, score WebSocketMatchScore, stats WebSocketMatchStats, ) *WebSocketLiveMatchEvent`

NewWebSocketLiveMatchEvent instantiates a new WebSocketLiveMatchEvent object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebSocketLiveMatchEventWithDefaults

`func NewWebSocketLiveMatchEventWithDefaults() *WebSocketLiveMatchEvent`

NewWebSocketLiveMatchEventWithDefaults instantiates a new WebSocketLiveMatchEvent object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAddedTime

`func (o *WebSocketLiveMatchEvent) GetAddedTime() int32`

GetAddedTime returns the AddedTime field if non-nil, zero value otherwise.

### GetAddedTimeOk

`func (o *WebSocketLiveMatchEvent) GetAddedTimeOk() (*int32, bool)`

GetAddedTimeOk returns a tuple with the AddedTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddedTime

`func (o *WebSocketLiveMatchEvent) SetAddedTime(v int32)`

SetAddedTime sets AddedTime field to given value.

### HasAddedTime

`func (o *WebSocketLiveMatchEvent) HasAddedTime() bool`

HasAddedTime returns a boolean if a field has been set.

### GetCommentary

`func (o *WebSocketLiveMatchEvent) GetCommentary() string`

GetCommentary returns the Commentary field if non-nil, zero value otherwise.

### GetCommentaryOk

`func (o *WebSocketLiveMatchEvent) GetCommentaryOk() (*string, bool)`

GetCommentaryOk returns a tuple with the Commentary field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCommentary

`func (o *WebSocketLiveMatchEvent) SetCommentary(v string)`

SetCommentary sets Commentary field to given value.


### GetCrowdReaction

`func (o *WebSocketLiveMatchEvent) GetCrowdReaction() string`

GetCrowdReaction returns the CrowdReaction field if non-nil, zero value otherwise.

### GetCrowdReactionOk

`func (o *WebSocketLiveMatchEvent) GetCrowdReactionOk() (*string, bool)`

GetCrowdReactionOk returns a tuple with the CrowdReaction field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCrowdReaction

`func (o *WebSocketLiveMatchEvent) SetCrowdReaction(v string)`

SetCrowdReaction sets CrowdReaction field to given value.

### HasCrowdReaction

`func (o *WebSocketLiveMatchEvent) HasCrowdReaction() bool`

HasCrowdReaction returns a boolean if a field has been set.

### GetDescription

`func (o *WebSocketLiveMatchEvent) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *WebSocketLiveMatchEvent) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *WebSocketLiveMatchEvent) SetDescription(v string)`

SetDescription sets Description field to given value.


### GetEventId

`func (o *WebSocketLiveMatchEvent) GetEventId() int32`

GetEventId returns the EventId field if non-nil, zero value otherwise.

### GetEventIdOk

`func (o *WebSocketLiveMatchEvent) GetEventIdOk() (*int32, bool)`

GetEventIdOk returns a tuple with the EventId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventId

`func (o *WebSocketLiveMatchEvent) SetEventId(v int32)`

SetEventId sets EventId field to given value.


### GetEventType

`func (o *WebSocketLiveMatchEvent) GetEventType() string`

GetEventType returns the EventType field if non-nil, zero value otherwise.

### GetEventTypeOk

`func (o *WebSocketLiveMatchEvent) GetEventTypeOk() (*string, bool)`

GetEventTypeOk returns a tuple with the EventType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventType

`func (o *WebSocketLiveMatchEvent) SetEventType(v string)`

SetEventType sets EventType field to given value.


### GetMinute

`func (o *WebSocketLiveMatchEvent) GetMinute() int32`

GetMinute returns the Minute field if non-nil, zero value otherwise.

### GetMinuteOk

`func (o *WebSocketLiveMatchEvent) GetMinuteOk() (*int32, bool)`

GetMinuteOk returns a tuple with the Minute field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinute

`func (o *WebSocketLiveMatchEvent) SetMinute(v int32)`

SetMinute sets Minute field to given value.


### GetPlayer

`func (o *WebSocketLiveMatchEvent) GetPlayer() WebSocketPlayerInfo`

GetPlayer returns the Player field if non-nil, zero value otherwise.

### GetPlayerOk

`func (o *WebSocketLiveMatchEvent) GetPlayerOk() (*WebSocketPlayerInfo, bool)`

GetPlayerOk returns a tuple with the Player field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlayer

`func (o *WebSocketLiveMatchEvent) SetPlayer(v WebSocketPlayerInfo)`

SetPlayer sets Player field to given value.

### HasPlayer

`func (o *WebSocketLiveMatchEvent) HasPlayer() bool`

HasPlayer returns a boolean if a field has been set.

### GetScore

`func (o *WebSocketLiveMatchEvent) GetScore() WebSocketMatchScore`

GetScore returns the Score field if non-nil, zero value otherwise.

### GetScoreOk

`func (o *WebSocketLiveMatchEvent) GetScoreOk() (*WebSocketMatchScore, bool)`

GetScoreOk returns a tuple with the Score field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScore

`func (o *WebSocketLiveMatchEvent) SetScore(v WebSocketMatchScore)`

SetScore sets Score field to given value.


### GetSecondaryPlayer

`func (o *WebSocketLiveMatchEvent) GetSecondaryPlayer() WebSocketPlayerInfo`

GetSecondaryPlayer returns the SecondaryPlayer field if non-nil, zero value otherwise.

### GetSecondaryPlayerOk

`func (o *WebSocketLiveMatchEvent) GetSecondaryPlayerOk() (*WebSocketPlayerInfo, bool)`

GetSecondaryPlayerOk returns a tuple with the SecondaryPlayer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecondaryPlayer

`func (o *WebSocketLiveMatchEvent) SetSecondaryPlayer(v WebSocketPlayerInfo)`

SetSecondaryPlayer sets SecondaryPlayer field to given value.

### HasSecondaryPlayer

`func (o *WebSocketLiveMatchEvent) HasSecondaryPlayer() bool`

HasSecondaryPlayer returns a boolean if a field has been set.

### GetStats

`func (o *WebSocketLiveMatchEvent) GetStats() WebSocketMatchStats`

GetStats returns the Stats field if non-nil, zero value otherwise.

### GetStatsOk

`func (o *WebSocketLiveMatchEvent) GetStatsOk() (*WebSocketMatchStats, bool)`

GetStatsOk returns a tuple with the Stats field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStats

`func (o *WebSocketLiveMatchEvent) SetStats(v WebSocketMatchStats)`

SetStats sets Stats field to given value.


### GetTeam

`func (o *WebSocketLiveMatchEvent) GetTeam() string`

GetTeam returns the Team field if non-nil, zero value otherwise.

### GetTeamOk

`func (o *WebSocketLiveMatchEvent) GetTeamOk() (*string, bool)`

GetTeamOk returns a tuple with the Team field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeam

`func (o *WebSocketLiveMatchEvent) SetTeam(v string)`

SetTeam sets Team field to given value.

### HasTeam

`func (o *WebSocketLiveMatchEvent) HasTeam() bool`

HasTeam returns a boolean if a field has been set.

### GetTedReaction

`func (o *WebSocketLiveMatchEvent) GetTedReaction() string`

GetTedReaction returns the TedReaction field if non-nil, zero value otherwise.

### GetTedReactionOk

`func (o *WebSocketLiveMatchEvent) GetTedReactionOk() (*string, bool)`

GetTedReactionOk returns a tuple with the TedReaction field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTedReaction

`func (o *WebSocketLiveMatchEvent) SetTedReaction(v string)`

SetTedReaction sets TedReaction field to given value.

### HasTedReaction

`func (o *WebSocketLiveMatchEvent) HasTedReaction() bool`

HasTedReaction returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


