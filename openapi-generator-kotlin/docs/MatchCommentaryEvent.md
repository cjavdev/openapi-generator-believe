
# MatchCommentaryEvent

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **commentary** | **kotlin.String** | Commentator&#39;s call |  |
| **description** | **kotlin.String** | What happened |  |
| **eventId** | **kotlin.Int** | Event sequence number |  |
| **eventType** | [**inline**](#EventType) | Type of event |  |
| **isFinal** | **kotlin.Boolean** | Is this the final event |  |
| **minute** | **kotlin.Int** | Match minute |  |
| **crowdReaction** | **kotlin.String** | How the crowd reacted |  [optional] |
| **tedSidelineReaction** | **kotlin.String** | Ted&#39;s reaction on the sideline |  [optional] |


<a id="EventType"></a>
## Enum: event_type
| Name | Value |
| ---- | ----- |
| eventType | kickoff, goal, near_miss, save, foul, substitution, halftime, ted_reaction, crowd_moment, final_whistle |



