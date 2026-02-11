
# Quote

Full quote model with ID.

## Properties

Name | Type
------------ | -------------
`characterId` | string
`context` | string
`episodeId` | string
`id` | string
`isFunny` | boolean
`isInspirational` | boolean
`momentType` | [QuoteMoment](QuoteMoment.md)
`popularityScore` | number
`secondaryThemes` | [Array&lt;QuoteTheme&gt;](QuoteTheme.md)
`text` | string
`theme` | [QuoteTheme](QuoteTheme.md)
`timesShared` | number

## Example

```typescript
import type { Quote } from ''

// TODO: Update the object below with actual values
const example = {
  "characterId": ted-lasso,
  "context": Ted playing darts against Rupert in the pub, explaining his philosophy,
  "episodeId": null,
  "id": quote-001,
  "isFunny": null,
  "isInspirational": null,
  "momentType": null,
  "popularityScore": null,
  "secondaryThemes": [wisdom, kindness],
  "text": Be curious, not judgmental.,
  "theme": null,
  "timesShared": null,
} satisfies Quote

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Quote
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


