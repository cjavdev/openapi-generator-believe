# TestStreamChunk

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Message** | **string** | The message content for this chunk | 
**Sequence** | **int32** | The sequence number of this chunk (1-5) | 

## Methods

### NewTestStreamChunk

`func NewTestStreamChunk(message string, sequence int32, ) *TestStreamChunk`

NewTestStreamChunk instantiates a new TestStreamChunk object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTestStreamChunkWithDefaults

`func NewTestStreamChunkWithDefaults() *TestStreamChunk`

NewTestStreamChunkWithDefaults instantiates a new TestStreamChunk object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMessage

`func (o *TestStreamChunk) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *TestStreamChunk) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *TestStreamChunk) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetSequence

`func (o *TestStreamChunk) GetSequence() int32`

GetSequence returns the Sequence field if non-nil, zero value otherwise.

### GetSequenceOk

`func (o *TestStreamChunk) GetSequenceOk() (*int32, bool)`

GetSequenceOk returns a tuple with the Sequence field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSequence

`func (o *TestStreamChunk) SetSequence(v int32)`

SetSequence sets Sequence field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


