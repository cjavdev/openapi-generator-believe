# Biscuit

A biscuit from Ted.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Biscuit identifier | 
**message** | **str** | Message that comes with the biscuit | 
**pairs_well_with** | **str** | What this biscuit pairs well with | 
**ted_note** | **str** | A handwritten note from Ted | 
**type** | [**BiscuitType**](BiscuitType.md) | Type of biscuit | 
**warmth_level** | **int** | How warm and fresh (1-10) | 

## Example

```python
from openapi_client.models.biscuit import Biscuit

# TODO update the JSON string below
json = "{}"
# create an instance of Biscuit from a JSON string
biscuit_instance = Biscuit.from_json(json)
# print the JSON string representation of the object
print(Biscuit.to_json())

# convert the object into a dict
biscuit_dict = biscuit_instance.to_dict()
# create an instance of Biscuit from a dict
biscuit_from_dict = Biscuit.from_dict(biscuit_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


