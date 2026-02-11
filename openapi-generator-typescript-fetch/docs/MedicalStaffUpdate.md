
# MedicalStaffUpdate

Update model for medical staff.

## Properties

Name | Type
------------ | -------------
`licenseNumber` | string
`qualifications` | Array&lt;string&gt;
`specialty` | [MedicalSpecialty](MedicalSpecialty.md)
`teamId` | string
`yearsWithTeam` | number

## Example

```typescript
import type { MedicalStaffUpdate } from ''

// TODO: Update the object below with actual values
const example = {
  "licenseNumber": null,
  "qualifications": null,
  "specialty": null,
  "teamId": null,
  "yearsWithTeam": null,
} satisfies MedicalStaffUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MedicalStaffUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


