
# Episode

Full episode model with ID.

## Properties

Name | Type
------------ | -------------
`airDate` | Date
`biscuitsWithBossMoment` | string
`characterFocus` | Array&lt;string&gt;
`director` | string
`episodeNumber` | number
`id` | string
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
import type { Episode } from ''

// TODO: Update the object below with actual values
const example = {
  "airDate": 2020-08-14,
  "biscuitsWithBossMoment": null,
  "characterFocus": [ted-lasso, rebecca-welton],
  "director": null,
  "episodeNumber": null,
  "id": s01e01,
  "mainTheme": Taking chances and believing in yourself,
  "memorableMoments": [Ted's first press conference, The BELIEVE sign goes up],
  "runtimeMinutes": null,
  "season": null,
  "synopsis": American football coach Ted Lasso is hired to manage AFC Richmond, a struggling English Premier League team.,
  "tedWisdom": Taking on a challenge is a lot like riding a horse. If you're comfortable while you're doing it, you're probably doing it wrong.,
  "title": Pilot,
  "usViewersMillions": null,
  "viewerRating": null,
  "writer": null,
} satisfies Episode

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Episode
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


