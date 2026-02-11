# OpenapiClient::Episode

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **air_date** | **Date** | Original air date |  |
| **biscuits_with_boss_moment** | **String** |  | [optional] |
| **character_focus** | **Array&lt;String&gt;** | Characters with significant development |  |
| **director** | **String** | Episode director |  |
| **episode_number** | **Integer** | Episode number within season |  |
| **id** | **String** | Unique identifier (format: s##e##) |  |
| **main_theme** | **String** | Central theme of the episode |  |
| **memorable_moments** | **Array&lt;String&gt;** | Standout moments from the episode | [optional] |
| **runtime_minutes** | **Integer** | Episode runtime in minutes |  |
| **season** | **Integer** | Season number |  |
| **synopsis** | **String** | Brief plot synopsis |  |
| **ted_wisdom** | **String** | Key piece of Ted wisdom from the episode |  |
| **title** | **String** | Episode title |  |
| **us_viewers_millions** | **Float** |  | [optional] |
| **viewer_rating** | **Float** |  | [optional] |
| **writer** | **String** | Episode writer(s) |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::Episode.new(
  air_date: 2020-08-14,
  biscuits_with_boss_moment: null,
  character_focus: [ted-lasso, rebecca-welton],
  director: null,
  episode_number: null,
  id: s01e01,
  main_theme: Taking chances and believing in yourself,
  memorable_moments: [Ted&#39;s first press conference, The BELIEVE sign goes up],
  runtime_minutes: null,
  season: null,
  synopsis: American football coach Ted Lasso is hired to manage AFC Richmond, a struggling English Premier League team.,
  ted_wisdom: Taking on a challenge is a lot like riding a horse. If you&#39;re comfortable while you&#39;re doing it, you&#39;re probably doing it wrong.,
  title: Pilot,
  us_viewers_millions: null,
  viewer_rating: null,
  writer: null
)
```

