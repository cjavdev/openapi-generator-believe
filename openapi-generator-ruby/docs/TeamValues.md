# OpenapiClient::TeamValues

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **primary_value** | **String** | The team&#39;s primary guiding value |  |
| **secondary_values** | **Array&lt;String&gt;** | Supporting values |  |
| **team_motto** | **String** | Team&#39;s motivational motto |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TeamValues.new(
  primary_value: Believe,
  secondary_values: [Family, Resilience, Joy],
  team_motto: Football is life!
)
```

