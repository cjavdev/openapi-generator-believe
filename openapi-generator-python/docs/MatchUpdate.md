# MatchUpdate

Model for updating a match (all fields optional).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**attendance** | **int** |  | [optional] 
**away_score** | **int** |  | [optional] 
**away_team_id** | **str** |  | [optional] 
**var_date** | **datetime** |  | [optional] 
**episode_id** | **str** |  | [optional] 
**home_score** | **int** |  | [optional] 
**home_team_id** | **str** |  | [optional] 
**lesson_learned** | **str** |  | [optional] 
**match_type** | [**MatchType**](MatchType.md) |  | [optional] 
**possession_percentage** | **float** |  | [optional] 
**result** | [**MatchResult**](MatchResult.md) |  | [optional] 
**ted_halftime_speech** | **str** |  | [optional] 
**ticket_revenue_gbp** | [**TicketRevenueGbp1**](TicketRevenueGbp1.md) |  | [optional] 
**turning_points** | [**List[TurningPoint]**](TurningPoint.md) |  | [optional] 
**weather_temp_celsius** | **float** |  | [optional] 

## Example

```python
from openapi_client.models.match_update import MatchUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of MatchUpdate from a JSON string
match_update_instance = MatchUpdate.from_json(json)
# print the JSON string representation of the object
print(MatchUpdate.to_json())

# convert the object into a dict
match_update_dict = match_update_instance.to_dict()
# create an instance of MatchUpdate from a dict
match_update_from_dict = MatchUpdate.from_dict(match_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


