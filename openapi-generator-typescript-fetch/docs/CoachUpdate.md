
# CoachUpdate

Update model for coaches.

## Properties

Name | Type
------------ | -------------
`certifications` | Array&lt;string&gt;
`specialty` | [CoachSpecialty](CoachSpecialty.md)
`teamId` | string
`winRate` | number
`yearsWithTeam` | number

## Example

```typescript
import type { CoachUpdate } from ''

// TODO: Update the object below with actual values
const example = {
  "certifications": null,
  "specialty": null,
  "teamId": null,
  "winRate": null,
  "yearsWithTeam": null,
} satisfies CoachUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CoachUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


