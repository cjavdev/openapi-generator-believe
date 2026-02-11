# OpenapiClient::MatchCompletedData

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **away_score** | **Integer** | Final away team score |  |
| **away_team_id** | **String** | Away team ID |  |
| **completed_at** | **Time** | When the match completed |  |
| **home_score** | **Integer** | Final home team score |  |
| **home_team_id** | **String** | Home team ID |  |
| **lesson_learned** | **String** | Ted&#39;s lesson from the match | [optional] |
| **man_of_the_match** | **String** | Player of the match (if awarded) | [optional] |
| **match_id** | **String** | Unique match identifier |  |
| **match_type** | **String** | Type of match |  |
| **result** | **String** | Match result from home team perspective |  |
| **ted_post_match_quote** | **String** | Ted&#39;s post-match wisdom |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::MatchCompletedData.new(
  away_score: null,
  away_team_id: null,
  completed_at: null,
  home_score: null,
  home_team_id: null,
  lesson_learned: null,
  man_of_the_match: null,
  match_id: null,
  match_type: null,
  result: null,
  ted_post_match_quote: null
)
```

