# PressConferenceRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Hostile** | Pointer to **bool** | Is this a hostile question from Trent Crimm? | [optional] [default to false]
**Question** | **string** | The press question to answer | 
**Topic** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewPressConferenceRequest

`func NewPressConferenceRequest(question string, ) *PressConferenceRequest`

NewPressConferenceRequest instantiates a new PressConferenceRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPressConferenceRequestWithDefaults

`func NewPressConferenceRequestWithDefaults() *PressConferenceRequest`

NewPressConferenceRequestWithDefaults instantiates a new PressConferenceRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetHostile

`func (o *PressConferenceRequest) GetHostile() bool`

GetHostile returns the Hostile field if non-nil, zero value otherwise.

### GetHostileOk

`func (o *PressConferenceRequest) GetHostileOk() (*bool, bool)`

GetHostileOk returns a tuple with the Hostile field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHostile

`func (o *PressConferenceRequest) SetHostile(v bool)`

SetHostile sets Hostile field to given value.

### HasHostile

`func (o *PressConferenceRequest) HasHostile() bool`

HasHostile returns a boolean if a field has been set.

### GetQuestion

`func (o *PressConferenceRequest) GetQuestion() string`

GetQuestion returns the Question field if non-nil, zero value otherwise.

### GetQuestionOk

`func (o *PressConferenceRequest) GetQuestionOk() (*string, bool)`

GetQuestionOk returns a tuple with the Question field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuestion

`func (o *PressConferenceRequest) SetQuestion(v string)`

SetQuestion sets Question field to given value.


### GetTopic

`func (o *PressConferenceRequest) GetTopic() string`

GetTopic returns the Topic field if non-nil, zero value otherwise.

### GetTopicOk

`func (o *PressConferenceRequest) GetTopicOk() (*string, bool)`

GetTopicOk returns a tuple with the Topic field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTopic

`func (o *PressConferenceRequest) SetTopic(v string)`

SetTopic sets Topic field to given value.

### HasTopic

`func (o *PressConferenceRequest) HasTopic() bool`

HasTopic returns a boolean if a field has been set.

### SetTopicNil

`func (o *PressConferenceRequest) SetTopicNil(b bool)`

 SetTopicNil sets the value for Topic to be an explicit nil

### UnsetTopic
`func (o *PressConferenceRequest) UnsetTopic()`

UnsetTopic ensures that no value is present for Topic, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


