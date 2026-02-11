
# WebSocketMatchStartMessage

Message sent when a match simulation starts.

## Properties

Name | Type
------------ | -------------
`awayTeam` | string
`homeTeam` | string
`matchId` | string
`message` | string
`type` | string

## Example

```typescript
import type { WebSocketMatchStartMessage } from ''

// TODO: Update the object below with actual values
const example = {
  "awayTeam": null,
  "homeTeam": null,
  "matchId": null,
  "message": null,
  "type": null,
} satisfies WebSocketMatchStartMessage

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebSocketMatchStartMessage
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


