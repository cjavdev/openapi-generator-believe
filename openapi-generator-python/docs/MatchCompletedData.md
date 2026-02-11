# MatchCompletedData

Data payload for a match completed event.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**away_score** | **int** | Final away team score | 
**away_team_id** | **str** | Away team ID | 
**completed_at** | **datetime** | When the match completed | 
**home_score** | **int** | Final home team score | 
**home_team_id** | **str** | Home team ID | 
**lesson_learned** | **str** | Ted&#39;s lesson from the match | [optional] 
**man_of_the_match** | **str** | Player of the match (if awarded) | [optional] 
**match_id** | **str** | Unique match identifier | 
**match_type** | **str** | Type of match | 
**result** | **str** | Match result from home team perspective | 
**ted_post_match_quote** | **str** | Ted&#39;s post-match wisdom | 

## Example

```python
from openapi_client.models.match_completed_data import MatchCompletedData

# TODO update the JSON string below
json = "{}"
# create an instance of MatchCompletedData from a JSON string
match_completed_data_instance = MatchCompletedData.from_json(json)
# print the JSON string representation of the object
print(MatchCompletedData.to_json())

# convert the object into a dict
match_completed_data_dict = match_completed_data_instance.to_dict()
# create an instance of MatchCompletedData from a dict
match_completed_data_from_dict = MatchCompletedData.from_dict(match_completed_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


