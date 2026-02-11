# OpenapiClient::TeamMemberTransferredData

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **character_id** | **String** | ID of the character (links to /characters) |  |
| **character_name** | **String** | Name of the character |  |
| **member_type** | **String** | Type of team member |  |
| **previous_team_id** | **String** | Previous team ID (for joins from another team) | [optional] |
| **previous_team_name** | **String** | Previous team name (for joins from another team) | [optional] |
| **team_id** | **String** | ID of the team involved |  |
| **team_member_id** | **String** | ID of the team member |  |
| **team_name** | **String** | Name of the team involved |  |
| **ted_reaction** | **String** | Ted&#39;s reaction to the transfer |  |
| **transfer_fee_gbp** | **String** | Transfer fee in GBP (for players) | [optional] |
| **transfer_type** | **String** | Whether the member joined or departed |  |
| **years_with_previous_team** | **Integer** | Years spent with previous team | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TeamMemberTransferredData.new(
  character_id: null,
  character_name: null,
  member_type: null,
  previous_team_id: null,
  previous_team_name: null,
  team_id: null,
  team_member_id: null,
  team_name: null,
  ted_reaction: null,
  transfer_fee_gbp: null,
  transfer_type: null,
  years_with_previous_team: null
)
```

