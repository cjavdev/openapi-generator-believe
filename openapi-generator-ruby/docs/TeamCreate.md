# OpenapiClient::TeamCreate

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **annual_budget_gbp** | [**AnnualBudgetGbp**](AnnualBudgetGbp.md) |  | [optional] |
| **average_attendance** | **Float** |  | [optional] |
| **contact_email** | **String** |  | [optional] |
| **culture_score** | **Integer** | Team culture/morale score (0-100) |  |
| **founded_year** | **Integer** | Year the club was founded |  |
| **is_active** | **Boolean** | Whether the team is currently active | [optional][default to true] |
| **league** | [**League**](League.md) | Current league |  |
| **name** | **String** | Team name |  |
| **nickname** | **String** |  | [optional] |
| **primary_color** | **String** |  | [optional] |
| **rival_teams** | **Array&lt;String&gt;** | List of rival team IDs | [optional] |
| **secondary_color** | **String** |  | [optional] |
| **stadium** | **String** | Home stadium name |  |
| **stadium_location** | [**GeoLocation**](GeoLocation.md) |  | [optional] |
| **values** | [**TeamValues**](TeamValues.md) | Team&#39;s core values |  |
| **website** | **String** |  | [optional] |
| **win_percentage** | **Float** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TeamCreate.new(
  annual_budget_gbp: null,
  average_attendance: null,
  contact_email: null,
  culture_score: 85,
  founded_year: 1897,
  is_active: null,
  league: null,
  name: AFC Richmond,
  nickname: null,
  primary_color: null,
  rival_teams: [west-ham, rupert-fc],
  secondary_color: null,
  stadium: Nelson Road,
  stadium_location: null,
  values: null,
  website: null,
  win_percentage: null
)
```

