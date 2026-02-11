

# MatchCompletedData

Data payload for a match completed event.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**awayScore** | **Integer** | Final away team score |  |
|**awayTeamId** | **String** | Away team ID |  |
|**completedAt** | **OffsetDateTime** | When the match completed |  |
|**homeScore** | **Integer** | Final home team score |  |
|**homeTeamId** | **String** | Home team ID |  |
|**lessonLearned** | **String** | Ted&#39;s lesson from the match |  [optional] |
|**manOfTheMatch** | **String** | Player of the match (if awarded) |  [optional] |
|**matchId** | **String** | Unique match identifier |  |
|**matchType** | [**MatchTypeEnum**](#MatchTypeEnum) | Type of match |  |
|**result** | [**ResultEnum**](#ResultEnum) | Match result from home team perspective |  |
|**tedPostMatchQuote** | **String** | Ted&#39;s post-match wisdom |  |



## Enum: MatchTypeEnum

| Name | Value |
|---- | -----|
| LEAGUE | &quot;league&quot; |
| CUP | &quot;cup&quot; |
| FRIENDLY | &quot;friendly&quot; |
| PLAYOFF | &quot;playoff&quot; |
| FINAL | &quot;final&quot; |



## Enum: ResultEnum

| Name | Value |
|---- | -----|
| HOME_WIN | &quot;home_win&quot; |
| AWAY_WIN | &quot;away_win&quot; |
| DRAW | &quot;draw&quot; |



