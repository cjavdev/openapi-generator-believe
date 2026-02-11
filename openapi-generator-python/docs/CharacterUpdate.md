# CharacterUpdate

Model for updating a character (all fields optional).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**background** | **str** |  | [optional] 
**date_of_birth** | **date** |  | [optional] 
**email** | **str** |  | [optional] 
**emotional_stats** | [**EmotionalStats**](EmotionalStats.md) |  | [optional] 
**growth_arcs** | [**List[GrowthArc]**](GrowthArc.md) |  | [optional] 
**height_meters** | **float** |  | [optional] 
**name** | **str** |  | [optional] 
**personality_traits** | **List[str]** |  | [optional] 
**profile_image_url** | **str** |  | [optional] 
**role** | [**CharacterRole**](CharacterRole.md) |  | [optional] 
**salary_gbp** | [**SalaryGbp1**](SalaryGbp1.md) |  | [optional] 
**signature_quotes** | **List[str]** |  | [optional] 
**team_id** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.character_update import CharacterUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of CharacterUpdate from a JSON string
character_update_instance = CharacterUpdate.from_json(json)
# print the JSON string representation of the object
print(CharacterUpdate.to_json())

# convert the object into a dict
character_update_dict = character_update_instance.to_dict()
# create an instance of CharacterUpdate from a dict
character_update_from_dict = CharacterUpdate.from_dict(character_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


