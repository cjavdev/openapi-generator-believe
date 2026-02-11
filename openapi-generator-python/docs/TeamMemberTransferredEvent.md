# TeamMemberTransferredEvent

Webhook event sent when a team member (player, coach, staff) transfers between teams.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **datetime** | When the event was created | 
**data** | [**TeamMemberTransferredData**](TeamMemberTransferredData.md) |  | 
**event_id** | **UUID** | Unique identifier for this event | 
**event_type** | **str** | The type of webhook event | 

## Example

```python
from openapi_client.models.team_member_transferred_event import TeamMemberTransferredEvent

# TODO update the JSON string below
json = "{}"
# create an instance of TeamMemberTransferredEvent from a JSON string
team_member_transferred_event_instance = TeamMemberTransferredEvent.from_json(json)
# print the JSON string representation of the object
print(TeamMemberTransferredEvent.to_json())

# convert the object into a dict
team_member_transferred_event_dict = team_member_transferred_event_instance.to_dict()
# create an instance of TeamMemberTransferredEvent from a dict
team_member_transferred_event_from_dict = TeamMemberTransferredEvent.from_dict(team_member_transferred_event_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


