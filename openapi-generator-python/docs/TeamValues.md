# TeamValues

Core values that define a team's culture.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**primary_value** | **str** | The team&#39;s primary guiding value | 
**secondary_values** | **List[str]** | Supporting values | 
**team_motto** | **str** | Team&#39;s motivational motto | 

## Example

```python
from openapi_client.models.team_values import TeamValues

# TODO update the JSON string below
json = "{}"
# create an instance of TeamValues from a JSON string
team_values_instance = TeamValues.from_json(json)
# print the JSON string representation of the object
print(TeamValues.to_json())

# convert the object into a dict
team_values_dict = team_values_instance.to_dict()
# create an instance of TeamValues from a dict
team_values_from_dict = TeamValues.from_dict(team_values_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


