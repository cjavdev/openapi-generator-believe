

# WebSocketLiveMatchEvent

A live match event with full details.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**addedTime** | **Integer** | Added/injury time minutes |  [optional] |
|**commentary** | **String** | Match commentary for this event |  |
|**crowdReaction** | **String** | Crowd reaction to the event |  [optional] |
|**description** | **String** | Human-readable event description |  |
|**eventId** | **Integer** | Unique event sequence number |  |
|**eventType** | [**EventTypeEnum**](#EventTypeEnum) | Type of match event |  |
|**minute** | **Integer** | Match minute |  |
|**player** | [**WebSocketPlayerInfo**](WebSocketPlayerInfo.md) |  |  [optional] |
|**score** | [**WebSocketMatchScore**](WebSocketMatchScore.md) |  |  |
|**secondaryPlayer** | [**WebSocketPlayerInfo**](WebSocketPlayerInfo.md) | Second player involved (e.g., assist, replaced player) |  [optional] |
|**stats** | [**WebSocketMatchStats**](WebSocketMatchStats.md) |  |  |
|**team** | [**TeamEnum**](#TeamEnum) | Which team the event relates to |  [optional] |
|**tedReaction** | **String** | Ted Lasso&#39;s sideline reaction |  [optional] |



## Enum: EventTypeEnum

| Name | Value |
|---- | -----|
| MATCH_START | &quot;match_start&quot; |
| GOAL | &quot;goal&quot; |
| POSSESSION_CHANGE | &quot;possession_change&quot; |
| FOUL | &quot;foul&quot; |
| YELLOW_CARD | &quot;yellow_card&quot; |
| RED_CARD | &quot;red_card&quot; |
| PENALTY_AWARDED | &quot;penalty_awarded&quot; |
| PENALTY_SCORED | &quot;penalty_scored&quot; |
| PENALTY_MISSED | &quot;penalty_missed&quot; |
| SUBSTITUTION | &quot;substitution&quot; |
| INJURY | &quot;injury&quot; |
| OFFSIDE | &quot;offside&quot; |
| CORNER | &quot;corner&quot; |
| FREE_KICK | &quot;free_kick&quot; |
| SHOT_ON_TARGET | &quot;shot_on_target&quot; |
| SHOT_OFF_TARGET | &quot;shot_off_target&quot; |
| SAVE | &quot;save&quot; |
| HALFTIME | &quot;halftime&quot; |
| SECOND_HALF_START | &quot;second_half_start&quot; |
| ADDED_TIME | &quot;added_time&quot; |
| MATCH_END | &quot;match_end&quot; |



## Enum: TeamEnum

| Name | Value |
|---- | -----|
| HOME | &quot;home&quot; |
| AWAY | &quot;away&quot; |



