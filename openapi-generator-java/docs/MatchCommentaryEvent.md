

# MatchCommentaryEvent

A single commentary event during a match stream.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**commentary** | **String** | Commentator&#39;s call |  |
|**crowdReaction** | **String** | How the crowd reacted |  [optional] |
|**description** | **String** | What happened |  |
|**eventId** | **Integer** | Event sequence number |  |
|**eventType** | [**EventTypeEnum**](#EventTypeEnum) | Type of event |  |
|**isFinal** | **Boolean** | Is this the final event |  |
|**minute** | **Integer** | Match minute |  |
|**tedSidelineReaction** | **String** | Ted&#39;s reaction on the sideline |  [optional] |



## Enum: EventTypeEnum

| Name | Value |
|---- | -----|
| KICKOFF | &quot;kickoff&quot; |
| GOAL | &quot;goal&quot; |
| NEAR_MISS | &quot;near_miss&quot; |
| SAVE | &quot;save&quot; |
| FOUL | &quot;foul&quot; |
| SUBSTITUTION | &quot;substitution&quot; |
| HALFTIME | &quot;halftime&quot; |
| TED_REACTION | &quot;ted_reaction&quot; |
| CROWD_MOMENT | &quot;crowd_moment&quot; |
| FINAL_WHISTLE | &quot;final_whistle&quot; |



