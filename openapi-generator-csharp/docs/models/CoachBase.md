# Org.OpenAPITools.Model.CoachBase
A coach or coaching staff member.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CharacterId** | **string** | ID of the character (references /characters/{id}) | 
**Specialty** | **CoachSpecialty** | Coaching specialty/role | 
**TeamId** | **string** | ID of the team they belong to | 
**YearsWithTeam** | **int** | Number of years with the current team | 
**Certifications** | **List&lt;string&gt;** | Coaching certifications and licenses | [optional] 
**MemberType** | **string** | Discriminator field indicating this is a coach | [optional] [default to MemberTypeEnum.Coach]
**WinRate** | **decimal** |  | [optional] 

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)

