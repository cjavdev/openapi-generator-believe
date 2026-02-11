
# TeamMemberTransferredEvent

Webhook event sent when a team member (player, coach, staff) transfers between teams.

## Properties

Name | Type
------------ | -------------
`createdAt` | Date
`data` | [TeamMemberTransferredData](TeamMemberTransferredData.md)
`eventId` | string
`eventType` | string

## Example

```typescript
import type { TeamMemberTransferredEvent } from ''

// TODO: Update the object below with actual values
const example = {
  "createdAt": null,
  "data": null,
  "eventId": null,
  "eventType": null,
} satisfies TeamMemberTransferredEvent

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TeamMemberTransferredEvent
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


