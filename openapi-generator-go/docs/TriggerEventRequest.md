# TriggerEventRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**EventType** | **string** | The type of event to trigger | 
**Payload** | Pointer to [**NullableTriggerEventRequestPayload**](TriggerEventRequestPayload.md) |  | [optional] 

## Methods

### NewTriggerEventRequest

`func NewTriggerEventRequest(eventType string, ) *TriggerEventRequest`

NewTriggerEventRequest instantiates a new TriggerEventRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTriggerEventRequestWithDefaults

`func NewTriggerEventRequestWithDefaults() *TriggerEventRequest`

NewTriggerEventRequestWithDefaults instantiates a new TriggerEventRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEventType

`func (o *TriggerEventRequest) GetEventType() string`

GetEventType returns the EventType field if non-nil, zero value otherwise.

### GetEventTypeOk

`func (o *TriggerEventRequest) GetEventTypeOk() (*string, bool)`

GetEventTypeOk returns a tuple with the EventType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventType

`func (o *TriggerEventRequest) SetEventType(v string)`

SetEventType sets EventType field to given value.


### GetPayload

`func (o *TriggerEventRequest) GetPayload() TriggerEventRequestPayload`

GetPayload returns the Payload field if non-nil, zero value otherwise.

### GetPayloadOk

`func (o *TriggerEventRequest) GetPayloadOk() (*TriggerEventRequestPayload, bool)`

GetPayloadOk returns a tuple with the Payload field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPayload

`func (o *TriggerEventRequest) SetPayload(v TriggerEventRequestPayload)`

SetPayload sets Payload field to given value.

### HasPayload

`func (o *TriggerEventRequest) HasPayload() bool`

HasPayload returns a boolean if a field has been set.

### SetPayloadNil

`func (o *TriggerEventRequest) SetPayloadNil(b bool)`

 SetPayloadNil sets the value for Payload to be an explicit nil

### UnsetPayload
`func (o *TriggerEventRequest) UnsetPayload()`

UnsetPayload ensures that no value is present for Payload, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


