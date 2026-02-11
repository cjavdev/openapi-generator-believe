
# EquipmentManager

Full equipment manager model with ID.

## Properties

Name | Type
------------ | -------------
`characterId` | string
`id` | string
`isHeadKitman` | boolean
`memberType` | string
`responsibilities` | Array&lt;string&gt;
`teamId` | string
`yearsWithTeam` | number

## Example

```typescript
import type { EquipmentManager } from ''

// TODO: Update the object below with actual values
const example = {
  "characterId": jamie-tartt,
  "id": nate-kitman-richmond,
  "isHeadKitman": true,
  "memberType": null,
  "responsibilities": [Kit preparation, Equipment maintenance],
  "teamId": afc-richmond,
  "yearsWithTeam": 3,
} satisfies EquipmentManager

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as EquipmentManager
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


