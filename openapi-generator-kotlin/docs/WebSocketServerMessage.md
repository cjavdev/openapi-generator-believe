
# WebSocketServerMessage

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **awayTeam** | **kotlin.String** | Away team name |  |
| **homeTeam** | **kotlin.String** | Home team name |  |
| **matchId** | **kotlin.String** | Match identifier |  |
| **message** | **kotlin.String** | Error description |  |
| **type** | [**inline**](#Type) | Message type |  |
| **event** | [**WebSocketLiveMatchEvent**](WebSocketLiveMatchEvent.md) |  |  |
| **finalScore** | [**WebSocketMatchScore**](WebSocketMatchScore.md) |  |  |
| **finalStats** | [**WebSocketMatchStats**](WebSocketMatchStats.md) |  |  |
| **manOfTheMatch** | **kotlin.String** | Man of the match |  |
| **tedPostMatch** | **kotlin.String** | Ted&#39;s post-match thoughts |  |
| **code** | **kotlin.String** | Error code |  |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | match_start, match_event, match_end, error, pong |



