
# ConflictRequest

Request for conflict resolution.

## Properties

Name | Type
------------ | -------------
`attemptsMade` | Array&lt;string&gt;
`conflictType` | [ConflictType](ConflictType.md)
`description` | string
`partiesInvolved` | Array&lt;string&gt;

## Example

```typescript
import type { ConflictRequest } from ''

// TODO: Update the object below with actual values
const example = {
  "attemptsMade": null,
  "conflictType": null,
  "description": Alex keeps taking credit for my ideas in meetings and I'm getting resentful.,
  "partiesInvolved": [Me, My teammate Alex],
} satisfies ConflictRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ConflictRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


