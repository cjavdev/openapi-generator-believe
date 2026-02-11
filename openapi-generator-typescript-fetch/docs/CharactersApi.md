# CharactersApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createCharacterCharactersPost**](CharactersApi.md#createcharactercharacterspost) | **POST** /characters | Create a new character |
| [**deleteCharacterCharactersCharacterIdDelete**](CharactersApi.md#deletecharactercharacterscharacteriddelete) | **DELETE** /characters/{character_id} | Delete a character |
| [**getCharacterCharactersCharacterIdGet**](CharactersApi.md#getcharactercharacterscharacteridget) | **GET** /characters/{character_id} | Get a character by ID |
| [**getCharacterQuotesCharactersCharacterIdQuotesGet**](CharactersApi.md#getcharacterquotescharacterscharacteridquotesget) | **GET** /characters/{character_id}/quotes | Get character\&#39;s signature quotes |
| [**listCharactersCharactersGet**](CharactersApi.md#listcharacterscharactersget) | **GET** /characters | List all characters |
| [**updateCharacterCharactersCharacterIdPatch**](CharactersApi.md#updatecharactercharacterscharacteridpatch) | **PATCH** /characters/{character_id} | Update a character |



## createCharacterCharactersPost

> Character createCharacterCharactersPost(characterCreate)

Create a new character

Add a new character to the Ted Lasso universe.

### Example

```ts
import {
  Configuration,
  CharactersApi,
} from '';
import type { CreateCharacterCharactersPostRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CharactersApi(config);

  const body = {
    // CharacterCreate
    characterCreate: ...,
  } satisfies CreateCharacterCharactersPostRequest;

  try {
    const data = await api.createCharacterCharactersPost(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **characterCreate** | [CharacterCreate](CharacterCreate.md) |  | |

### Return type

[**Character**](Character.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Character created successfully |  -  |
| **409** | Character already exists |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteCharacterCharactersCharacterIdDelete

> deleteCharacterCharactersCharacterIdDelete(characterId)

Delete a character

Remove a character from the database.

### Example

```ts
import {
  Configuration,
  CharactersApi,
} from '';
import type { DeleteCharacterCharactersCharacterIdDeleteRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CharactersApi(config);

  const body = {
    // string
    characterId: characterId_example,
  } satisfies DeleteCharacterCharactersCharacterIdDeleteRequest;

  try {
    const data = await api.deleteCharacterCharactersCharacterIdDelete(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **characterId** | `string` |  | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Character deleted successfully |  -  |
| **404** | Character not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getCharacterCharactersCharacterIdGet

> Character getCharacterCharactersCharacterIdGet(characterId)

Get a character by ID

Retrieve detailed information about a specific character.

### Example

```ts
import {
  Configuration,
  CharactersApi,
} from '';
import type { GetCharacterCharactersCharacterIdGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CharactersApi(config);

  const body = {
    // string
    characterId: characterId_example,
  } satisfies GetCharacterCharactersCharacterIdGetRequest;

  try {
    const data = await api.getCharacterCharactersCharacterIdGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **characterId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Character**](Character.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Character details |  -  |
| **404** | Character not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getCharacterQuotesCharactersCharacterIdQuotesGet

> Array&lt;string | null&gt; getCharacterQuotesCharactersCharacterIdQuotesGet(characterId)

Get character\&#39;s signature quotes

Get all signature quotes from a specific character.

### Example

```ts
import {
  Configuration,
  CharactersApi,
} from '';
import type { GetCharacterQuotesCharactersCharacterIdQuotesGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CharactersApi(config);

  const body = {
    // string
    characterId: characterId_example,
  } satisfies GetCharacterQuotesCharactersCharacterIdQuotesGetRequest;

  try {
    const data = await api.getCharacterQuotesCharactersCharacterIdQuotesGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **characterId** | `string` |  | [Defaults to `undefined`] |

### Return type

**Array<string | null>**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of signature quotes |  -  |
| **404** | Character not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listCharactersCharactersGet

> PaginatedResponseCharacter listCharactersCharactersGet(role, teamId, minOptimism, skip, limit)

List all characters

Get a paginated list of Ted Lasso characters.

### Example

```ts
import {
  Configuration,
  CharactersApi,
} from '';
import type { ListCharactersCharactersGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CharactersApi(config);

  const body = {
    // CharacterRole | Filter by role (optional)
    role: ...,
    // string | Filter by team ID (optional)
    teamId: teamId_example,
    // number | Minimum optimism score (optional)
    minOptimism: 56,
    // number | Number of items to skip (offset) (optional)
    skip: 56,
    // number | Maximum number of items to return (max: 100) (optional)
    limit: 56,
  } satisfies ListCharactersCharactersGetRequest;

  try {
    const data = await api.listCharactersCharactersGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **role** | `CharacterRole` | Filter by role | [Optional] [Defaults to `undefined`] [Enum: coach, player, owner, manager, staff, journalist, family, friend, fan, other] |
| **teamId** | `string` | Filter by team ID | [Optional] [Defaults to `undefined`] |
| **minOptimism** | `number` | Minimum optimism score | [Optional] [Defaults to `undefined`] |
| **skip** | `number` | Number of items to skip (offset) | [Optional] [Defaults to `0`] |
| **limit** | `number` | Maximum number of items to return (max: 100) | [Optional] [Defaults to `20`] |

### Return type

[**PaginatedResponseCharacter**](PaginatedResponseCharacter.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of characters |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateCharacterCharactersCharacterIdPatch

> Character updateCharacterCharactersCharacterIdPatch(characterId, characterUpdate)

Update a character

Update specific fields of an existing character.

### Example

```ts
import {
  Configuration,
  CharactersApi,
} from '';
import type { UpdateCharacterCharactersCharacterIdPatchRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CharactersApi(config);

  const body = {
    // string
    characterId: characterId_example,
    // CharacterUpdate
    characterUpdate: ...,
  } satisfies UpdateCharacterCharactersCharacterIdPatchRequest;

  try {
    const data = await api.updateCharacterCharactersCharacterIdPatch(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **characterId** | `string` |  | [Defaults to `undefined`] |
| **characterUpdate** | [CharacterUpdate](CharacterUpdate.md) |  | |

### Return type

[**Character**](Character.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Character updated successfully |  -  |
| **404** | Character not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

