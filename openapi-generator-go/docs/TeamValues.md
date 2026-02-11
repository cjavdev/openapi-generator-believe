# TeamValues

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**PrimaryValue** | **string** | The team&#39;s primary guiding value | 
**SecondaryValues** | **[]string** | Supporting values | 
**TeamMotto** | **string** | Team&#39;s motivational motto | 

## Methods

### NewTeamValues

`func NewTeamValues(primaryValue string, secondaryValues []string, teamMotto string, ) *TeamValues`

NewTeamValues instantiates a new TeamValues object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTeamValuesWithDefaults

`func NewTeamValuesWithDefaults() *TeamValues`

NewTeamValuesWithDefaults instantiates a new TeamValues object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPrimaryValue

`func (o *TeamValues) GetPrimaryValue() string`

GetPrimaryValue returns the PrimaryValue field if non-nil, zero value otherwise.

### GetPrimaryValueOk

`func (o *TeamValues) GetPrimaryValueOk() (*string, bool)`

GetPrimaryValueOk returns a tuple with the PrimaryValue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrimaryValue

`func (o *TeamValues) SetPrimaryValue(v string)`

SetPrimaryValue sets PrimaryValue field to given value.


### GetSecondaryValues

`func (o *TeamValues) GetSecondaryValues() []string`

GetSecondaryValues returns the SecondaryValues field if non-nil, zero value otherwise.

### GetSecondaryValuesOk

`func (o *TeamValues) GetSecondaryValuesOk() (*[]string, bool)`

GetSecondaryValuesOk returns a tuple with the SecondaryValues field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecondaryValues

`func (o *TeamValues) SetSecondaryValues(v []string)`

SetSecondaryValues sets SecondaryValues field to given value.


### GetTeamMotto

`func (o *TeamValues) GetTeamMotto() string`

GetTeamMotto returns the TeamMotto field if non-nil, zero value otherwise.

### GetTeamMottoOk

`func (o *TeamValues) GetTeamMottoOk() (*string, bool)`

GetTeamMottoOk returns a tuple with the TeamMotto field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamMotto

`func (o *TeamValues) SetTeamMotto(v string)`

SetTeamMotto sets TeamMotto field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


