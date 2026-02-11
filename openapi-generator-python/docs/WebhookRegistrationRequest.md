# WebhookRegistrationRequest

Request to register a new webhook endpoint.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** |  | [optional] 
**event_types** | **List[str]** |  | [optional] 
**url** | **str** | The URL to send webhook events to | 

## Example

```python
from openapi_client.models.webhook_registration_request import WebhookRegistrationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookRegistrationRequest from a JSON string
webhook_registration_request_instance = WebhookRegistrationRequest.from_json(json)
# print the JSON string representation of the object
print(WebhookRegistrationRequest.to_json())

# convert the object into a dict
webhook_registration_request_dict = webhook_registration_request_instance.to_dict()
# create an instance of WebhookRegistrationRequest from a dict
webhook_registration_request_from_dict = WebhookRegistrationRequest.from_dict(webhook_registration_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


