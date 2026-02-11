
# WebSocketErrorMessage

Error message for WebSocket communication.

## Properties

Name | Type
------------ | -------------
`code` | string
`message` | string
`type` | string

## Example

```typescript
import type { WebSocketErrorMessage } from ''

// TODO: Update the object below with actual values
const example = {
  "code": null,
  "message": null,
  "type": null,
} satisfies WebSocketErrorMessage

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebSocketErrorMessage
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


