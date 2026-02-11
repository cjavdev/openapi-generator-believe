
# ResponseUpdateTeamMemberTeamMembersMemberIdPatch


## Properties

Name | Type
------------ | -------------
`assists` | number
`characterId` | string
`goalsScored` | number
`id` | string
`isCaptain` | boolean
`jerseyNumber` | number
`memberType` | string
`position` | [Position](Position.md)
`teamId` | string
`yearsWithTeam` | number
`certifications` | Array&lt;string&gt;
`specialty` | [MedicalSpecialty](MedicalSpecialty.md)
`winRate` | number
`licenseNumber` | string
`qualifications` | Array&lt;string&gt;
`isHeadKitman` | boolean
`responsibilities` | Array&lt;string&gt;

## Example

```typescript
import type { ResponseUpdateTeamMemberTeamMembersMemberIdPatch } from ''

// TODO: Update the object below with actual values
const example = {
  "assists": 23,
  "characterId": jamie-tartt,
  "goalsScored": 47,
  "id": nate-kitman-richmond,
  "isCaptain": false,
  "jerseyNumber": 9,
  "memberType": null,
  "position": null,
  "teamId": afc-richmond,
  "yearsWithTeam": 3,
  "certifications": [UEFA Pro License, FA Level 4],
  "specialty": null,
  "winRate": null,
  "licenseNumber": null,
  "qualifications": [PhD Clinical Psychology, Sports Psychology Certification],
  "isHeadKitman": true,
  "responsibilities": [Kit preparation, Equipment maintenance],
} satisfies ResponseUpdateTeamMemberTeamMembersMemberIdPatch

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ResponseUpdateTeamMemberTeamMembersMemberIdPatch
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


