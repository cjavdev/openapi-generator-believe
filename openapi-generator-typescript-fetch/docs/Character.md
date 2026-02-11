
# Character

Full character model with ID.

## Properties

Name | Type
------------ | -------------
`background` | string
`dateOfBirth` | Date
`email` | string
`emotionalStats` | [EmotionalStats](EmotionalStats.md)
`growthArcs` | [Array&lt;GrowthArc&gt;](GrowthArc.md)
`heightMeters` | number
`id` | string
`name` | string
`personalityTraits` | Array&lt;string&gt;
`profileImageUrl` | string
`role` | [CharacterRole](CharacterRole.md)
`salaryGbp` | string
`signatureQuotes` | Array&lt;string&gt;
`teamId` | string

## Example

```typescript
import type { Character } from ''

// TODO: Update the object below with actual values
const example = {
  "background": Former American football coach from Kansas who moved to London to coach AFC Richmond,
  "dateOfBirth": null,
  "email": null,
  "emotionalStats": null,
  "growthArcs": null,
  "heightMeters": null,
  "id": ted-lasso,
  "name": Ted Lasso,
  "personalityTraits": [optimistic, kind, folksy, persistent],
  "profileImageUrl": null,
  "role": null,
  "salaryGbp": null,
  "signatureQuotes": [I believe in believe., Be curious, not judgmental.],
  "teamId": null,
} satisfies Character

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Character
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


