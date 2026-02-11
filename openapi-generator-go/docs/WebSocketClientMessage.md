# WebSocketClientMessage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Action** | **string** | Action to perform | 
**Speed** | **float32** | Simulation speed multiplier (0.1 &#x3D; slow motion, 10.0 &#x3D; 10x faster) | 

## Methods

### NewWebSocketClientMessage

`func NewWebSocketClientMessage(action string, speed float32, ) *WebSocketClientMessage`

NewWebSocketClientMessage instantiates a new WebSocketClientMessage object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebSocketClientMessageWithDefaults

`func NewWebSocketClientMessageWithDefaults() *WebSocketClientMessage`

NewWebSocketClientMessageWithDefaults instantiates a new WebSocketClientMessage object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAction

`func (o *WebSocketClientMessage) GetAction() string`

GetAction returns the Action field if non-nil, zero value otherwise.

### GetActionOk

`func (o *WebSocketClientMessage) GetActionOk() (*string, bool)`

GetActionOk returns a tuple with the Action field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAction

`func (o *WebSocketClientMessage) SetAction(v string)`

SetAction sets Action field to given value.


### GetSpeed

`func (o *WebSocketClientMessage) GetSpeed() float32`

GetSpeed returns the Speed field if non-nil, zero value otherwise.

### GetSpeedOk

`func (o *WebSocketClientMessage) GetSpeedOk() (*float32, bool)`

GetSpeedOk returns a tuple with the Speed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSpeed

`func (o *WebSocketClientMessage) SetSpeed(v float32)`

SetSpeed sets Speed field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


