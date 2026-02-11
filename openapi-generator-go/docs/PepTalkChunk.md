# PepTalkChunk

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ChunkId** | **int32** | Chunk sequence number | 
**EmotionalBeat** | Pointer to **string** | The emotional purpose of this chunk (e.g., greeting, acknowledgment, wisdom, affirmation, encouragement) | [optional] 
**IsFinal** | **bool** | Is this the final chunk | [default to false]
**Text** | **string** | The text of this chunk | 

## Methods

### NewPepTalkChunk

`func NewPepTalkChunk(chunkId int32, isFinal bool, text string, ) *PepTalkChunk`

NewPepTalkChunk instantiates a new PepTalkChunk object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPepTalkChunkWithDefaults

`func NewPepTalkChunkWithDefaults() *PepTalkChunk`

NewPepTalkChunkWithDefaults instantiates a new PepTalkChunk object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetChunkId

`func (o *PepTalkChunk) GetChunkId() int32`

GetChunkId returns the ChunkId field if non-nil, zero value otherwise.

### GetChunkIdOk

`func (o *PepTalkChunk) GetChunkIdOk() (*int32, bool)`

GetChunkIdOk returns a tuple with the ChunkId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChunkId

`func (o *PepTalkChunk) SetChunkId(v int32)`

SetChunkId sets ChunkId field to given value.


### GetEmotionalBeat

`func (o *PepTalkChunk) GetEmotionalBeat() string`

GetEmotionalBeat returns the EmotionalBeat field if non-nil, zero value otherwise.

### GetEmotionalBeatOk

`func (o *PepTalkChunk) GetEmotionalBeatOk() (*string, bool)`

GetEmotionalBeatOk returns a tuple with the EmotionalBeat field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmotionalBeat

`func (o *PepTalkChunk) SetEmotionalBeat(v string)`

SetEmotionalBeat sets EmotionalBeat field to given value.

### HasEmotionalBeat

`func (o *PepTalkChunk) HasEmotionalBeat() bool`

HasEmotionalBeat returns a boolean if a field has been set.

### GetIsFinal

`func (o *PepTalkChunk) GetIsFinal() bool`

GetIsFinal returns the IsFinal field if non-nil, zero value otherwise.

### GetIsFinalOk

`func (o *PepTalkChunk) GetIsFinalOk() (*bool, bool)`

GetIsFinalOk returns a tuple with the IsFinal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsFinal

`func (o *PepTalkChunk) SetIsFinal(v bool)`

SetIsFinal sets IsFinal field to given value.


### GetText

`func (o *PepTalkChunk) GetText() string`

GetText returns the Text field if non-nil, zero value otherwise.

### GetTextOk

`func (o *PepTalkChunk) GetTextOk() (*string, bool)`

GetTextOk returns a tuple with the Text field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetText

`func (o *PepTalkChunk) SetText(v string)`

SetText sets Text field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


