# CharacterCreate

Model for creating a new character.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**background** | **str** | Character background and history | 
**date_of_birth** | **date** |  | [optional] 
**email** | **str** |  | [optional] 
**emotional_stats** | [**EmotionalStats**](EmotionalStats.md) | Emotional intelligence stats | 
**growth_arcs** | [**List[GrowthArc]**](GrowthArc.md) | Character development across seasons | [optional] 
**height_meters** | **float** |  | [optional] 
**name** | **str** | Character&#39;s full name | 
**personality_traits** | **List[str]** | Key personality traits | 
**profile_image_url** | **str** |  | [optional] 
**role** | [**CharacterRole**](CharacterRole.md) | Character&#39;s role | 
**salary_gbp** | [**SalaryGbp**](SalaryGbp.md) |  | [optional] 
**signature_quotes** | **List[str]** | Memorable quotes from this character | [optional] 
**team_id** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.character_create import CharacterCreate

# TODO update the JSON string below
json = "{}"
# create an instance of CharacterCreate from a JSON string
character_create_instance = CharacterCreate.from_json(json)
# print the JSON string representation of the object
print(CharacterCreate.to_json())

# convert the object into a dict
character_create_dict = character_create_instance.to_dict()
# create an instance of CharacterCreate from a dict
character_create_from_dict = CharacterCreate.from_dict(character_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


