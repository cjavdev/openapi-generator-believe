
# BelieveRequest

Request for the Believe Engine.

## Properties

Name | Type
------------ | -------------
`context` | string
`intensity` | number
`situation` | string
`situationType` | [SituationType](SituationType.md)

## Example

```typescript
import type { BelieveRequest } from ''

// TODO: Update the object below with actual values
const example = {
  "context": null,
  "intensity": null,
  "situation": I just got passed over for a promotion I've been working toward for two years.,
  "situationType": null,
} satisfies BelieveRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BelieveRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


