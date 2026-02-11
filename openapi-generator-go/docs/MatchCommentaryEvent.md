# MatchCommentaryEvent

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Commentary** | **string** | Commentator&#39;s call | 
**CrowdReaction** | Pointer to **string** | How the crowd reacted | [optional] 
**Description** | **string** | What happened | 
**EventId** | **int32** | Event sequence number | 
**EventType** | **string** | Type of event | 
**IsFinal** | **bool** | Is this the final event | [default to false]
**Minute** | **int32** | Match minute | 
**TedSidelineReaction** | Pointer to **string** | Ted&#39;s reaction on the sideline | [optional] 

## Methods

### NewMatchCommentaryEvent

`func NewMatchCommentaryEvent(commentary string, description string, eventId int32, eventType string, isFinal bool, minute int32, ) *MatchCommentaryEvent`

NewMatchCommentaryEvent instantiates a new MatchCommentaryEvent object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMatchCommentaryEventWithDefaults

`func NewMatchCommentaryEventWithDefaults() *MatchCommentaryEvent`

NewMatchCommentaryEventWithDefaults instantiates a new MatchCommentaryEvent object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCommentary

`func (o *MatchCommentaryEvent) GetCommentary() string`

GetCommentary returns the Commentary field if non-nil, zero value otherwise.

### GetCommentaryOk

`func (o *MatchCommentaryEvent) GetCommentaryOk() (*string, bool)`

GetCommentaryOk returns a tuple with the Commentary field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCommentary

`func (o *MatchCommentaryEvent) SetCommentary(v string)`

SetCommentary sets Commentary field to given value.


### GetCrowdReaction

`func (o *MatchCommentaryEvent) GetCrowdReaction() string`

GetCrowdReaction returns the CrowdReaction field if non-nil, zero value otherwise.

### GetCrowdReactionOk

`func (o *MatchCommentaryEvent) GetCrowdReactionOk() (*string, bool)`

GetCrowdReactionOk returns a tuple with the CrowdReaction field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCrowdReaction

`func (o *MatchCommentaryEvent) SetCrowdReaction(v string)`

SetCrowdReaction sets CrowdReaction field to given value.

### HasCrowdReaction

`func (o *MatchCommentaryEvent) HasCrowdReaction() bool`

HasCrowdReaction returns a boolean if a field has been set.

### GetDescription

`func (o *MatchCommentaryEvent) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *MatchCommentaryEvent) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *MatchCommentaryEvent) SetDescription(v string)`

SetDescription sets Description field to given value.


### GetEventId

`func (o *MatchCommentaryEvent) GetEventId() int32`

GetEventId returns the EventId field if non-nil, zero value otherwise.

### GetEventIdOk

`func (o *MatchCommentaryEvent) GetEventIdOk() (*int32, bool)`

GetEventIdOk returns a tuple with the EventId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventId

`func (o *MatchCommentaryEvent) SetEventId(v int32)`

SetEventId sets EventId field to given value.


### GetEventType

`func (o *MatchCommentaryEvent) GetEventType() string`

GetEventType returns the EventType field if non-nil, zero value otherwise.

### GetEventTypeOk

`func (o *MatchCommentaryEvent) GetEventTypeOk() (*string, bool)`

GetEventTypeOk returns a tuple with the EventType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventType

`func (o *MatchCommentaryEvent) SetEventType(v string)`

SetEventType sets EventType field to given value.


### GetIsFinal

`func (o *MatchCommentaryEvent) GetIsFinal() bool`

GetIsFinal returns the IsFinal field if non-nil, zero value otherwise.

### GetIsFinalOk

`func (o *MatchCommentaryEvent) GetIsFinalOk() (*bool, bool)`

GetIsFinalOk returns a tuple with the IsFinal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsFinal

`func (o *MatchCommentaryEvent) SetIsFinal(v bool)`

SetIsFinal sets IsFinal field to given value.


### GetMinute

`func (o *MatchCommentaryEvent) GetMinute() int32`

GetMinute returns the Minute field if non-nil, zero value otherwise.

### GetMinuteOk

`func (o *MatchCommentaryEvent) GetMinuteOk() (*int32, bool)`

GetMinuteOk returns a tuple with the Minute field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinute

`func (o *MatchCommentaryEvent) SetMinute(v int32)`

SetMinute sets Minute field to given value.


### GetTedSidelineReaction

`func (o *MatchCommentaryEvent) GetTedSidelineReaction() string`

GetTedSidelineReaction returns the TedSidelineReaction field if non-nil, zero value otherwise.

### GetTedSidelineReactionOk

`func (o *MatchCommentaryEvent) GetTedSidelineReactionOk() (*string, bool)`

GetTedSidelineReactionOk returns a tuple with the TedSidelineReaction field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTedSidelineReaction

`func (o *MatchCommentaryEvent) SetTedSidelineReaction(v string)`

SetTedSidelineReaction sets TedSidelineReaction field to given value.

### HasTedSidelineReaction

`func (o *MatchCommentaryEvent) HasTedSidelineReaction() bool`

HasTedSidelineReaction returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


