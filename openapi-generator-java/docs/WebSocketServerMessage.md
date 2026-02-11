

# WebSocketServerMessage

Messages sent by the server during live match simulation.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**awayTeam** | **String** | Away team name |  |
|**homeTeam** | **String** | Home team name |  |
|**matchId** | **String** | Match identifier |  |
|**message** | **String** | Error description |  |
|**type** | [**TypeEnum**](#TypeEnum) | Message type |  |
|**event** | [**WebSocketLiveMatchEvent**](WebSocketLiveMatchEvent.md) |  |  |
|**finalScore** | [**WebSocketMatchScore**](WebSocketMatchScore.md) |  |  |
|**finalStats** | [**WebSocketMatchStats**](WebSocketMatchStats.md) |  |  |
|**manOfTheMatch** | **String** | Man of the match |  |
|**tedPostMatch** | **String** | Ted&#39;s post-match thoughts |  |
|**code** | **String** | Error code |  |



## Enum: TypeEnum

| Name | Value |
|---- | -----|
| MATCH_START | &quot;match_start&quot; |
| MATCH_EVENT | &quot;match_event&quot; |
| MATCH_END | &quot;match_end&quot; |
| ERROR | &quot;error&quot; |
| PONG | &quot;pong&quot; |



