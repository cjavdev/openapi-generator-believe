# MatchCommentaryEvent

A single commentary event during a match stream.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**commentary** | **str** | Commentator&#39;s call | 
**crowd_reaction** | **str** | How the crowd reacted | [optional] 
**description** | **str** | What happened | 
**event_id** | **int** | Event sequence number | 
**event_type** | **str** | Type of event | 
**is_final** | **bool** | Is this the final event | [default to False]
**minute** | **int** | Match minute | 
**ted_sideline_reaction** | **str** | Ted&#39;s reaction on the sideline | [optional] 

## Example

```python
from openapi_client.models.match_commentary_event import MatchCommentaryEvent

# TODO update the JSON string below
json = "{}"
# create an instance of MatchCommentaryEvent from a JSON string
match_commentary_event_instance = MatchCommentaryEvent.from_json(json)
# print the JSON string representation of the object
print(MatchCommentaryEvent.to_json())

# convert the object into a dict
match_commentary_event_dict = match_commentary_event_instance.to_dict()
# create an instance of MatchCommentaryEvent from a dict
match_commentary_event_from_dict = MatchCommentaryEvent.from_dict(match_commentary_event_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


