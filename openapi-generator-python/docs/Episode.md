# Episode

Full episode model with ID.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**air_date** | **date** | Original air date | 
**biscuits_with_boss_moment** | **str** |  | [optional] 
**character_focus** | **List[str]** | Characters with significant development | 
**director** | **str** | Episode director | 
**episode_number** | **int** | Episode number within season | 
**id** | **str** | Unique identifier (format: s##e##) | 
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
from openapi_client.models.episode import Episode

# TODO update the JSON string below
json = "{}"
# create an instance of Episode from a JSON string
episode_instance = Episode.from_json(json)
# print the JSON string representation of the object
print(Episode.to_json())

# convert the object into a dict
episode_dict = episode_instance.to_dict()
# create an instance of Episode from a dict
episode_from_dict = Episode.from_dict(episode_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


