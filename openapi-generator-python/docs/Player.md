# Player

Full player model with ID.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assists** | **int** | Total assists for the team | [optional] [default to 0]
**character_id** | **str** | ID of the character (references /characters/{id}) | 
**goals_scored** | **int** | Total goals scored for the team | [optional] [default to 0]
**id** | **str** | Unique identifier for this team membership | 
**is_captain** | **bool** | Whether this player is team captain | [optional] [default to False]
**jersey_number** | **int** | Jersey/shirt number | 
**member_type** | **str** | Discriminator field indicating this is a player | [optional] [default to 'player']
**position** | [**Position**](Position.md) | Playing position on the field | 
**team_id** | **str** | ID of the team they belong to | 
**years_with_team** | **int** | Number of years with the current team | 

## Example

```python
from openapi_client.models.player import Player

# TODO update the JSON string below
json = "{}"
# create an instance of Player from a JSON string
player_instance = Player.from_json(json)
# print the JSON string representation of the object
print(Player.to_json())

# convert the object into a dict
player_dict = player_instance.to_dict()
# create an instance of Player from a dict
player_from_dict = Player.from_dict(player_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


