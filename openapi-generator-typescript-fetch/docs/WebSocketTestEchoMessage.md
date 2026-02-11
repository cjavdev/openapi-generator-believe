
# WebSocketTestEchoMessage

Echo response from the test WebSocket.

## Properties

Name | Type
------------ | -------------
`message` | string
`tedSays` | string
`type` | string

## Example

```typescript
import type { WebSocketTestEchoMessage } from ''

// TODO: Update the object below with actual values
const example = {
  "message": null,
  "tedSays": null,
  "type": null,
} satisfies WebSocketTestEchoMessage

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebSocketTestEchoMessage
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


