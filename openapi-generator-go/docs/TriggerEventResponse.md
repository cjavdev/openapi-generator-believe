# TriggerEventResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Deliveries** | [**[]WebhookDeliveryResult**](WebhookDeliveryResult.md) | Results of webhook deliveries | 
**EventId** | **string** | Unique event identifier | 
**EventType** | **string** | The type of event triggered | 
**SuccessfulDeliveries** | **int32** | Number of successful deliveries | 
**TedSays** | **string** | Ted&#39;s reaction | 
**TotalWebhooks** | **int32** | Total number of webhooks that received this event | 

## Methods

### NewTriggerEventResponse

`func NewTriggerEventResponse(deliveries []WebhookDeliveryResult, eventId string, eventType string, successfulDeliveries int32, tedSays string, totalWebhooks int32, ) *TriggerEventResponse`

NewTriggerEventResponse instantiates a new TriggerEventResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTriggerEventResponseWithDefaults

`func NewTriggerEventResponseWithDefaults() *TriggerEventResponse`

NewTriggerEventResponseWithDefaults instantiates a new TriggerEventResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDeliveries

`func (o *TriggerEventResponse) GetDeliveries() []WebhookDeliveryResult`

GetDeliveries returns the Deliveries field if non-nil, zero value otherwise.

### GetDeliveriesOk

`func (o *TriggerEventResponse) GetDeliveriesOk() (*[]WebhookDeliveryResult, bool)`

GetDeliveriesOk returns a tuple with the Deliveries field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeliveries

`func (o *TriggerEventResponse) SetDeliveries(v []WebhookDeliveryResult)`

SetDeliveries sets Deliveries field to given value.


### GetEventId

`func (o *TriggerEventResponse) GetEventId() string`

GetEventId returns the EventId field if non-nil, zero value otherwise.

### GetEventIdOk

`func (o *TriggerEventResponse) GetEventIdOk() (*string, bool)`

GetEventIdOk returns a tuple with the EventId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventId

`func (o *TriggerEventResponse) SetEventId(v string)`

SetEventId sets EventId field to given value.


### GetEventType

`func (o *TriggerEventResponse) GetEventType() string`

GetEventType returns the EventType field if non-nil, zero value otherwise.

### GetEventTypeOk

`func (o *TriggerEventResponse) GetEventTypeOk() (*string, bool)`

GetEventTypeOk returns a tuple with the EventType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventType

`func (o *TriggerEventResponse) SetEventType(v string)`

SetEventType sets EventType field to given value.


### GetSuccessfulDeliveries

`func (o *TriggerEventResponse) GetSuccessfulDeliveries() int32`

GetSuccessfulDeliveries returns the SuccessfulDeliveries field if non-nil, zero value otherwise.

### GetSuccessfulDeliveriesOk

`func (o *TriggerEventResponse) GetSuccessfulDeliveriesOk() (*int32, bool)`

GetSuccessfulDeliveriesOk returns a tuple with the SuccessfulDeliveries field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccessfulDeliveries

`func (o *TriggerEventResponse) SetSuccessfulDeliveries(v int32)`

SetSuccessfulDeliveries sets SuccessfulDeliveries field to given value.


### GetTedSays

`func (o *TriggerEventResponse) GetTedSays() string`

GetTedSays returns the TedSays field if non-nil, zero value otherwise.

### GetTedSaysOk

`func (o *TriggerEventResponse) GetTedSaysOk() (*string, bool)`

GetTedSaysOk returns a tuple with the TedSays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTedSays

`func (o *TriggerEventResponse) SetTedSays(v string)`

SetTedSays sets TedSays field to given value.


### GetTotalWebhooks

`func (o *TriggerEventResponse) GetTotalWebhooks() int32`

GetTotalWebhooks returns the TotalWebhooks field if non-nil, zero value otherwise.

### GetTotalWebhooksOk

`func (o *TriggerEventResponse) GetTotalWebhooksOk() (*int32, bool)`

GetTotalWebhooksOk returns a tuple with the TotalWebhooks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalWebhooks

`func (o *TriggerEventResponse) SetTotalWebhooks(v int32)`

SetTotalWebhooks sets TotalWebhooks field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


