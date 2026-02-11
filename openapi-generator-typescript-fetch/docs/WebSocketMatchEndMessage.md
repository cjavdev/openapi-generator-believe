
# WebSocketMatchEndMessage

Message sent when a match simulation ends.

## Properties

Name | Type
------------ | -------------
`finalScore` | [WebSocketMatchScore](WebSocketMatchScore.md)
`finalStats` | [WebSocketMatchStats](WebSocketMatchStats.md)
`manOfTheMatch` | string
`matchId` | string
`tedPostMatch` | string
`type` | string

## Example

```typescript
import type { WebSocketMatchEndMessage } from ''

// TODO: Update the object below with actual values
const example = {
  "finalScore": null,
  "finalStats": null,
  "manOfTheMatch": null,
  "matchId": null,
  "tedPostMatch": null,
  "type": null,
} satisfies WebSocketMatchEndMessage

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebSocketMatchEndMessage
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


