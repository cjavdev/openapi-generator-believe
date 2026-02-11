
# CharacterUpdate

Model for updating a character (all fields optional).

## Properties

Name | Type
------------ | -------------
`background` | string
`dateOfBirth` | Date
`email` | string
`emotionalStats` | [EmotionalStats](EmotionalStats.md)
`growthArcs` | [Array&lt;GrowthArc&gt;](GrowthArc.md)
`heightMeters` | number
`name` | string
`personalityTraits` | Array&lt;string&gt;
`profileImageUrl` | string
`role` | [CharacterRole](CharacterRole.md)
`salaryGbp` | [SalaryGbp1](SalaryGbp1.md)
`signatureQuotes` | Array&lt;string&gt;
`teamId` | string

## Example

```typescript
import type { CharacterUpdate } from ''

// TODO: Update the object below with actual values
const example = {
  "background": null,
  "dateOfBirth": null,
  "email": null,
  "emotionalStats": null,
  "growthArcs": null,
  "heightMeters": null,
  "name": null,
  "personalityTraits": null,
  "profileImageUrl": null,
  "role": null,
  "salaryGbp": null,
  "signatureQuotes": null,
  "teamId": null,
} satisfies CharacterUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CharacterUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


