# WebSocketClientSetSpeedMessage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Action** | **string** | Action to perform | 
**Speed** | **float32** | Simulation speed multiplier (0.1 &#x3D; slow motion, 10.0 &#x3D; 10x faster) | 

## Methods

### NewWebSocketClientSetSpeedMessage

`func NewWebSocketClientSetSpeedMessage(action string, speed float32, ) *WebSocketClientSetSpeedMessage`

NewWebSocketClientSetSpeedMessage instantiates a new WebSocketClientSetSpeedMessage object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebSocketClientSetSpeedMessageWithDefaults

`func NewWebSocketClientSetSpeedMessageWithDefaults() *WebSocketClientSetSpeedMessage`

NewWebSocketClientSetSpeedMessageWithDefaults instantiates a new WebSocketClientSetSpeedMessage object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAction

`func (o *WebSocketClientSetSpeedMessage) GetAction() string`

GetAction returns the Action field if non-nil, zero value otherwise.

### GetActionOk

`func (o *WebSocketClientSetSpeedMessage) GetActionOk() (*string, bool)`

GetActionOk returns a tuple with the Action field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAction

`func (o *WebSocketClientSetSpeedMessage) SetAction(v string)`

SetAction sets Action field to given value.


### GetSpeed

`func (o *WebSocketClientSetSpeedMessage) GetSpeed() float32`

GetSpeed returns the Speed field if non-nil, zero value otherwise.

### GetSpeedOk

`func (o *WebSocketClientSetSpeedMessage) GetSpeedOk() (*float32, bool)`

GetSpeedOk returns a tuple with the Speed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSpeed

`func (o *WebSocketClientSetSpeedMessage) SetSpeed(v float32)`

SetSpeed sets Speed field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


