# OpenapiClient::Match

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **attendance** | **Integer** |  | [optional] |
| **away_score** | **Integer** | Away team score | [optional][default to 0] |
| **away_team_id** | **String** | Away team ID |  |
| **date** | **Time** | Match date and time |  |
| **episode_id** | **String** |  | [optional] |
| **home_score** | **Integer** | Home team score | [optional][default to 0] |
| **home_team_id** | **String** | Home team ID |  |
| **id** | **String** | Unique identifier |  |
| **lesson_learned** | **String** |  | [optional] |
| **match_type** | [**MatchType**](MatchType.md) | Type of match |  |
| **possession_percentage** | **Float** |  | [optional] |
| **result** | [**MatchResult**](MatchResult.md) | Match result from home team perspective | [optional] |
| **ted_halftime_speech** | **String** |  | [optional] |
| **ticket_revenue_gbp** | **String** |  | [optional] |
| **turning_points** | [**Array&lt;TurningPoint&gt;**](TurningPoint.md) | Key moments that changed the match | [optional] |
| **weather_temp_celsius** | **Float** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::Match.new(
  attendance: null,
  away_score: null,
  away_team_id: manchester-city,
  date: null,
  episode_id: null,
  home_score: null,
  home_team_id: afc-richmond,
  id: match-001,
  lesson_learned: null,
  match_type: null,
  possession_percentage: null,
  result: null,
  ted_halftime_speech: null,
  ticket_revenue_gbp: null,
  turning_points: null,
  weather_temp_celsius: null
)
```

