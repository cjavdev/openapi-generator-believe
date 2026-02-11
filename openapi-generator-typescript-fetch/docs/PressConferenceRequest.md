
# PressConferenceRequest

Request for press conference response.

## Properties

Name | Type
------------ | -------------
`hostile` | boolean
`question` | string
`topic` | string

## Example

```typescript
import type { PressConferenceRequest } from ''

// TODO: Update the object below with actual values
const example = {
  "hostile": null,
  "question": Ted, your team just lost 5-0. How do you explain this embarrassing defeat?,
  "topic": null,
} satisfies PressConferenceRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PressConferenceRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


