# TriggerEventResponse

Response after triggering webhook events.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**deliveries** | [**List[WebhookDeliveryResult]**](WebhookDeliveryResult.md) | Results of webhook deliveries | 
**event_id** | **str** | Unique event identifier | 
**event_type** | **str** | The type of event triggered | 
**successful_deliveries** | **int** | Number of successful deliveries | 
**ted_says** | **str** | Ted&#39;s reaction | 
**total_webhooks** | **int** | Total number of webhooks that received this event | 

## Example

```python
from openapi_client.models.trigger_event_response import TriggerEventResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TriggerEventResponse from a JSON string
trigger_event_response_instance = TriggerEventResponse.from_json(json)
# print the JSON string representation of the object
print(TriggerEventResponse.to_json())

# convert the object into a dict
trigger_event_response_dict = trigger_event_response_instance.to_dict()
# create an instance of TriggerEventResponse from a dict
trigger_event_response_from_dict = TriggerEventResponse.from_dict(trigger_event_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


