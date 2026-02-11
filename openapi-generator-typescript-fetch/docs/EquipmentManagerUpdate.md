
# EquipmentManagerUpdate

Update model for equipment managers.

## Properties

Name | Type
------------ | -------------
`isHeadKitman` | boolean
`responsibilities` | Array&lt;string&gt;
`teamId` | string
`yearsWithTeam` | number

## Example

```typescript
import type { EquipmentManagerUpdate } from ''

// TODO: Update the object below with actual values
const example = {
  "isHeadKitman": null,
  "responsibilities": null,
  "teamId": null,
  "yearsWithTeam": null,
} satisfies EquipmentManagerUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as EquipmentManagerUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


