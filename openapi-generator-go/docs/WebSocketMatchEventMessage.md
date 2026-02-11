# WebSocketMatchEventMessage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Event** | [**WebSocketLiveMatchEvent**](WebSocketLiveMatchEvent.md) |  | 
**Type** | **string** | Message type | 

## Methods

### NewWebSocketMatchEventMessage

`func NewWebSocketMatchEventMessage(event WebSocketLiveMatchEvent, type_ string, ) *WebSocketMatchEventMessage`

NewWebSocketMatchEventMessage instantiates a new WebSocketMatchEventMessage object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebSocketMatchEventMessageWithDefaults

`func NewWebSocketMatchEventMessageWithDefaults() *WebSocketMatchEventMessage`

NewWebSocketMatchEventMessageWithDefaults instantiates a new WebSocketMatchEventMessage object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEvent

`func (o *WebSocketMatchEventMessage) GetEvent() WebSocketLiveMatchEvent`

GetEvent returns the Event field if non-nil, zero value otherwise.

### GetEventOk

`func (o *WebSocketMatchEventMessage) GetEventOk() (*WebSocketLiveMatchEvent, bool)`

GetEventOk returns a tuple with the Event field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEvent

`func (o *WebSocketMatchEventMessage) SetEvent(v WebSocketLiveMatchEvent)`

SetEvent sets Event field to given value.


### GetType

`func (o *WebSocketMatchEventMessage) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *WebSocketMatchEventMessage) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *WebSocketMatchEventMessage) SetType(v string)`

SetType sets Type field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


