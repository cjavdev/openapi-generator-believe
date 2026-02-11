
# WebSocketServerMessage

Messages sent by the server during live match simulation.

## Properties

Name | Type
------------ | -------------
`awayTeam` | string
`homeTeam` | string
`matchId` | string
`message` | string
`type` | string
`event` | [WebSocketLiveMatchEvent](WebSocketLiveMatchEvent.md)
`finalScore` | [WebSocketMatchScore](WebSocketMatchScore.md)
`finalStats` | [WebSocketMatchStats](WebSocketMatchStats.md)
`manOfTheMatch` | string
`tedPostMatch` | string
`code` | string

## Example

```typescript
import type { WebSocketServerMessage } from ''

// TODO: Update the object below with actual values
const example = {
  "awayTeam": null,
  "homeTeam": null,
  "matchId": null,
  "message": null,
  "type": null,
  "event": null,
  "finalScore": null,
  "finalStats": null,
  "manOfTheMatch": null,
  "tedPostMatch": null,
  "code": null,
} satisfies WebSocketServerMessage

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebSocketServerMessage
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


