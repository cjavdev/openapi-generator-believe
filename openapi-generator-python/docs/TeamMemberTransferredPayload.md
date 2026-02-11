# TeamMemberTransferredPayload

Payload for team_member.transferred event.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**TeamMemberTransferredData**](TeamMemberTransferredData.md) | Event data | 
**event_type** | **str** | The type of webhook event | [optional] [default to 'team_member.transferred']

## Example

```python
from openapi_client.models.team_member_transferred_payload import TeamMemberTransferredPayload

# TODO update the JSON string below
json = "{}"
# create an instance of TeamMemberTransferredPayload from a JSON string
team_member_transferred_payload_instance = TeamMemberTransferredPayload.from_json(json)
# print the JSON string representation of the object
print(TeamMemberTransferredPayload.to_json())

# convert the object into a dict
team_member_transferred_payload_dict = team_member_transferred_payload_instance.to_dict()
# create an instance of TeamMemberTransferredPayload from a dict
team_member_transferred_payload_from_dict = TeamMemberTransferredPayload.from_dict(team_member_transferred_payload_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


