
# MedicalStaffBase

Medical and wellness staff member.

## Properties

Name | Type
------------ | -------------
`characterId` | string
`licenseNumber` | string
`memberType` | string
`qualifications` | Array&lt;string&gt;
`specialty` | [MedicalSpecialty](MedicalSpecialty.md)
`teamId` | string
`yearsWithTeam` | number

## Example

```typescript
import type { MedicalStaffBase } from ''

// TODO: Update the object below with actual values
const example = {
  "characterId": jamie-tartt,
  "licenseNumber": null,
  "memberType": null,
  "qualifications": [PhD Clinical Psychology, Sports Psychology Certification],
  "specialty": null,
  "teamId": afc-richmond,
  "yearsWithTeam": 3,
} satisfies MedicalStaffBase

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MedicalStaffBase
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


