# PepTalkResponse

A complete pep talk response.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**chunks** | [**List[PepTalkChunk]**](PepTalkChunk.md) | Individual chunks of the pep talk | 
**text** | **str** | The full pep talk text | 

## Example

```python
from openapi_client.models.pep_talk_response import PepTalkResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PepTalkResponse from a JSON string
pep_talk_response_instance = PepTalkResponse.from_json(json)
# print the JSON string representation of the object
print(PepTalkResponse.to_json())

# convert the object into a dict
pep_talk_response_dict = pep_talk_response_instance.to_dict()
# create an instance of PepTalkResponse from a dict
pep_talk_response_from_dict = PepTalkResponse.from_dict(pep_talk_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


