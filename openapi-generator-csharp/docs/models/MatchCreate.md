# Org.OpenAPITools.Model.MatchCreate
Model for creating a new match.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AwayTeamId** | **string** | Away team ID | 
**Date** | **DateTime** | Match date and time | 
**HomeTeamId** | **string** | Home team ID | 
**MatchType** | **MatchType** | Type of match | 
**Attendance** | **int** |  | [optional] 
**AwayScore** | **int** | Away team score | [optional] [default to 0]
**EpisodeId** | **string** |  | [optional] 
**HomeScore** | **int** | Home team score | [optional] [default to 0]
**LessonLearned** | **string** |  | [optional] 
**PossessionPercentage** | **decimal** |  | [optional] 
**Result** | **MatchResult** | Match result from home team perspective | [optional] 
**TedHalftimeSpeech** | **string** |  | [optional] 
**TicketRevenueGbp** | [**TicketRevenueGbp**](TicketRevenueGbp.md) |  | [optional] 
**TurningPoints** | [**List&lt;TurningPoint&gt;**](TurningPoint.md) | Key moments that changed the match | [optional] 
**WeatherTempCelsius** | **decimal** |  | [optional] 

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)

