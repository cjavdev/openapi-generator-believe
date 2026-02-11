# TeamCreate

Model for creating a new team.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**annual_budget_gbp** | [**AnnualBudgetGbp**](AnnualBudgetGbp.md) |  | [optional] 
**average_attendance** | **float** |  | [optional] 
**contact_email** | **str** |  | [optional] 
**culture_score** | **int** | Team culture/morale score (0-100) | 
**founded_year** | **int** | Year the club was founded | 
**is_active** | **bool** | Whether the team is currently active | [optional] [default to True]
**league** | [**League**](League.md) | Current league | 
**name** | **str** | Team name | 
**nickname** | **str** |  | [optional] 
**primary_color** | **str** |  | [optional] 
**rival_teams** | **List[str]** | List of rival team IDs | [optional] 
**secondary_color** | **str** |  | [optional] 
**stadium** | **str** | Home stadium name | 
**stadium_location** | [**GeoLocation**](GeoLocation.md) |  | [optional] 
**values** | [**TeamValues**](TeamValues.md) | Team&#39;s core values | 
**website** | **str** |  | [optional] 
**win_percentage** | **float** |  | [optional] 

## Example

```python
from openapi_client.models.team_create import TeamCreate

# TODO update the JSON string below
json = "{}"
# create an instance of TeamCreate from a JSON string
team_create_instance = TeamCreate.from_json(json)
# print the JSON string representation of the object
print(TeamCreate.to_json())

# convert the object into a dict
team_create_dict = team_create_instance.to_dict()
# create an instance of TeamCreate from a dict
team_create_from_dict = TeamCreate.from_dict(team_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


