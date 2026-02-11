# OpenapiClient::PaginatedResponseQuote

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **data** | [**Array&lt;Quote&gt;**](Quote.md) |  |  |
| **has_more** | **Boolean** | Whether there are more items after this page. | [readonly] |
| **limit** | **Integer** |  |  |
| **page** | **Integer** | Current page number (1-indexed, for display purposes). | [readonly] |
| **pages** | **Integer** | Total number of pages. | [readonly] |
| **skip** | **Integer** |  |  |
| **total** | **Integer** |  |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::PaginatedResponseQuote.new(
  data: null,
  has_more: null,
  limit: null,
  page: null,
  pages: null,
  skip: null,
  total: null
)
```

