
# TeamUpdate

Model for updating a team (all fields optional).

## Properties

Name | Type
------------ | -------------
`annualBudgetGbp` | [AnnualBudgetGbp1](AnnualBudgetGbp1.md)
`averageAttendance` | number
`contactEmail` | string
`cultureScore` | number
`foundedYear` | number
`isActive` | boolean
`league` | [League](League.md)
`name` | string
`nickname` | string
`primaryColor` | string
`rivalTeams` | Array&lt;string&gt;
`secondaryColor` | string
`stadium` | string
`stadiumLocation` | [GeoLocation](GeoLocation.md)
`values` | [TeamValues](TeamValues.md)
`website` | string
`winPercentage` | number

## Example

```typescript
import type { TeamUpdate } from ''

// TODO: Update the object below with actual values
const example = {
  "annualBudgetGbp": null,
  "averageAttendance": null,
  "contactEmail": null,
  "cultureScore": null,
  "foundedYear": null,
  "isActive": null,
  "league": null,
  "name": null,
  "nickname": null,
  "primaryColor": null,
  "rivalTeams": null,
  "secondaryColor": null,
  "stadium": null,
  "stadiumLocation": null,
  "values": null,
  "website": null,
  "winPercentage": null,
} satisfies TeamUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TeamUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


