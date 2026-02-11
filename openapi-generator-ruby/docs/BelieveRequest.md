# OpenapiClient::BelieveRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **context** | **String** |  | [optional] |
| **intensity** | **Integer** | How intense is the response needed (1&#x3D;gentle, 10&#x3D;full Ted) | [optional][default to 5] |
| **situation** | **String** | Describe your situation |  |
| **situation_type** | [**SituationType**](SituationType.md) | Type of situation |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::BelieveRequest.new(
  context: null,
  intensity: null,
  situation: I just got passed over for a promotion I&#39;ve been working toward for two years.,
  situation_type: null
)
```

