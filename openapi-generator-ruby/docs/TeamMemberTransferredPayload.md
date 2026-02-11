# OpenapiClient::TeamMemberTransferredPayload

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **data** | [**TeamMemberTransferredData**](TeamMemberTransferredData.md) | Event data |  |
| **event_type** | **String** | The type of webhook event | [optional][default to &#39;team_member.transferred&#39;] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TeamMemberTransferredPayload.new(
  data: null,
  event_type: null
)
```

