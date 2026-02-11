# Biscuit

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Biscuit identifier | 
**Message** | **string** | Message that comes with the biscuit | 
**PairsWellWith** | **string** | What this biscuit pairs well with | 
**TedNote** | **string** | A handwritten note from Ted | 
**Type** | [**BiscuitType**](BiscuitType.md) | Type of biscuit | 
**WarmthLevel** | **int32** | How warm and fresh (1-10) | 

## Methods

### NewBiscuit

`func NewBiscuit(id string, message string, pairsWellWith string, tedNote string, type_ BiscuitType, warmthLevel int32, ) *Biscuit`

NewBiscuit instantiates a new Biscuit object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBiscuitWithDefaults

`func NewBiscuitWithDefaults() *Biscuit`

NewBiscuitWithDefaults instantiates a new Biscuit object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Biscuit) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Biscuit) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Biscuit) SetId(v string)`

SetId sets Id field to given value.


### GetMessage

`func (o *Biscuit) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *Biscuit) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *Biscuit) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetPairsWellWith

`func (o *Biscuit) GetPairsWellWith() string`

GetPairsWellWith returns the PairsWellWith field if non-nil, zero value otherwise.

### GetPairsWellWithOk

`func (o *Biscuit) GetPairsWellWithOk() (*string, bool)`

GetPairsWellWithOk returns a tuple with the PairsWellWith field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPairsWellWith

`func (o *Biscuit) SetPairsWellWith(v string)`

SetPairsWellWith sets PairsWellWith field to given value.


### GetTedNote

`func (o *Biscuit) GetTedNote() string`

GetTedNote returns the TedNote field if non-nil, zero value otherwise.

### GetTedNoteOk

`func (o *Biscuit) GetTedNoteOk() (*string, bool)`

GetTedNoteOk returns a tuple with the TedNote field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTedNote

`func (o *Biscuit) SetTedNote(v string)`

SetTedNote sets TedNote field to given value.


### GetType

`func (o *Biscuit) GetType() BiscuitType`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *Biscuit) GetTypeOk() (*BiscuitType, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *Biscuit) SetType(v BiscuitType)`

SetType sets Type field to given value.


### GetWarmthLevel

`func (o *Biscuit) GetWarmthLevel() int32`

GetWarmthLevel returns the WarmthLevel field if non-nil, zero value otherwise.

### GetWarmthLevelOk

`func (o *Biscuit) GetWarmthLevelOk() (*int32, bool)`

GetWarmthLevelOk returns a tuple with the WarmthLevel field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWarmthLevel

`func (o *Biscuit) SetWarmthLevel(v int32)`

SetWarmthLevel sets WarmthLevel field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


