# MatchCreate

Model for creating a new match.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**attendance** | **int** |  | [optional] 
**away_score** | **int** | Away team score | [optional] [default to 0]
**away_team_id** | **str** | Away team ID | 
**var_date** | **datetime** | Match date and time | 
**episode_id** | **str** |  | [optional] 
**home_score** | **int** | Home team score | [optional] [default to 0]
**home_team_id** | **str** | Home team ID | 
**lesson_learned** | **str** |  | [optional] 
**match_type** | [**MatchType**](MatchType.md) | Type of match | 
**possession_percentage** | **float** |  | [optional] 
**result** | [**MatchResult**](MatchResult.md) | Match result from home team perspective | [optional] 
**ted_halftime_speech** | **str** |  | [optional] 
**ticket_revenue_gbp** | [**TicketRevenueGbp**](TicketRevenueGbp.md) |  | [optional] 
**turning_points** | [**List[TurningPoint]**](TurningPoint.md) | Key moments that changed the match | [optional] 
**weather_temp_celsius** | **float** |  | [optional] 

## Example

```python
from openapi_client.models.match_create import MatchCreate

# TODO update the JSON string below
json = "{}"
# create an instance of MatchCreate from a JSON string
match_create_instance = MatchCreate.from_json(json)
# print the JSON string representation of the object
print(MatchCreate.to_json())

# convert the object into a dict
match_create_dict = match_create_instance.to_dict()
# create an instance of MatchCreate from a dict
match_create_from_dict = MatchCreate.from_dict(match_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


