
# WebSocketClientMessage

Messages sent by the client to control the match simulation.

## Properties

Name | Type
------------ | -------------
`action` | string
`speed` | number

## Example

```typescript
import type { WebSocketClientMessage } from ''

// TODO: Update the object below with actual values
const example = {
  "action": null,
  "speed": null,
} satisfies WebSocketClientMessage

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebSocketClientMessage
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


