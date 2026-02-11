

# WebSocketMatchEndMessage

Message sent when a match simulation ends.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**finalScore** | [**WebSocketMatchScore**](WebSocketMatchScore.md) |  |  |
|**finalStats** | [**WebSocketMatchStats**](WebSocketMatchStats.md) |  |  |
|**manOfTheMatch** | **String** | Man of the match |  |
|**matchId** | **String** | Match identifier |  |
|**tedPostMatch** | **String** | Ted&#39;s post-match thoughts |  |
|**type** | [**TypeEnum**](#TypeEnum) | Message type |  |



## Enum: TypeEnum

| Name | Value |
|---- | -----|
| MATCH_END | &quot;match_end&quot; |



