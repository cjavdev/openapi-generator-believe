
# WebSocketLiveMatchEvent

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **commentary** | **kotlin.String** | Match commentary for this event |  |
| **description** | **kotlin.String** | Human-readable event description |  |
| **eventId** | **kotlin.Int** | Unique event sequence number |  |
| **eventType** | [**inline**](#EventType) | Type of match event |  |
| **minute** | **kotlin.Int** | Match minute |  |
| **score** | [**WebSocketMatchScore**](WebSocketMatchScore.md) |  |  |
| **stats** | [**WebSocketMatchStats**](WebSocketMatchStats.md) |  |  |
| **addedTime** | **kotlin.Int** | Added/injury time minutes |  [optional] |
| **crowdReaction** | **kotlin.String** | Crowd reaction to the event |  [optional] |
| **player** | [**WebSocketPlayerInfo**](WebSocketPlayerInfo.md) |  |  [optional] |
| **secondaryPlayer** | [**WebSocketPlayerInfo**](WebSocketPlayerInfo.md) | Second player involved (e.g., assist, replaced player) |  [optional] |
| **team** | [**inline**](#Team) | Which team the event relates to |  [optional] |
| **tedReaction** | **kotlin.String** | Ted Lasso&#39;s sideline reaction |  [optional] |


<a id="EventType"></a>
## Enum: event_type
| Name | Value |
| ---- | ----- |
| eventType | match_start, goal, possession_change, foul, yellow_card, red_card, penalty_awarded, penalty_scored, penalty_missed, substitution, injury, offside, corner, free_kick, shot_on_target, shot_off_target, save, halftime, second_half_start, added_time, match_end |


<a id="Team"></a>
## Enum: team
| Name | Value |
| ---- | ----- |
| team | home, away |



