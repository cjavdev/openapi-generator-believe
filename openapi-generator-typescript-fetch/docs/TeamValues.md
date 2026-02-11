
# TeamValues

Core values that define a team\'s culture.

## Properties

Name | Type
------------ | -------------
`primaryValue` | string
`secondaryValues` | Array&lt;string&gt;
`teamMotto` | string

## Example

```typescript
import type { TeamValues } from ''

// TODO: Update the object below with actual values
const example = {
  "primaryValue": Believe,
  "secondaryValues": [Family, Resilience, Joy],
  "teamMotto": Football is life!,
} satisfies TeamValues

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TeamValues
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


