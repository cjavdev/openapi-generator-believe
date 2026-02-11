
# TriggerEventResponse

Response after triggering webhook events.

## Properties

Name | Type
------------ | -------------
`deliveries` | [Array&lt;WebhookDeliveryResult&gt;](WebhookDeliveryResult.md)
`eventId` | string
`eventType` | string
`successfulDeliveries` | number
`tedSays` | string
`totalWebhooks` | number

## Example

```typescript
import type { TriggerEventResponse } from ''

// TODO: Update the object below with actual values
const example = {
  "deliveries": null,
  "eventId": null,
  "eventType": null,
  "successfulDeliveries": null,
  "tedSays": null,
  "totalWebhooks": null,
} satisfies TriggerEventResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TriggerEventResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


