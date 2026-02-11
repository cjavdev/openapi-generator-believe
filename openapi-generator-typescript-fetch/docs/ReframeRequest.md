
# ReframeRequest

Request to reframe a negative thought.

## Properties

Name | Type
------------ | -------------
`negativeThought` | string
`recurring` | boolean

## Example

```typescript
import type { ReframeRequest } from ''

// TODO: Update the object below with actual values
const example = {
  "negativeThought": I'm not good enough for this job.,
  "recurring": null,
} satisfies ReframeRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReframeRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


