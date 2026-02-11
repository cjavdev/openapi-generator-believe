# TeamMemberTransferredData

Data payload for a team member transfer event.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**character_id** | **str** | ID of the character (links to /characters) | 
**character_name** | **str** | Name of the character | 
**member_type** | **str** | Type of team member | 
**previous_team_id** | **str** | Previous team ID (for joins from another team) | [optional] 
**previous_team_name** | **str** | Previous team name (for joins from another team) | [optional] 
**team_id** | **str** | ID of the team involved | 
**team_member_id** | **str** | ID of the team member | 
**team_name** | **str** | Name of the team involved | 
**ted_reaction** | **str** | Ted&#39;s reaction to the transfer | 
**transfer_fee_gbp** | **str** | Transfer fee in GBP (for players) | [optional] 
**transfer_type** | **str** | Whether the member joined or departed | 
**years_with_previous_team** | **int** | Years spent with previous team | [optional] 

## Example

```python
from openapi_client.models.team_member_transferred_data import TeamMemberTransferredData

# TODO update the JSON string below
json = "{}"
# create an instance of TeamMemberTransferredData from a JSON string
team_member_transferred_data_instance = TeamMemberTransferredData.from_json(json)
# print the JSON string representation of the object
print(TeamMemberTransferredData.to_json())

# convert the object into a dict
team_member_transferred_data_dict = team_member_transferred_data_instance.to_dict()
# create an instance of TeamMemberTransferredData from a dict
team_member_transferred_data_from_dict = TeamMemberTransferredData.from_dict(team_member_transferred_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


