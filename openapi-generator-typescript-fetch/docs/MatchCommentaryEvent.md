
# MatchCommentaryEvent

A single commentary event during a match stream.

## Properties

Name | Type
------------ | -------------
`commentary` | string
`crowdReaction` | string
`description` | string
`eventId` | number
`eventType` | string
`isFinal` | boolean
`minute` | number
`tedSidelineReaction` | string

## Example

```typescript
import type { MatchCommentaryEvent } from ''

// TODO: Update the object below with actual values
const example = {
  "commentary": null,
  "crowdReaction": null,
  "description": null,
  "eventId": null,
  "eventType": null,
  "isFinal": null,
  "minute": null,
  "tedSidelineReaction": null,
} satisfies MatchCommentaryEvent

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MatchCommentaryEvent
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


