# TeamMemberTransferredEvent

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CreatedAt** | **time.Time** | When the event was created | 
**Data** | [**TeamMemberTransferredData**](TeamMemberTransferredData.md) |  | 
**EventId** | **string** | Unique identifier for this event | 
**EventType** | **string** | The type of webhook event | 

## Methods

### NewTeamMemberTransferredEvent

`func NewTeamMemberTransferredEvent(createdAt time.Time, data TeamMemberTransferredData, eventId string, eventType string, ) *TeamMemberTransferredEvent`

NewTeamMemberTransferredEvent instantiates a new TeamMemberTransferredEvent object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTeamMemberTransferredEventWithDefaults

`func NewTeamMemberTransferredEventWithDefaults() *TeamMemberTransferredEvent`

NewTeamMemberTransferredEventWithDefaults instantiates a new TeamMemberTransferredEvent object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCreatedAt

`func (o *TeamMemberTransferredEvent) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *TeamMemberTransferredEvent) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *TeamMemberTransferredEvent) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetData

`func (o *TeamMemberTransferredEvent) GetData() TeamMemberTransferredData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *TeamMemberTransferredEvent) GetDataOk() (*TeamMemberTransferredData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *TeamMemberTransferredEvent) SetData(v TeamMemberTransferredData)`

SetData sets Data field to given value.


### GetEventId

`func (o *TeamMemberTransferredEvent) GetEventId() string`

GetEventId returns the EventId field if non-nil, zero value otherwise.

### GetEventIdOk

`func (o *TeamMemberTransferredEvent) GetEventIdOk() (*string, bool)`

GetEventIdOk returns a tuple with the EventId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventId

`func (o *TeamMemberTransferredEvent) SetEventId(v string)`

SetEventId sets EventId field to given value.


### GetEventType

`func (o *TeamMemberTransferredEvent) GetEventType() string`

GetEventType returns the EventType field if non-nil, zero value otherwise.

### GetEventTypeOk

`func (o *TeamMemberTransferredEvent) GetEventTypeOk() (*string, bool)`

GetEventTypeOk returns a tuple with the EventType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventType

`func (o *TeamMemberTransferredEvent) SetEventType(v string)`

SetEventType sets EventType field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


