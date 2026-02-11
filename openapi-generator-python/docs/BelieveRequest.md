# BelieveRequest

Request for the Believe Engine.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | **str** |  | [optional] 
**intensity** | **int** | How intense is the response needed (1&#x3D;gentle, 10&#x3D;full Ted) | [optional] [default to 5]
**situation** | **str** | Describe your situation | 
**situation_type** | [**SituationType**](SituationType.md) | Type of situation | 

## Example

```python
from openapi_client.models.believe_request import BelieveRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BelieveRequest from a JSON string
believe_request_instance = BelieveRequest.from_json(json)
# print the JSON string representation of the object
print(BelieveRequest.to_json())

# convert the object into a dict
believe_request_dict = believe_request_instance.to_dict()
# create an instance of BelieveRequest from a dict
believe_request_from_dict = BelieveRequest.from_dict(believe_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


