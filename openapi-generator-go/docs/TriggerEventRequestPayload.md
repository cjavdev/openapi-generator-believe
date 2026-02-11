# TriggerEventRequestPayload

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | [**TeamMemberTransferredData**](TeamMemberTransferredData.md) | Event data | 
**EventType** | Pointer to **string** | The type of webhook event | [optional] [default to "team_member.transferred"]

## Methods

### NewTriggerEventRequestPayload

`func NewTriggerEventRequestPayload(data TeamMemberTransferredData, ) *TriggerEventRequestPayload`

NewTriggerEventRequestPayload instantiates a new TriggerEventRequestPayload object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTriggerEventRequestPayloadWithDefaults

`func NewTriggerEventRequestPayloadWithDefaults() *TriggerEventRequestPayload`

NewTriggerEventRequestPayloadWithDefaults instantiates a new TriggerEventRequestPayload object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *TriggerEventRequestPayload) GetData() TeamMemberTransferredData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *TriggerEventRequestPayload) GetDataOk() (*TeamMemberTransferredData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *TriggerEventRequestPayload) SetData(v TeamMemberTransferredData)`

SetData sets Data field to given value.


### GetEventType

`func (o *TriggerEventRequestPayload) GetEventType() string`

GetEventType returns the EventType field if non-nil, zero value otherwise.

### GetEventTypeOk

`func (o *TriggerEventRequestPayload) GetEventTypeOk() (*string, bool)`

GetEventTypeOk returns a tuple with the EventType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventType

`func (o *TriggerEventRequestPayload) SetEventType(v string)`

SetEventType sets EventType field to given value.

### HasEventType

`func (o *TriggerEventRequestPayload) HasEventType() bool`

HasEventType returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


