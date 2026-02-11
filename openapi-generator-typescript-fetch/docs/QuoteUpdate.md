
# QuoteUpdate

Model for updating a quote (all fields optional).

## Properties

Name | Type
------------ | -------------
`characterId` | string
`context` | string
`episodeId` | string
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
import type { QuoteUpdate } from ''

// TODO: Update the object below with actual values
const example = {
  "characterId": null,
  "context": null,
  "episodeId": null,
  "isFunny": null,
  "isInspirational": null,
  "momentType": null,
  "popularityScore": null,
  "secondaryThemes": null,
  "text": null,
  "theme": null,
  "timesShared": null,
} satisfies QuoteUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as QuoteUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


