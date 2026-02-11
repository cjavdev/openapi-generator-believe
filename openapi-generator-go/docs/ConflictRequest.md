# ConflictRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AttemptsMade** | Pointer to **[]string** |  | [optional] 
**ConflictType** | [**ConflictType**](ConflictType.md) | Type of conflict | 
**Description** | **string** | Describe the conflict | 
**PartiesInvolved** | **[]string** | Who is involved in the conflict | 

## Methods

### NewConflictRequest

`func NewConflictRequest(conflictType ConflictType, description string, partiesInvolved []string, ) *ConflictRequest`

NewConflictRequest instantiates a new ConflictRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewConflictRequestWithDefaults

`func NewConflictRequestWithDefaults() *ConflictRequest`

NewConflictRequestWithDefaults instantiates a new ConflictRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttemptsMade

`func (o *ConflictRequest) GetAttemptsMade() []string`

GetAttemptsMade returns the AttemptsMade field if non-nil, zero value otherwise.

### GetAttemptsMadeOk

`func (o *ConflictRequest) GetAttemptsMadeOk() (*[]string, bool)`

GetAttemptsMadeOk returns a tuple with the AttemptsMade field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttemptsMade

`func (o *ConflictRequest) SetAttemptsMade(v []string)`

SetAttemptsMade sets AttemptsMade field to given value.

### HasAttemptsMade

`func (o *ConflictRequest) HasAttemptsMade() bool`

HasAttemptsMade returns a boolean if a field has been set.

### SetAttemptsMadeNil

`func (o *ConflictRequest) SetAttemptsMadeNil(b bool)`

 SetAttemptsMadeNil sets the value for AttemptsMade to be an explicit nil

### UnsetAttemptsMade
`func (o *ConflictRequest) UnsetAttemptsMade()`

UnsetAttemptsMade ensures that no value is present for AttemptsMade, not even an explicit nil
### GetConflictType

`func (o *ConflictRequest) GetConflictType() ConflictType`

GetConflictType returns the ConflictType field if non-nil, zero value otherwise.

### GetConflictTypeOk

`func (o *ConflictRequest) GetConflictTypeOk() (*ConflictType, bool)`

GetConflictTypeOk returns a tuple with the ConflictType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConflictType

`func (o *ConflictRequest) SetConflictType(v ConflictType)`

SetConflictType sets ConflictType field to given value.


### GetDescription

`func (o *ConflictRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ConflictRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ConflictRequest) SetDescription(v string)`

SetDescription sets Description field to given value.


### GetPartiesInvolved

`func (o *ConflictRequest) GetPartiesInvolved() []string`

GetPartiesInvolved returns the PartiesInvolved field if non-nil, zero value otherwise.

### GetPartiesInvolvedOk

`func (o *ConflictRequest) GetPartiesInvolvedOk() (*[]string, bool)`

GetPartiesInvolvedOk returns a tuple with the PartiesInvolved field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPartiesInvolved

`func (o *ConflictRequest) SetPartiesInvolved(v []string)`

SetPartiesInvolved sets PartiesInvolved field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


