
# WebSocketLiveMatchEvent

A live match event with full details.

## Properties

Name | Type
------------ | -------------
`addedTime` | number
`commentary` | string
`crowdReaction` | string
`description` | string
`eventId` | number
`eventType` | string
`minute` | number
`player` | [WebSocketPlayerInfo](WebSocketPlayerInfo.md)
`score` | [WebSocketMatchScore](WebSocketMatchScore.md)
`secondaryPlayer` | [WebSocketPlayerInfo](WebSocketPlayerInfo.md)
`stats` | [WebSocketMatchStats](WebSocketMatchStats.md)
`team` | string
`tedReaction` | string

## Example

```typescript
import type { WebSocketLiveMatchEvent } from ''

// TODO: Update the object below with actual values
const example = {
  "addedTime": null,
  "commentary": null,
  "crowdReaction": null,
  "description": null,
  "eventId": null,
  "eventType": null,
  "minute": null,
  "player": null,
  "score": null,
  "secondaryPlayer": null,
  "stats": null,
  "team": null,
  "tedReaction": null,
} satisfies WebSocketLiveMatchEvent

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebSocketLiveMatchEvent
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


