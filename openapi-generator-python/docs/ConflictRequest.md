# ConflictRequest

Request for conflict resolution.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**attempts_made** | **List[str]** |  | [optional] 
**conflict_type** | [**ConflictType**](ConflictType.md) | Type of conflict | 
**description** | **str** | Describe the conflict | 
**parties_involved** | **List[str]** | Who is involved in the conflict | 

## Example

```python
from openapi_client.models.conflict_request import ConflictRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ConflictRequest from a JSON string
conflict_request_instance = ConflictRequest.from_json(json)
# print the JSON string representation of the object
print(ConflictRequest.to_json())

# convert the object into a dict
conflict_request_dict = conflict_request_instance.to_dict()
# create an instance of ConflictRequest from a dict
conflict_request_from_dict = ConflictRequest.from_dict(conflict_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


