# WebSocketMatchStartMessage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AwayTeam** | **string** | Away team name | 
**HomeTeam** | **string** | Home team name | 
**MatchId** | **string** | Unique match identifier | 
**Message** | **string** | Welcome message | 
**Type** | **string** | Message type | 

## Methods

### NewWebSocketMatchStartMessage

`func NewWebSocketMatchStartMessage(awayTeam string, homeTeam string, matchId string, message string, type_ string, ) *WebSocketMatchStartMessage`

NewWebSocketMatchStartMessage instantiates a new WebSocketMatchStartMessage object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebSocketMatchStartMessageWithDefaults

`func NewWebSocketMatchStartMessageWithDefaults() *WebSocketMatchStartMessage`

NewWebSocketMatchStartMessageWithDefaults instantiates a new WebSocketMatchStartMessage object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAwayTeam

`func (o *WebSocketMatchStartMessage) GetAwayTeam() string`

GetAwayTeam returns the AwayTeam field if non-nil, zero value otherwise.

### GetAwayTeamOk

`func (o *WebSocketMatchStartMessage) GetAwayTeamOk() (*string, bool)`

GetAwayTeamOk returns a tuple with the AwayTeam field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAwayTeam

`func (o *WebSocketMatchStartMessage) SetAwayTeam(v string)`

SetAwayTeam sets AwayTeam field to given value.


### GetHomeTeam

`func (o *WebSocketMatchStartMessage) GetHomeTeam() string`

GetHomeTeam returns the HomeTeam field if non-nil, zero value otherwise.

### GetHomeTeamOk

`func (o *WebSocketMatchStartMessage) GetHomeTeamOk() (*string, bool)`

GetHomeTeamOk returns a tuple with the HomeTeam field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHomeTeam

`func (o *WebSocketMatchStartMessage) SetHomeTeam(v string)`

SetHomeTeam sets HomeTeam field to given value.


### GetMatchId

`func (o *WebSocketMatchStartMessage) GetMatchId() string`

GetMatchId returns the MatchId field if non-nil, zero value otherwise.

### GetMatchIdOk

`func (o *WebSocketMatchStartMessage) GetMatchIdOk() (*string, bool)`

GetMatchIdOk returns a tuple with the MatchId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMatchId

`func (o *WebSocketMatchStartMessage) SetMatchId(v string)`

SetMatchId sets MatchId field to given value.


### GetMessage

`func (o *WebSocketMatchStartMessage) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *WebSocketMatchStartMessage) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *WebSocketMatchStartMessage) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetType

`func (o *WebSocketMatchStartMessage) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *WebSocketMatchStartMessage) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *WebSocketMatchStartMessage) SetType(v string)`

SetType sets Type field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


