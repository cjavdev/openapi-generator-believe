
# PlayerUpdate

Update model for players.

## Properties

Name | Type
------------ | -------------
`assists` | number
`goalsScored` | number
`isCaptain` | boolean
`jerseyNumber` | number
`position` | [Position](Position.md)
`teamId` | string
`yearsWithTeam` | number

## Example

```typescript
import type { PlayerUpdate } from ''

// TODO: Update the object below with actual values
const example = {
  "assists": null,
  "goalsScored": null,
  "isCaptain": null,
  "jerseyNumber": null,
  "position": null,
  "teamId": null,
  "yearsWithTeam": null,
} satisfies PlayerUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PlayerUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


