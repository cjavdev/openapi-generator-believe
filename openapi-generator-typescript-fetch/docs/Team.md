
# Team

Full team model with ID.

## Properties

Name | Type
------------ | -------------
`annualBudgetGbp` | string
`averageAttendance` | number
`contactEmail` | string
`cultureScore` | number
`foundedYear` | number
`id` | string
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
import type { Team } from ''

// TODO: Update the object below with actual values
const example = {
  "annualBudgetGbp": null,
  "averageAttendance": null,
  "contactEmail": null,
  "cultureScore": 85,
  "foundedYear": 1897,
  "id": afc-richmond,
  "isActive": null,
  "league": null,
  "name": AFC Richmond,
  "nickname": null,
  "primaryColor": null,
  "rivalTeams": [west-ham, rupert-fc],
  "secondaryColor": null,
  "stadium": Nelson Road,
  "stadiumLocation": null,
  "values": null,
  "website": null,
  "winPercentage": null,
} satisfies Team

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Team
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


