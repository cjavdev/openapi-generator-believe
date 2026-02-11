# MatchCompletedEvent

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CreatedAt** | **time.Time** | When the event was created | 
**Data** | [**MatchCompletedData**](MatchCompletedData.md) |  | 
**EventId** | **string** | Unique identifier for this event | 
**EventType** | **string** | The type of webhook event | 

## Methods

### NewMatchCompletedEvent

`func NewMatchCompletedEvent(createdAt time.Time, data MatchCompletedData, eventId string, eventType string, ) *MatchCompletedEvent`

NewMatchCompletedEvent instantiates a new MatchCompletedEvent object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMatchCompletedEventWithDefaults

`func NewMatchCompletedEventWithDefaults() *MatchCompletedEvent`

NewMatchCompletedEventWithDefaults instantiates a new MatchCompletedEvent object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCreatedAt

`func (o *MatchCompletedEvent) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *MatchCompletedEvent) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *MatchCompletedEvent) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetData

`func (o *MatchCompletedEvent) GetData() MatchCompletedData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *MatchCompletedEvent) GetDataOk() (*MatchCompletedData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *MatchCompletedEvent) SetData(v MatchCompletedData)`

SetData sets Data field to given value.


### GetEventId

`func (o *MatchCompletedEvent) GetEventId() string`

GetEventId returns the EventId field if non-nil, zero value otherwise.

### GetEventIdOk

`func (o *MatchCompletedEvent) GetEventIdOk() (*string, bool)`

GetEventIdOk returns a tuple with the EventId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventId

`func (o *MatchCompletedEvent) SetEventId(v string)`

SetEventId sets EventId field to given value.


### GetEventType

`func (o *MatchCompletedEvent) GetEventType() string`

GetEventType returns the EventType field if non-nil, zero value otherwise.

### GetEventTypeOk

`func (o *MatchCompletedEvent) GetEventTypeOk() (*string, bool)`

GetEventTypeOk returns a tuple with the EventType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventType

`func (o *MatchCompletedEvent) SetEventType(v string)`

SetEventType sets EventType field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


