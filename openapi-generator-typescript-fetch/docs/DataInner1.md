
# DataInner1


## Properties

Name | Type
------------ | -------------
`characterId` | string
`id` | string
`licenseNumber` | string
`memberType` | string
`qualifications` | Array&lt;string&gt;
`specialty` | [MedicalSpecialty](MedicalSpecialty.md)
`teamId` | string
`yearsWithTeam` | number
`isHeadKitman` | boolean
`responsibilities` | Array&lt;string&gt;

## Example

```typescript
import type { DataInner1 } from ''

// TODO: Update the object below with actual values
const example = {
  "characterId": jamie-tartt,
  "id": nate-kitman-richmond,
  "licenseNumber": null,
  "memberType": null,
  "qualifications": [PhD Clinical Psychology, Sports Psychology Certification],
  "specialty": null,
  "teamId": afc-richmond,
  "yearsWithTeam": 3,
  "isHeadKitman": true,
  "responsibilities": [Kit preparation, Equipment maintenance],
} satisfies DataInner1

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DataInner1
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


