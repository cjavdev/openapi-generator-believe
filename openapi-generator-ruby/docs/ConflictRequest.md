# OpenapiClient::ConflictRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **attempts_made** | **Array&lt;String&gt;** |  | [optional] |
| **conflict_type** | [**ConflictType**](ConflictType.md) | Type of conflict |  |
| **description** | **String** | Describe the conflict |  |
| **parties_involved** | **Array&lt;String&gt;** | Who is involved in the conflict |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ConflictRequest.new(
  attempts_made: null,
  conflict_type: null,
  description: Alex keeps taking credit for my ideas in meetings and I&#39;m getting resentful.,
  parties_involved: [Me, My teammate Alex]
)
```

