# Character

Full character model with ID.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**background** | **str** | Character background and history | 
**date_of_birth** | **date** |  | [optional] 
**email** | **str** |  | [optional] 
**emotional_stats** | [**EmotionalStats**](EmotionalStats.md) | Emotional intelligence stats | 
**growth_arcs** | [**List[GrowthArc]**](GrowthArc.md) | Character development across seasons | [optional] 
**height_meters** | **float** |  | [optional] 
**id** | **str** | Unique identifier | 
**name** | **str** | Character&#39;s full name | 
**personality_traits** | **List[str]** | Key personality traits | 
**profile_image_url** | **str** |  | [optional] 
**role** | [**CharacterRole**](CharacterRole.md) | Character&#39;s role | 
**salary_gbp** | **str** |  | [optional] 
**signature_quotes** | **List[str]** | Memorable quotes from this character | [optional] 
**team_id** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.character import Character

# TODO update the JSON string below
json = "{}"
# create an instance of Character from a JSON string
character_instance = Character.from_json(json)
# print the JSON string representation of the object
print(Character.to_json())

# convert the object into a dict
character_dict = character_instance.to_dict()
# create an instance of Character from a dict
character_from_dict = Character.from_dict(character_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


