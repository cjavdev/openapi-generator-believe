
# WebSocketPlayerInfo

Information about a player involved in an event.

## Properties

Name | Type
------------ | -------------
`name` | string
`number` | number
`position` | string

## Example

```typescript
import type { WebSocketPlayerInfo } from ''

// TODO: Update the object below with actual values
const example = {
  "name": null,
  "number": null,
  "position": null,
} satisfies WebSocketPlayerInfo

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebSocketPlayerInfo
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


