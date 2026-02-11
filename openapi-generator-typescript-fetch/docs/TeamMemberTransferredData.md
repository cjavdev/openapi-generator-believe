
# TeamMemberTransferredData

Data payload for a team member transfer event.

## Properties

Name | Type
------------ | -------------
`characterId` | string
`characterName` | string
`memberType` | string
`previousTeamId` | string
`previousTeamName` | string
`teamId` | string
`teamMemberId` | string
`teamName` | string
`tedReaction` | string
`transferFeeGbp` | string
`transferType` | string
`yearsWithPreviousTeam` | number

## Example

```typescript
import type { TeamMemberTransferredData } from ''

// TODO: Update the object below with actual values
const example = {
  "characterId": null,
  "characterName": null,
  "memberType": null,
  "previousTeamId": null,
  "previousTeamName": null,
  "teamId": null,
  "teamMemberId": null,
  "teamName": null,
  "tedReaction": null,
  "transferFeeGbp": null,
  "transferType": null,
  "yearsWithPreviousTeam": null,
} satisfies TeamMemberTransferredData

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TeamMemberTransferredData
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


