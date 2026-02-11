
# FileUploadResponse

Response model for file uploads.

## Properties

Name | Type
------------ | -------------
`checksumSha256` | string
`contentType` | string
`fileId` | string
`filename` | string
`sizeBytes` | number
`uploadedAt` | Date

## Example

```typescript
import type { FileUploadResponse } from ''

// TODO: Update the object below with actual values
const example = {
  "checksumSha256": null,
  "contentType": null,
  "fileId": null,
  "filename": null,
  "sizeBytes": null,
  "uploadedAt": null,
} satisfies FileUploadResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as FileUploadResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


