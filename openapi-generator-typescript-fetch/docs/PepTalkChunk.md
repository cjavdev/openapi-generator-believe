
# PepTalkChunk

A chunk of a streaming pep talk from Ted.

## Properties

Name | Type
------------ | -------------
`chunkId` | number
`emotionalBeat` | string
`isFinal` | boolean
`text` | string

## Example

```typescript
import type { PepTalkChunk } from ''

// TODO: Update the object below with actual values
const example = {
  "chunkId": null,
  "emotionalBeat": null,
  "isFinal": null,
  "text": null,
} satisfies PepTalkChunk

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PepTalkChunk
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


