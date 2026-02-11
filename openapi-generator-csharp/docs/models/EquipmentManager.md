# Org.OpenAPITools.Model.EquipmentManager
Full equipment manager model with ID.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CharacterId** | **string** | ID of the character (references /characters/{id}) | 
**Id** | **string** | Unique identifier for this team membership | 
**TeamId** | **string** | ID of the team they belong to | 
**YearsWithTeam** | **int** | Number of years with the current team | 
**IsHeadKitman** | **bool** | Whether this is the head equipment manager | [optional] [default to false]
**MemberType** | **string** | Discriminator field indicating this is an equipment manager | [optional] [default to MemberTypeEnum.EquipmentManager]
**Responsibilities** | **List&lt;string&gt;** | List of responsibilities | [optional] 

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)

