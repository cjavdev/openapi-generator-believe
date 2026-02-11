# EmotionalStats

Emotional intelligence statistics for a character.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**curiosity** | **int** | Level of curiosity over judgment (0-100) | 
**empathy** | **int** | Capacity for empathy (0-100) | 
**optimism** | **int** | Level of optimism (0-100) | 
**resilience** | **int** | Bounce-back ability (0-100) | 
**vulnerability** | **int** | Willingness to be vulnerable (0-100) | 

## Example

```python
from openapi_client.models.emotional_stats import EmotionalStats

# TODO update the JSON string below
json = "{}"
# create an instance of EmotionalStats from a JSON string
emotional_stats_instance = EmotionalStats.from_json(json)
# print the JSON string representation of the object
print(EmotionalStats.to_json())

# convert the object into a dict
emotional_stats_dict = emotional_stats_instance.to_dict()
# create an instance of EmotionalStats from a dict
emotional_stats_from_dict = EmotionalStats.from_dict(emotional_stats_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


