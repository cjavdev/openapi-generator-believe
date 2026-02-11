
# MatchCompletedData

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **awayScore** | **kotlin.Int** | Final away team score |  |
| **awayTeamId** | **kotlin.String** | Away team ID |  |
| **completedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | When the match completed |  |
| **homeScore** | **kotlin.Int** | Final home team score |  |
| **homeTeamId** | **kotlin.String** | Home team ID |  |
| **matchId** | **kotlin.String** | Unique match identifier |  |
| **matchType** | [**inline**](#MatchType) | Type of match |  |
| **result** | [**inline**](#Result) | Match result from home team perspective |  |
| **tedPostMatchQuote** | **kotlin.String** | Ted&#39;s post-match wisdom |  |
| **lessonLearned** | **kotlin.String** | Ted&#39;s lesson from the match |  [optional] |
| **manOfTheMatch** | **kotlin.String** | Player of the match (if awarded) |  [optional] |


<a id="MatchType"></a>
## Enum: match_type
| Name | Value |
| ---- | ----- |
| matchType | league, cup, friendly, playoff, final |


<a id="Result"></a>
## Enum: result
| Name | Value |
| ---- | ----- |
| result | home_win, away_win, draw |



