# PepTalkResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Chunks** | [**[]PepTalkChunk**](PepTalkChunk.md) | Individual chunks of the pep talk | 
**Text** | **string** | The full pep talk text | 

## Methods

### NewPepTalkResponse

`func NewPepTalkResponse(chunks []PepTalkChunk, text string, ) *PepTalkResponse`

NewPepTalkResponse instantiates a new PepTalkResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPepTalkResponseWithDefaults

`func NewPepTalkResponseWithDefaults() *PepTalkResponse`

NewPepTalkResponseWithDefaults instantiates a new PepTalkResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetChunks

`func (o *PepTalkResponse) GetChunks() []PepTalkChunk`

GetChunks returns the Chunks field if non-nil, zero value otherwise.

### GetChunksOk

`func (o *PepTalkResponse) GetChunksOk() (*[]PepTalkChunk, bool)`

GetChunksOk returns a tuple with the Chunks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChunks

`func (o *PepTalkResponse) SetChunks(v []PepTalkChunk)`

SetChunks sets Chunks field to given value.


### GetText

`func (o *PepTalkResponse) GetText() string`

GetText returns the Text field if non-nil, zero value otherwise.

### GetTextOk

`func (o *PepTalkResponse) GetTextOk() (*string, bool)`

GetTextOk returns a tuple with the Text field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetText

`func (o *PepTalkResponse) SetText(v string)`

SetText sets Text field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


