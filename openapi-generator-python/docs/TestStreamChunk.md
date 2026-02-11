# TestStreamChunk

A test stream chunk for SSE connectivity testing.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** | The message content for this chunk | 
**sequence** | **int** | The sequence number of this chunk (1-5) | 

## Example

```python
from openapi_client.models.test_stream_chunk import TestStreamChunk

# TODO update the JSON string below
json = "{}"
# create an instance of TestStreamChunk from a JSON string
test_stream_chunk_instance = TestStreamChunk.from_json(json)
# print the JSON string representation of the object
print(TestStreamChunk.to_json())

# convert the object into a dict
test_stream_chunk_dict = test_stream_chunk_instance.to_dict()
# create an instance of TestStreamChunk from a dict
test_stream_chunk_from_dict = TestStreamChunk.from_dict(test_stream_chunk_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


