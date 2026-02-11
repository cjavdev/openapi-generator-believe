# EpisodeCreate

Model for creating a new episode.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**air_date** | **date** | Original air date | 
**biscuits_with_boss_moment** | **str** |  | [optional] 
**character_focus** | **List[str]** | Characters with significant development | 
**director** | **str** | Episode director | 
**episode_number** | **int** | Episode number within season | 
**main_theme** | **str** | Central theme of the episode | 
**memorable_moments** | **List[str]** | Standout moments from the episode | [optional] 
**runtime_minutes** | **int** | Episode runtime in minutes | 
**season** | **int** | Season number | 
**synopsis** | **str** | Brief plot synopsis | 
**ted_wisdom** | **str** | Key piece of Ted wisdom from the episode | 
**title** | **str** | Episode title | 
**us_viewers_millions** | **float** |  | [optional] 
**viewer_rating** | **float** |  | [optional] 
**writer** | **str** | Episode writer(s) | 

## Example

```python
from openapi_client.models.episode_create import EpisodeCreate

# TODO update the JSON string below
json = "{}"
# create an instance of EpisodeCreate from a JSON string
episode_create_instance = EpisodeCreate.from_json(json)
# print the JSON string representation of the object
print(EpisodeCreate.to_json())

# convert the object into a dict
episode_create_dict = episode_create_instance.to_dict()
# create an instance of EpisodeCreate from a dict
episode_create_from_dict = EpisodeCreate.from_dict(episode_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


