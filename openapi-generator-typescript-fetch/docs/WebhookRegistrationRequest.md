
# WebhookRegistrationRequest

Request to register a new webhook endpoint.

## Properties

Name | Type
------------ | -------------
`description` | string
`eventTypes` | Array&lt;string&gt;
`url` | string

## Example

```typescript
import type { WebhookRegistrationRequest } from ''

// TODO: Update the object below with actual values
const example = {
  "description": null,
  "eventTypes": null,
  "url": null,
} satisfies WebhookRegistrationRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebhookRegistrationRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


