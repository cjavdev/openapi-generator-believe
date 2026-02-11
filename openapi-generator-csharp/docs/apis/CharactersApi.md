# Org.OpenAPITools.Api.CharactersApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CreateCharacterCharactersPost**](CharactersApi.md#createcharactercharacterspost) | **POST** /characters | Create a new character |
| [**DeleteCharacterCharactersCharacterIdDelete**](CharactersApi.md#deletecharactercharacterscharacteriddelete) | **DELETE** /characters/{character_id} | Delete a character |
| [**GetCharacterCharactersCharacterIdGet**](CharactersApi.md#getcharactercharacterscharacteridget) | **GET** /characters/{character_id} | Get a character by ID |
| [**GetCharacterQuotesCharactersCharacterIdQuotesGet**](CharactersApi.md#getcharacterquotescharacterscharacteridquotesget) | **GET** /characters/{character_id}/quotes | Get character&#39;s signature quotes |
| [**ListCharactersCharactersGet**](CharactersApi.md#listcharacterscharactersget) | **GET** /characters | List all characters |
| [**UpdateCharacterCharactersCharacterIdPatch**](CharactersApi.md#updatecharactercharacterscharacteridpatch) | **PATCH** /characters/{character_id} | Update a character |

<a id="createcharactercharacterspost"></a>
# **CreateCharacterCharactersPost**
> Character CreateCharacterCharactersPost (CharacterCreate characterCreate)

Create a new character

Add a new character to the Ted Lasso universe.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **characterCreate** | [**CharacterCreate**](CharacterCreate.md) |  |  |

### Return type

[**Character**](Character.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Character created successfully |  -  |
| **409** | Character already exists |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="deletecharactercharacterscharacteriddelete"></a>
# **DeleteCharacterCharactersCharacterIdDelete**
> void DeleteCharacterCharactersCharacterIdDelete (string characterId)

Delete a character

Remove a character from the database.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **characterId** | **string** |  |  |

### Return type

void (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Character deleted successfully |  -  |
| **404** | Character not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getcharactercharacterscharacteridget"></a>
# **GetCharacterCharactersCharacterIdGet**
> Character GetCharacterCharactersCharacterIdGet (string characterId)

Get a character by ID

Retrieve detailed information about a specific character.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **characterId** | **string** |  |  |

### Return type

[**Character**](Character.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Character details |  -  |
| **404** | Character not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getcharacterquotescharacterscharacteridquotesget"></a>
# **GetCharacterQuotesCharactersCharacterIdQuotesGet**
> List&lt;string&gt; GetCharacterQuotesCharactersCharacterIdQuotesGet (string characterId)

Get character's signature quotes

Get all signature quotes from a specific character.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **characterId** | **string** |  |  |

### Return type

**List<string>**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of signature quotes |  -  |
| **404** | Character not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="listcharacterscharactersget"></a>
# **ListCharactersCharactersGet**
> PaginatedResponseCharacter ListCharactersCharactersGet (CharacterRole role = null, string teamId = null, int minOptimism = null, int skip = null, int limit = null)

List all characters

Get a paginated list of Ted Lasso characters.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **role** | **CharacterRole** | Filter by role | [optional]  |
| **teamId** | **string** | Filter by team ID | [optional]  |
| **minOptimism** | **int** | Minimum optimism score | [optional]  |
| **skip** | **int** | Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int** | Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseCharacter**](PaginatedResponseCharacter.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of characters |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="updatecharactercharacterscharacteridpatch"></a>
# **UpdateCharacterCharactersCharacterIdPatch**
> Character UpdateCharacterCharactersCharacterIdPatch (string characterId, CharacterUpdate characterUpdate)

Update a character

Update specific fields of an existing character.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **characterId** | **string** |  |  |
| **characterUpdate** | [**CharacterUpdate**](CharacterUpdate.md) |  |  |

### Return type

[**Character**](Character.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Character updated successfully |  -  |
| **404** | Character not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

