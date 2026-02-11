
# PaginatedResponseEpisode


## Properties

Name | Type
------------ | -------------
`data` | [Array&lt;Episode&gt;](Episode.md)
`hasMore` | boolean
`limit` | number
`page` | number
`pages` | number
`skip` | number
`total` | number

## Example

```typescript
import type { PaginatedResponseEpisode } from ''

// TODO: Update the object below with actual values
const example = {
  "data": null,
  "hasMore": null,
  "limit": null,
  "page": null,
  "pages": null,
  "skip": null,
  "total": null,
} satisfies PaginatedResponseEpisode

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PaginatedResponseEpisode
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


