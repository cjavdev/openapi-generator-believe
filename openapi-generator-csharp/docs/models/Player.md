# Org.OpenAPITools.Model.Player
Full player model with ID.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CharacterId** | **string** | ID of the character (references /characters/{id}) | 
**Id** | **string** | Unique identifier for this team membership | 
**JerseyNumber** | **int** | Jersey/shirt number | 
**Position** | **Position** | Playing position on the field | 
**TeamId** | **string** | ID of the team they belong to | 
**YearsWithTeam** | **int** | Number of years with the current team | 
**Assists** | **int** | Total assists for the team | [optional] [default to 0]
**GoalsScored** | **int** | Total goals scored for the team | [optional] [default to 0]
**IsCaptain** | **bool** | Whether this player is team captain | [optional] [default to false]
**MemberType** | **string** | Discriminator field indicating this is a player | [optional] [default to MemberTypeEnum.Player]

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)

