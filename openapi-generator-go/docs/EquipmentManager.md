# EquipmentManager

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CharacterId** | **string** | ID of the character (references /characters/{id}) | 
**Id** | **string** | Unique identifier for this team membership | 
**IsHeadKitman** | Pointer to **bool** | Whether this is the head equipment manager | [optional] [default to false]
**MemberType** | Pointer to **string** | Discriminator field indicating this is an equipment manager | [optional] [default to "equipment_manager"]
**Responsibilities** | Pointer to **[]string** | List of responsibilities | [optional] 
**TeamId** | **string** | ID of the team they belong to | 
**YearsWithTeam** | **int32** | Number of years with the current team | 

## Methods

### NewEquipmentManager

`func NewEquipmentManager(characterId string, id string, teamId string, yearsWithTeam int32, ) *EquipmentManager`

NewEquipmentManager instantiates a new EquipmentManager object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEquipmentManagerWithDefaults

`func NewEquipmentManagerWithDefaults() *EquipmentManager`

NewEquipmentManagerWithDefaults instantiates a new EquipmentManager object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCharacterId

`func (o *EquipmentManager) GetCharacterId() string`

GetCharacterId returns the CharacterId field if non-nil, zero value otherwise.

### GetCharacterIdOk

`func (o *EquipmentManager) GetCharacterIdOk() (*string, bool)`

GetCharacterIdOk returns a tuple with the CharacterId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCharacterId

`func (o *EquipmentManager) SetCharacterId(v string)`

SetCharacterId sets CharacterId field to given value.


### GetId

`func (o *EquipmentManager) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *EquipmentManager) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *EquipmentManager) SetId(v string)`

SetId sets Id field to given value.


### GetIsHeadKitman

`func (o *EquipmentManager) GetIsHeadKitman() bool`

GetIsHeadKitman returns the IsHeadKitman field if non-nil, zero value otherwise.

### GetIsHeadKitmanOk

`func (o *EquipmentManager) GetIsHeadKitmanOk() (*bool, bool)`

GetIsHeadKitmanOk returns a tuple with the IsHeadKitman field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsHeadKitman

`func (o *EquipmentManager) SetIsHeadKitman(v bool)`

SetIsHeadKitman sets IsHeadKitman field to given value.

### HasIsHeadKitman

`func (o *EquipmentManager) HasIsHeadKitman() bool`

HasIsHeadKitman returns a boolean if a field has been set.

### GetMemberType

`func (o *EquipmentManager) GetMemberType() string`

GetMemberType returns the MemberType field if non-nil, zero value otherwise.

### GetMemberTypeOk

`func (o *EquipmentManager) GetMemberTypeOk() (*string, bool)`

GetMemberTypeOk returns a tuple with the MemberType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMemberType

`func (o *EquipmentManager) SetMemberType(v string)`

SetMemberType sets MemberType field to given value.

### HasMemberType

`func (o *EquipmentManager) HasMemberType() bool`

HasMemberType returns a boolean if a field has been set.

### GetResponsibilities

`func (o *EquipmentManager) GetResponsibilities() []string`

GetResponsibilities returns the Responsibilities field if non-nil, zero value otherwise.

### GetResponsibilitiesOk

`func (o *EquipmentManager) GetResponsibilitiesOk() (*[]string, bool)`

GetResponsibilitiesOk returns a tuple with the Responsibilities field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponsibilities

`func (o *EquipmentManager) SetResponsibilities(v []string)`

SetResponsibilities sets Responsibilities field to given value.

### HasResponsibilities

`func (o *EquipmentManager) HasResponsibilities() bool`

HasResponsibilities returns a boolean if a field has been set.

### GetTeamId

`func (o *EquipmentManager) GetTeamId() string`

GetTeamId returns the TeamId field if non-nil, zero value otherwise.

### GetTeamIdOk

`func (o *EquipmentManager) GetTeamIdOk() (*string, bool)`

GetTeamIdOk returns a tuple with the TeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamId

`func (o *EquipmentManager) SetTeamId(v string)`

SetTeamId sets TeamId field to given value.


### GetYearsWithTeam

`func (o *EquipmentManager) GetYearsWithTeam() int32`

GetYearsWithTeam returns the YearsWithTeam field if non-nil, zero value otherwise.

### GetYearsWithTeamOk

`func (o *EquipmentManager) GetYearsWithTeamOk() (*int32, bool)`

GetYearsWithTeamOk returns a tuple with the YearsWithTeam field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetYearsWithTeam

`func (o *EquipmentManager) SetYearsWithTeam(v int32)`

SetYearsWithTeam sets YearsWithTeam field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


