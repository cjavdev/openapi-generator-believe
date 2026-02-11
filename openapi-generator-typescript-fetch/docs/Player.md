
# Player

Full player model with ID.

## Properties

Name | Type
------------ | -------------
`assists` | number
`characterId` | string
`goalsScored` | number
`id` | string
`isCaptain` | boolean
`jerseyNumber` | number
`memberType` | string
`position` | [Position](Position.md)
`teamId` | string
`yearsWithTeam` | number

## Example

```typescript
import type { Player } from ''

// TODO: Update the object below with actual values
const example = {
  "assists": 23,
  "characterId": jamie-tartt,
  "goalsScored": 47,
  "id": jamie-tartt-richmond,
  "isCaptain": false,
  "jerseyNumber": 9,
  "memberType": null,
  "position": null,
  "teamId": afc-richmond,
  "yearsWithTeam": 3,
} satisfies Player

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Player
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


