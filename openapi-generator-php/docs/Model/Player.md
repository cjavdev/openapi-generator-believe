# # Player

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assists** | **int** | Total assists for the team | [optional] [default to 0]
**character_id** | **string** | ID of the character (references /characters/{id}) |
**goals_scored** | **int** | Total goals scored for the team | [optional] [default to 0]
**id** | **string** | Unique identifier for this team membership |
**is_captain** | **bool** | Whether this player is team captain | [optional] [default to false]
**jersey_number** | **int** | Jersey/shirt number |
**member_type** | **string** | Discriminator field indicating this is a player | [optional] [default to 'player']
**position** | [**\OpenAPI\Client\Model\Position**](Position.md) | Playing position on the field |
**team_id** | **string** | ID of the team they belong to |
**years_with_team** | **int** | Number of years with the current team |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
