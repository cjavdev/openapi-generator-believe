
# EquipmentManagerBase

Equipment and kit management staff.

## Properties

Name | Type
------------ | -------------
`characterId` | string
`isHeadKitman` | boolean
`memberType` | string
`responsibilities` | Array&lt;string&gt;
`teamId` | string
`yearsWithTeam` | number

## Example

```typescript
import type { EquipmentManagerBase } from ''

// TODO: Update the object below with actual values
const example = {
  "characterId": jamie-tartt,
  "isHeadKitman": true,
  "memberType": null,
  "responsibilities": [Kit preparation, Equipment maintenance],
  "teamId": afc-richmond,
  "yearsWithTeam": 3,
} satisfies EquipmentManagerBase

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as EquipmentManagerBase
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


