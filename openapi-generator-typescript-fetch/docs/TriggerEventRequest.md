
# TriggerEventRequest

Request to trigger a webhook event.

## Properties

Name | Type
------------ | -------------
`eventType` | string
`payload` | [TriggerEventRequestPayload](TriggerEventRequestPayload.md)

## Example

```typescript
import type { TriggerEventRequest } from ''

// TODO: Update the object below with actual values
const example = {
  "eventType": null,
  "payload": null,
} satisfies TriggerEventRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TriggerEventRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


