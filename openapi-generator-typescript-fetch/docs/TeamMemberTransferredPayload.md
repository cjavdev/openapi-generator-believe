
# TeamMemberTransferredPayload

Payload for team_member.transferred event.

## Properties

Name | Type
------------ | -------------
`data` | [TeamMemberTransferredData](TeamMemberTransferredData.md)
`eventType` | string

## Example

```typescript
import type { TeamMemberTransferredPayload } from ''

// TODO: Update the object below with actual values
const example = {
  "data": null,
  "eventType": null,
} satisfies TeamMemberTransferredPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TeamMemberTransferredPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


