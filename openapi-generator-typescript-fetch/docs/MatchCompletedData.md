
# MatchCompletedData

Data payload for a match completed event.

## Properties

Name | Type
------------ | -------------
`awayScore` | number
`awayTeamId` | string
`completedAt` | Date
`homeScore` | number
`homeTeamId` | string
`lessonLearned` | string
`manOfTheMatch` | string
`matchId` | string
`matchType` | string
`result` | string
`tedPostMatchQuote` | string

## Example

```typescript
import type { MatchCompletedData } from ''

// TODO: Update the object below with actual values
const example = {
  "awayScore": null,
  "awayTeamId": null,
  "completedAt": null,
  "homeScore": null,
  "homeTeamId": null,
  "lessonLearned": null,
  "manOfTheMatch": null,
  "matchId": null,
  "matchType": null,
  "result": null,
  "tedPostMatchQuote": null,
} satisfies MatchCompletedData

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MatchCompletedData
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


