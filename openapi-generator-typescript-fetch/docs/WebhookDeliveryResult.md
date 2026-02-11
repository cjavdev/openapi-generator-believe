
# WebhookDeliveryResult

Result of delivering a webhook to a single endpoint.

## Properties

Name | Type
------------ | -------------
`error` | string
`statusCode` | number
`success` | boolean
`url` | string
`webhookId` | string

## Example

```typescript
import type { WebhookDeliveryResult } from ''

// TODO: Update the object below with actual values
const example = {
  "error": null,
  "statusCode": null,
  "success": null,
  "url": null,
  "webhookId": null,
} satisfies WebhookDeliveryResult

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookDeliveryResult
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


