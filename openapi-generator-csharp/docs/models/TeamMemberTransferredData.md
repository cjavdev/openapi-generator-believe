# Org.OpenAPITools.Model.TeamMemberTransferredData
Data payload for a team member transfer event.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CharacterId** | **string** | ID of the character (links to /characters) | 
**CharacterName** | **string** | Name of the character | 
**MemberType** | **string** | Type of team member | 
**TeamId** | **string** | ID of the team involved | 
**TeamMemberId** | **string** | ID of the team member | 
**TeamName** | **string** | Name of the team involved | 
**TedReaction** | **string** | Ted&#39;s reaction to the transfer | 
**TransferType** | **string** | Whether the member joined or departed | 
**PreviousTeamId** | **string** | Previous team ID (for joins from another team) | [optional] 
**PreviousTeamName** | **string** | Previous team name (for joins from another team) | [optional] 
**TransferFeeGbp** | **string** | Transfer fee in GBP (for players) | [optional] 
**YearsWithPreviousTeam** | **int** | Years spent with previous team | [optional] 

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)

