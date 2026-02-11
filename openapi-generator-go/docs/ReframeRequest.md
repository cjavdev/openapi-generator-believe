# ReframeRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**NegativeThought** | **string** | The negative thought to reframe | 
**Recurring** | Pointer to **bool** | Is this a recurring thought? | [optional] [default to false]

## Methods

### NewReframeRequest

`func NewReframeRequest(negativeThought string, ) *ReframeRequest`

NewReframeRequest instantiates a new ReframeRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReframeRequestWithDefaults

`func NewReframeRequestWithDefaults() *ReframeRequest`

NewReframeRequestWithDefaults instantiates a new ReframeRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetNegativeThought

`func (o *ReframeRequest) GetNegativeThought() string`

GetNegativeThought returns the NegativeThought field if non-nil, zero value otherwise.

### GetNegativeThoughtOk

`func (o *ReframeRequest) GetNegativeThoughtOk() (*string, bool)`

GetNegativeThoughtOk returns a tuple with the NegativeThought field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNegativeThought

`func (o *ReframeRequest) SetNegativeThought(v string)`

SetNegativeThought sets NegativeThought field to given value.


### GetRecurring

`func (o *ReframeRequest) GetRecurring() bool`

GetRecurring returns the Recurring field if non-nil, zero value otherwise.

### GetRecurringOk

`func (o *ReframeRequest) GetRecurringOk() (*bool, bool)`

GetRecurringOk returns a tuple with the Recurring field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecurring

`func (o *ReframeRequest) SetRecurring(v bool)`

SetRecurring sets Recurring field to given value.

### HasRecurring

`func (o *ReframeRequest) HasRecurring() bool`

HasRecurring returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


