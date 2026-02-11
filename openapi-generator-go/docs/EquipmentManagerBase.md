# EquipmentManagerBase

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CharacterId** | **string** | ID of the character (references /characters/{id}) | 
**IsHeadKitman** | Pointer to **bool** | Whether this is the head equipment manager | [optional] [default to false]
**MemberType** | Pointer to **string** | Discriminator field indicating this is an equipment manager | [optional] [default to "equipment_manager"]
**Responsibilities** | Pointer to **[]string** | List of responsibilities | [optional] 
**TeamId** | **string** | ID of the team they belong to | 
**YearsWithTeam** | **int32** | Number of years with the current team | 

## Methods

### NewEquipmentManagerBase

`func NewEquipmentManagerBase(characterId string, teamId string, yearsWithTeam int32, ) *EquipmentManagerBase`

NewEquipmentManagerBase instantiates a new EquipmentManagerBase object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEquipmentManagerBaseWithDefaults

`func NewEquipmentManagerBaseWithDefaults() *EquipmentManagerBase`

NewEquipmentManagerBaseWithDefaults instantiates a new EquipmentManagerBase object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCharacterId

`func (o *EquipmentManagerBase) GetCharacterId() string`

GetCharacterId returns the CharacterId field if non-nil, zero value otherwise.

### GetCharacterIdOk

`func (o *EquipmentManagerBase) GetCharacterIdOk() (*string, bool)`

GetCharacterIdOk returns a tuple with the CharacterId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCharacterId

`func (o *EquipmentManagerBase) SetCharacterId(v string)`

SetCharacterId sets CharacterId field to given value.


### GetIsHeadKitman

`func (o *EquipmentManagerBase) GetIsHeadKitman() bool`

GetIsHeadKitman returns the IsHeadKitman field if non-nil, zero value otherwise.

### GetIsHeadKitmanOk

`func (o *EquipmentManagerBase) GetIsHeadKitmanOk() (*bool, bool)`

GetIsHeadKitmanOk returns a tuple with the IsHeadKitman field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsHeadKitman

`func (o *EquipmentManagerBase) SetIsHeadKitman(v bool)`

SetIsHeadKitman sets IsHeadKitman field to given value.

### HasIsHeadKitman

`func (o *EquipmentManagerBase) HasIsHeadKitman() bool`

HasIsHeadKitman returns a boolean if a field has been set.

### GetMemberType

`func (o *EquipmentManagerBase) GetMemberType() string`

GetMemberType returns the MemberType field if non-nil, zero value otherwise.

### GetMemberTypeOk

`func (o *EquipmentManagerBase) GetMemberTypeOk() (*string, bool)`

GetMemberTypeOk returns a tuple with the MemberType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMemberType

`func (o *EquipmentManagerBase) SetMemberType(v string)`

SetMemberType sets MemberType field to given value.

### HasMemberType

`func (o *EquipmentManagerBase) HasMemberType() bool`

HasMemberType returns a boolean if a field has been set.

### GetResponsibilities

`func (o *EquipmentManagerBase) GetResponsibilities() []string`

GetResponsibilities returns the Responsibilities field if non-nil, zero value otherwise.

### GetResponsibilitiesOk

`func (o *EquipmentManagerBase) GetResponsibilitiesOk() (*[]string, bool)`

GetResponsibilitiesOk returns a tuple with the Responsibilities field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponsibilities

`func (o *EquipmentManagerBase) SetResponsibilities(v []string)`

SetResponsibilities sets Responsibilities field to given value.

### HasResponsibilities

`func (o *EquipmentManagerBase) HasResponsibilities() bool`

HasResponsibilities returns a boolean if a field has been set.

### GetTeamId

`func (o *EquipmentManagerBase) GetTeamId() string`

GetTeamId returns the TeamId field if non-nil, zero value otherwise.

### GetTeamIdOk

`func (o *EquipmentManagerBase) GetTeamIdOk() (*string, bool)`

GetTeamIdOk returns a tuple with the TeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamId

`func (o *EquipmentManagerBase) SetTeamId(v string)`

SetTeamId sets TeamId field to given value.


### GetYearsWithTeam

`func (o *EquipmentManagerBase) GetYearsWithTeam() int32`

GetYearsWithTeam returns the YearsWithTeam field if non-nil, zero value otherwise.

### GetYearsWithTeamOk

`func (o *EquipmentManagerBase) GetYearsWithTeamOk() (*int32, bool)`

GetYearsWithTeamOk returns a tuple with the YearsWithTeam field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetYearsWithTeam

`func (o *EquipmentManagerBase) SetYearsWithTeam(v int32)`

SetYearsWithTeam sets YearsWithTeam field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


