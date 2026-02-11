
# MatchCreate

Model for creating a new match.

## Properties

Name | Type
------------ | -------------
`attendance` | number
`awayScore` | number
`awayTeamId` | string
`date` | Date
`episodeId` | string
`homeScore` | number
`homeTeamId` | string
`lessonLearned` | string
`matchType` | [MatchType](MatchType.md)
`possessionPercentage` | number
`result` | [MatchResult](MatchResult.md)
`tedHalftimeSpeech` | string
`ticketRevenueGbp` | [TicketRevenueGbp](TicketRevenueGbp.md)
`turningPoints` | [Array&lt;TurningPoint&gt;](TurningPoint.md)
`weatherTempCelsius` | number

## Example

```typescript
import type { MatchCreate } from ''

// TODO: Update the object below with actual values
const example = {
  "attendance": null,
  "awayScore": null,
  "awayTeamId": manchester-city,
  "date": null,
  "episodeId": null,
  "homeScore": null,
  "homeTeamId": afc-richmond,
  "lessonLearned": null,
  "matchType": null,
  "possessionPercentage": null,
  "result": null,
  "tedHalftimeSpeech": null,
  "ticketRevenueGbp": null,
  "turningPoints": null,
  "weatherTempCelsius": null,
} satisfies MatchCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MatchCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


