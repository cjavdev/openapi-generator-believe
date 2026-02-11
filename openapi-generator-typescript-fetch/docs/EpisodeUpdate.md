
# EpisodeUpdate

Model for updating an episode (all fields optional).

## Properties

Name | Type
------------ | -------------
`airDate` | Date
`biscuitsWithBossMoment` | string
`characterFocus` | Array&lt;string&gt;
`director` | string
`episodeNumber` | number
`mainTheme` | string
`memorableMoments` | Array&lt;string&gt;
`runtimeMinutes` | number
`season` | number
`synopsis` | string
`tedWisdom` | string
`title` | string
`usViewersMillions` | number
`viewerRating` | number
`writer` | string

## Example

```typescript
import type { EpisodeUpdate } from ''

// TODO: Update the object below with actual values
const example = {
  "airDate": null,
  "biscuitsWithBossMoment": null,
  "characterFocus": null,
  "director": null,
  "episodeNumber": null,
  "mainTheme": null,
  "memorableMoments": null,
  "runtimeMinutes": null,
  "season": null,
  "synopsis": null,
  "tedWisdom": null,
  "title": null,
  "usViewersMillions": null,
  "viewerRating": null,
  "writer": null,
} satisfies EpisodeUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as EpisodeUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


