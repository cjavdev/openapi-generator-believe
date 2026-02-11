# OpenapiClient::MatchUpdate

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **attendance** | **Integer** |  | [optional] |
| **away_score** | **Integer** |  | [optional] |
| **away_team_id** | **String** |  | [optional] |
| **date** | **Time** |  | [optional] |
| **episode_id** | **String** |  | [optional] |
| **home_score** | **Integer** |  | [optional] |
| **home_team_id** | **String** |  | [optional] |
| **lesson_learned** | **String** |  | [optional] |
| **match_type** | [**MatchType**](MatchType.md) |  | [optional] |
| **possession_percentage** | **Float** |  | [optional] |
| **result** | [**MatchResult**](MatchResult.md) |  | [optional] |
| **ted_halftime_speech** | **String** |  | [optional] |
| **ticket_revenue_gbp** | [**TicketRevenueGbp1**](TicketRevenueGbp1.md) |  | [optional] |
| **turning_points** | [**Array&lt;TurningPoint&gt;**](TurningPoint.md) |  | [optional] |
| **weather_temp_celsius** | **Float** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::MatchUpdate.new(
  attendance: null,
  away_score: null,
  away_team_id: null,
  date: null,
  episode_id: null,
  home_score: null,
  home_team_id: null,
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

