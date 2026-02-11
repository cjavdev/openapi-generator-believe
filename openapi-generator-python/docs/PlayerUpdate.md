# PlayerUpdate

Update model for players.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assists** | **int** |  | [optional] 
**goals_scored** | **int** |  | [optional] 
**is_captain** | **bool** |  | [optional] 
**jersey_number** | **int** |  | [optional] 
**position** | [**Position**](Position.md) |  | [optional] 
**team_id** | **str** |  | [optional] 
**years_with_team** | **int** |  | [optional] 

## Example

```python
from openapi_client.models.player_update import PlayerUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of PlayerUpdate from a JSON string
player_update_instance = PlayerUpdate.from_json(json)
# print the JSON string representation of the object
print(PlayerUpdate.to_json())

# convert the object into a dict
player_update_dict = player_update_instance.to_dict()
# create an instance of PlayerUpdate from a dict
player_update_from_dict = PlayerUpdate.from_dict(player_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


