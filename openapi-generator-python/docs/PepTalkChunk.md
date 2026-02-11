# PepTalkChunk

A chunk of a streaming pep talk from Ted.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**chunk_id** | **int** | Chunk sequence number | 
**emotional_beat** | **str** | The emotional purpose of this chunk (e.g., greeting, acknowledgment, wisdom, affirmation, encouragement) | [optional] 
**is_final** | **bool** | Is this the final chunk | [default to False]
**text** | **str** | The text of this chunk | 

## Example

```python
from openapi_client.models.pep_talk_chunk import PepTalkChunk

# TODO update the JSON string below
json = "{}"
# create an instance of PepTalkChunk from a JSON string
pep_talk_chunk_instance = PepTalkChunk.from_json(json)
# print the JSON string representation of the object
print(PepTalkChunk.to_json())

# convert the object into a dict
pep_talk_chunk_dict = pep_talk_chunk_instance.to_dict()
# create an instance of PepTalkChunk from a dict
pep_talk_chunk_from_dict = PepTalkChunk.from_dict(pep_talk_chunk_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


