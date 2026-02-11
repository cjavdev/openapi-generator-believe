# TurningPoint

A pivotal moment in a match.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**character_involved** | **str** |  | [optional] 
**description** | **str** | What happened | 
**emotional_impact** | **str** | How this affected the team emotionally | 
**minute** | **int** | Minute of the match | 

## Example

```python
from openapi_client.models.turning_point import TurningPoint

# TODO update the JSON string below
json = "{}"
# create an instance of TurningPoint from a JSON string
turning_point_instance = TurningPoint.from_json(json)
# print the JSON string representation of the object
print(TurningPoint.to_json())

# convert the object into a dict
turning_point_dict = turning_point_instance.to_dict()
# create an instance of TurningPoint from a dict
turning_point_from_dict = TurningPoint.from_dict(turning_point_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


