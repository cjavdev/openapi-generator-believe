
# WebSocketMatchStats

Current match statistics.

## Properties

Name | Type
------------ | -------------
`cornersAway` | number
`cornersHome` | number
`foulsAway` | number
`foulsHome` | number
`possessionAway` | number
`possessionHome` | number
`redCardsAway` | number
`redCardsHome` | number
`shotsAway` | number
`shotsHome` | number
`shotsOnTargetAway` | number
`shotsOnTargetHome` | number
`yellowCardsAway` | number
`yellowCardsHome` | number

## Example

```typescript
import type { WebSocketMatchStats } from ''

// TODO: Update the object below with actual values
const example = {
  "cornersAway": null,
  "cornersHome": null,
  "foulsAway": null,
  "foulsHome": null,
  "possessionAway": null,
  "possessionHome": null,
  "redCardsAway": null,
  "redCardsHome": null,
  "shotsAway": null,
  "shotsHome": null,
  "shotsOnTargetAway": null,
  "shotsOnTargetHome": null,
  "yellowCardsAway": null,
  "yellowCardsHome": null,
} satisfies WebSocketMatchStats

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebSocketMatchStats
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


