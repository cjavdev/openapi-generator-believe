# OpenapiClient::CharacterUpdate

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **background** | **String** |  | [optional] |
| **date_of_birth** | **Date** |  | [optional] |
| **email** | **String** |  | [optional] |
| **emotional_stats** | [**EmotionalStats**](EmotionalStats.md) |  | [optional] |
| **growth_arcs** | [**Array&lt;GrowthArc&gt;**](GrowthArc.md) |  | [optional] |
| **height_meters** | **Float** |  | [optional] |
| **name** | **String** |  | [optional] |
| **personality_traits** | **Array&lt;String&gt;** |  | [optional] |
| **profile_image_url** | **String** |  | [optional] |
| **role** | [**CharacterRole**](CharacterRole.md) |  | [optional] |
| **salary_gbp** | [**SalaryGbp1**](SalaryGbp1.md) |  | [optional] |
| **signature_quotes** | **Array&lt;String&gt;** |  | [optional] |
| **team_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::CharacterUpdate.new(
  background: null,
  date_of_birth: null,
  email: null,
  emotional_stats: null,
  growth_arcs: null,
  height_meters: null,
  name: null,
  personality_traits: null,
  profile_image_url: null,
  role: null,
  salary_gbp: null,
  signature_quotes: null,
  team_id: null
)
```

