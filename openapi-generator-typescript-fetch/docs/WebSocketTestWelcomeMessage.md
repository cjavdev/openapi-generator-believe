
# WebSocketTestWelcomeMessage

Welcome message sent when connecting to the test WebSocket.

## Properties

Name | Type
------------ | -------------
`message` | string
`tedSays` | string
`type` | string

## Example

```typescript
import type { WebSocketTestWelcomeMessage } from ''

// TODO: Update the object below with actual values
const example = {
  "message": null,
  "tedSays": null,
  "type": null,
} satisfies WebSocketTestWelcomeMessage

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebSocketTestWelcomeMessage
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


