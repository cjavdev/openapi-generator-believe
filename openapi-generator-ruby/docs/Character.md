# OpenapiClient::Character

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **background** | **String** | Character background and history |  |
| **date_of_birth** | **Date** |  | [optional] |
| **email** | **String** |  | [optional] |
| **emotional_stats** | [**EmotionalStats**](EmotionalStats.md) | Emotional intelligence stats |  |
| **growth_arcs** | [**Array&lt;GrowthArc&gt;**](GrowthArc.md) | Character development across seasons | [optional] |
| **height_meters** | **Float** |  | [optional] |
| **id** | **String** | Unique identifier |  |
| **name** | **String** | Character&#39;s full name |  |
| **personality_traits** | **Array&lt;String&gt;** | Key personality traits |  |
| **profile_image_url** | **String** |  | [optional] |
| **role** | [**CharacterRole**](CharacterRole.md) | Character&#39;s role |  |
| **salary_gbp** | **String** |  | [optional] |
| **signature_quotes** | **Array&lt;String&gt;** | Memorable quotes from this character | [optional] |
| **team_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::Character.new(
  background: Former American football coach from Kansas who moved to London to coach AFC Richmond,
  date_of_birth: null,
  email: null,
  emotional_stats: null,
  growth_arcs: null,
  height_meters: null,
  id: ted-lasso,
  name: Ted Lasso,
  personality_traits: [optimistic, kind, folksy, persistent],
  profile_image_url: null,
  role: null,
  salary_gbp: null,
  signature_quotes: [I believe in believe., Be curious, not judgmental.],
  team_id: null
)
```

