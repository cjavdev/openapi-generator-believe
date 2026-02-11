# TeamUpdate

Model for updating a team (all fields optional).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**annual_budget_gbp** | [**AnnualBudgetGbp1**](AnnualBudgetGbp1.md) |  | [optional] 
**average_attendance** | **float** |  | [optional] 
**contact_email** | **str** |  | [optional] 
**culture_score** | **int** |  | [optional] 
**founded_year** | **int** |  | [optional] 
**is_active** | **bool** |  | [optional] 
**league** | [**League**](League.md) |  | [optional] 
**name** | **str** |  | [optional] 
**nickname** | **str** |  | [optional] 
**primary_color** | **str** |  | [optional] 
**rival_teams** | **List[str]** |  | [optional] 
**secondary_color** | **str** |  | [optional] 
**stadium** | **str** |  | [optional] 
**stadium_location** | [**GeoLocation**](GeoLocation.md) |  | [optional] 
**values** | [**TeamValues**](TeamValues.md) |  | [optional] 
**website** | **str** |  | [optional] 
**win_percentage** | **float** |  | [optional] 

## Example

```python
from openapi_client.models.team_update import TeamUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of TeamUpdate from a JSON string
team_update_instance = TeamUpdate.from_json(json)
# print the JSON string representation of the object
print(TeamUpdate.to_json())

# convert the object into a dict
team_update_dict = team_update_instance.to_dict()
# create an instance of TeamUpdate from a dict
team_update_from_dict = TeamUpdate.from_dict(team_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


