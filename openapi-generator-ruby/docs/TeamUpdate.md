# OpenapiClient::TeamUpdate

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **annual_budget_gbp** | [**AnnualBudgetGbp1**](AnnualBudgetGbp1.md) |  | [optional] |
| **average_attendance** | **Float** |  | [optional] |
| **contact_email** | **String** |  | [optional] |
| **culture_score** | **Integer** |  | [optional] |
| **founded_year** | **Integer** |  | [optional] |
| **is_active** | **Boolean** |  | [optional] |
| **league** | [**League**](League.md) |  | [optional] |
| **name** | **String** |  | [optional] |
| **nickname** | **String** |  | [optional] |
| **primary_color** | **String** |  | [optional] |
| **rival_teams** | **Array&lt;String&gt;** |  | [optional] |
| **secondary_color** | **String** |  | [optional] |
| **stadium** | **String** |  | [optional] |
| **stadium_location** | [**GeoLocation**](GeoLocation.md) |  | [optional] |
| **values** | [**TeamValues**](TeamValues.md) |  | [optional] |
| **website** | **String** |  | [optional] |
| **win_percentage** | **Float** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TeamUpdate.new(
  annual_budget_gbp: null,
  average_attendance: null,
  contact_email: null,
  culture_score: null,
  founded_year: null,
  is_active: null,
  league: null,
  name: null,
  nickname: null,
  primary_color: null,
  rival_teams: null,
  secondary_color: null,
  stadium: null,
  stadium_location: null,
  values: null,
  website: null,
  win_percentage: null
)
```

