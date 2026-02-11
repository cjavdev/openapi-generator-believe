# EpisodeUpdate

Model for updating an episode (all fields optional).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**air_date** | **date** |  | [optional] 
**biscuits_with_boss_moment** | **str** |  | [optional] 
**character_focus** | **List[str]** |  | [optional] 
**director** | **str** |  | [optional] 
**episode_number** | **int** |  | [optional] 
**main_theme** | **str** |  | [optional] 
**memorable_moments** | **List[str]** |  | [optional] 
**runtime_minutes** | **int** |  | [optional] 
**season** | **int** |  | [optional] 
**synopsis** | **str** |  | [optional] 
**ted_wisdom** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**us_viewers_millions** | **float** |  | [optional] 
**viewer_rating** | **float** |  | [optional] 
**writer** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.episode_update import EpisodeUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of EpisodeUpdate from a JSON string
episode_update_instance = EpisodeUpdate.from_json(json)
# print the JSON string representation of the object
print(EpisodeUpdate.to_json())

# convert the object into a dict
episode_update_dict = episode_update_instance.to_dict()
# create an instance of EpisodeUpdate from a dict
episode_update_from_dict = EpisodeUpdate.from_dict(episode_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


