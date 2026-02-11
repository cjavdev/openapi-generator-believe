
# TeamMemberTransferredData

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **characterId** | **kotlin.String** | ID of the character (links to /characters) |  |
| **characterName** | **kotlin.String** | Name of the character |  |
| **memberType** | [**inline**](#MemberType) | Type of team member |  |
| **teamId** | **kotlin.String** | ID of the team involved |  |
| **teamMemberId** | **kotlin.String** | ID of the team member |  |
| **teamName** | **kotlin.String** | Name of the team involved |  |
| **tedReaction** | **kotlin.String** | Ted&#39;s reaction to the transfer |  |
| **transferType** | [**inline**](#TransferType) | Whether the member joined or departed |  |
| **previousTeamId** | **kotlin.String** | Previous team ID (for joins from another team) |  [optional] |
| **previousTeamName** | **kotlin.String** | Previous team name (for joins from another team) |  [optional] |
| **transferFeeGbp** | **kotlin.String** | Transfer fee in GBP (for players) |  [optional] |
| **yearsWithPreviousTeam** | **kotlin.Int** | Years spent with previous team |  [optional] |


<a id="MemberType"></a>
## Enum: member_type
| Name | Value |
| ---- | ----- |
| memberType | player, coach, medical_staff, equipment_manager |


<a id="TransferType"></a>
## Enum: transfer_type
| Name | Value |
| ---- | ----- |
| transferType | joined, departed |



