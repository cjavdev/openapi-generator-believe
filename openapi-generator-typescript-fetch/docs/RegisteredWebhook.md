
# RegisteredWebhook

A registered webhook endpoint.

## Properties

Name | Type
------------ | -------------
`createdAt` | Date
`description` | string
`eventTypes` | Array&lt;string&gt;
`id` | string
`secret` | string
`url` | string

## Example

```typescript
import type { RegisteredWebhook } from ''

// TODO: Update the object below with actual values
const example = {
  "createdAt": null,
  "description": null,
  "eventTypes": null,
  "id": null,
  "secret": null,
  "url": null,
} satisfies RegisteredWebhook

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RegisteredWebhook
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


