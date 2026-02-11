
# Biscuit

A biscuit from Ted.

## Properties

Name | Type
------------ | -------------
`id` | string
`message` | string
`pairsWellWith` | string
`tedNote` | string
`type` | [BiscuitType](BiscuitType.md)
`warmthLevel` | number

## Example

```typescript
import type { Biscuit } from ''

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "message": null,
  "pairsWellWith": null,
  "tedNote": null,
  "type": null,
  "warmthLevel": null,
} satisfies Biscuit

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Biscuit
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


