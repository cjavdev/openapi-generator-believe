# InteractiveApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**believeEngineBelievePost**](InteractiveApi.md#believeenginebelievepost) | **POST** /believe | The Believe Engine |
| [**getBiscuitBiscuitsBiscuitIdGet**](InteractiveApi.md#getbiscuitbiscuitsbiscuitidget) | **GET** /biscuits/{biscuit_id} | Get a Specific Biscuit |
| [**getBiscuitsBiscuitsGet**](InteractiveApi.md#getbiscuitsbiscuitsget) | **GET** /biscuits | Biscuits as a Service |
| [**getCoachingPrincipleCoachingPrinciplesPrincipleIdGet**](InteractiveApi.md#getcoachingprinciplecoachingprinciplesprincipleidget) | **GET** /coaching/principles/{principle_id} | Get a Specific Coaching Principle |
| [**getCoachingPrinciplesCoachingPrinciplesGet**](InteractiveApi.md#getcoachingprinciplescoachingprinciplesget) | **GET** /coaching/principles | Get Coaching Principles |
| [**getFreshBiscuitBiscuitsFreshGet**](InteractiveApi.md#getfreshbiscuitbiscuitsfreshget) | **GET** /biscuits/fresh | Get a Fresh Biscuit |
| [**getRandomPrincipleCoachingPrinciplesRandomGet**](InteractiveApi.md#getrandomprinciplecoachingprinciplesrandomget) | **GET** /coaching/principles/random | Get a Random Coaching Principle |
| [**pressConferencePressPost**](InteractiveApi.md#pressconferencepresspost) | **POST** /press | Press Conference Simulator |
| [**reframeThoughtReframePost**](InteractiveApi.md#reframethoughtreframepost) | **POST** /reframe | Reframe Negative Thoughts |
| [**resolveConflictConflictsResolvePost**](InteractiveApi.md#resolveconflictconflictsresolvepost) | **POST** /conflicts/resolve | Resolve Conflicts |



## believeEngineBelievePost

> BelieveResponse believeEngineBelievePost(believeRequest)

The Believe Engine

Submit your situation and receive Ted Lasso-style motivational guidance.

### Example

```ts
import {
  Configuration,
  InteractiveApi,
} from '';
import type { BelieveEngineBelievePostRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InteractiveApi(config);

  const body = {
    // BelieveRequest
    believeRequest: ...,
  } satisfies BelieveEngineBelievePostRequest;

  try {
    const data = await api.believeEngineBelievePost(body);
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
| **believeRequest** | [BelieveRequest](BelieveRequest.md) |  | |

### Return type

[**BelieveResponse**](BelieveResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Motivational response generated |  -  |
| **418** | You\&#39;re already a believer! |  -  |
| **422** | Validation Error |  -  |
| **429** | Too much negativity detected |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getBiscuitBiscuitsBiscuitIdGet

> Biscuit getBiscuitBiscuitsBiscuitIdGet(biscuitId)

Get a Specific Biscuit

Get a specific type of biscuit by ID.

### Example

```ts
import {
  Configuration,
  InteractiveApi,
} from '';
import type { GetBiscuitBiscuitsBiscuitIdGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InteractiveApi(config);

  const body = {
    // string
    biscuitId: biscuitId_example,
  } satisfies GetBiscuitBiscuitsBiscuitIdGetRequest;

  try {
    const data = await api.getBiscuitBiscuitsBiscuitIdGet(body);
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
| **biscuitId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Biscuit**](Biscuit.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Biscuit details |  -  |
| **404** | Biscuit not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getBiscuitsBiscuitsGet

> PaginatedResponseBiscuit getBiscuitsBiscuitsGet(skip, limit)

Biscuits as a Service

Get a paginated list of Ted\&#39;s famous homemade biscuits! Each comes with a heartwarming message.

### Example

```ts
import {
  Configuration,
  InteractiveApi,
} from '';
import type { GetBiscuitsBiscuitsGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InteractiveApi(config);

  const body = {
    // number | Number of items to skip (offset) (optional)
    skip: 56,
    // number | Maximum number of items to return (max: 100) (optional)
    limit: 56,
  } satisfies GetBiscuitsBiscuitsGetRequest;

  try {
    const data = await api.getBiscuitsBiscuitsGet(body);
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
| **skip** | `number` | Number of items to skip (offset) | [Optional] [Defaults to `0`] |
| **limit** | `number` | Maximum number of items to return (max: 100) | [Optional] [Defaults to `20`] |

### Return type

[**PaginatedResponseBiscuit**](PaginatedResponseBiscuit.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of fresh biscuits from Ted\&#39;s kitchen |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getCoachingPrincipleCoachingPrinciplesPrincipleIdGet

> CoachingPrinciple getCoachingPrincipleCoachingPrinciplesPrincipleIdGet(principleId)

Get a Specific Coaching Principle

Get details about a specific coaching principle.

### Example

```ts
import {
  Configuration,
  InteractiveApi,
} from '';
import type { GetCoachingPrincipleCoachingPrinciplesPrincipleIdGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InteractiveApi(config);

  const body = {
    // string
    principleId: principleId_example,
  } satisfies GetCoachingPrincipleCoachingPrinciplesPrincipleIdGetRequest;

  try {
    const data = await api.getCoachingPrincipleCoachingPrinciplesPrincipleIdGet(body);
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
| **principleId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**CoachingPrinciple**](CoachingPrinciple.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Coaching principle details |  -  |
| **404** | Principle not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getCoachingPrinciplesCoachingPrinciplesGet

> PaginatedResponseCoachingPrinciple getCoachingPrinciplesCoachingPrinciplesGet(skip, limit)

Get Coaching Principles

Get a paginated list of Ted Lasso\&#39;s core coaching principles and philosophy.

### Example

```ts
import {
  Configuration,
  InteractiveApi,
} from '';
import type { GetCoachingPrinciplesCoachingPrinciplesGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InteractiveApi(config);

  const body = {
    // number | Number of items to skip (offset) (optional)
    skip: 56,
    // number | Maximum number of items to return (max: 100) (optional)
    limit: 56,
  } satisfies GetCoachingPrinciplesCoachingPrinciplesGetRequest;

  try {
    const data = await api.getCoachingPrinciplesCoachingPrinciplesGet(body);
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
| **skip** | `number` | Number of items to skip (offset) | [Optional] [Defaults to `0`] |
| **limit** | `number` | Maximum number of items to return (max: 100) | [Optional] [Defaults to `20`] |

### Return type

[**PaginatedResponseCoachingPrinciple**](PaginatedResponseCoachingPrinciple.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of coaching principles |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getFreshBiscuitBiscuitsFreshGet

> Biscuit getFreshBiscuitBiscuitsFreshGet()

Get a Fresh Biscuit

Get a single fresh biscuit with a personalized message from Ted.

### Example

```ts
import {
  Configuration,
  InteractiveApi,
} from '';
import type { GetFreshBiscuitBiscuitsFreshGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InteractiveApi(config);

  try {
    const data = await api.getFreshBiscuitBiscuitsFreshGet();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**Biscuit**](Biscuit.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | A fresh biscuit from Ted\&#39;s kitchen |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getRandomPrincipleCoachingPrinciplesRandomGet

> CoachingPrinciple getRandomPrincipleCoachingPrinciplesRandomGet()

Get a Random Coaching Principle

Get a random coaching principle to inspire your day.

### Example

```ts
import {
  Configuration,
  InteractiveApi,
} from '';
import type { GetRandomPrincipleCoachingPrinciplesRandomGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InteractiveApi(config);

  try {
    const data = await api.getRandomPrincipleCoachingPrinciplesRandomGet();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**CoachingPrinciple**](CoachingPrinciple.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | A random coaching principle |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## pressConferencePressPost

> PressConferenceResponse pressConferencePressPost(pressConferenceRequest)

Press Conference Simulator

Get Ted\&#39;s response to press conference questions.

### Example

```ts
import {
  Configuration,
  InteractiveApi,
} from '';
import type { PressConferencePressPostRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InteractiveApi(config);

  const body = {
    // PressConferenceRequest
    pressConferenceRequest: ...,
  } satisfies PressConferencePressPostRequest;

  try {
    const data = await api.pressConferencePressPost(body);
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
| **pressConferenceRequest** | [PressConferenceRequest](PressConferenceRequest.md) |  | |

### Return type

[**PressConferenceResponse**](PressConferenceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Press conference response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## reframeThoughtReframePost

> ReframeResponse reframeThoughtReframePost(reframeRequest)

Reframe Negative Thoughts

Transform negative thoughts into positive perspectives with Ted\&#39;s help.

### Example

```ts
import {
  Configuration,
  InteractiveApi,
} from '';
import type { ReframeThoughtReframePostRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InteractiveApi(config);

  const body = {
    // ReframeRequest
    reframeRequest: ...,
  } satisfies ReframeThoughtReframePostRequest;

  try {
    const data = await api.reframeThoughtReframePost(body);
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
| **reframeRequest** | [ReframeRequest](ReframeRequest.md) |  | |

### Return type

[**ReframeResponse**](ReframeResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Reframed perspective |  -  |
| **422** | Validation Error |  -  |
| **429** | Too much negativity |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## resolveConflictConflictsResolvePost

> ConflictResolution resolveConflictConflictsResolvePost(conflictRequest)

Resolve Conflicts

Get Ted Lasso-style advice for resolving conflicts.

### Example

```ts
import {
  Configuration,
  InteractiveApi,
} from '';
import type { ResolveConflictConflictsResolvePostRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InteractiveApi(config);

  const body = {
    // ConflictRequest
    conflictRequest: ...,
  } satisfies ResolveConflictConflictsResolvePostRequest;

  try {
    const data = await api.resolveConflictConflictsResolvePost(body);
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
| **conflictRequest** | [ConflictRequest](ConflictRequest.md) |  | |

### Return type

[**ConflictResolution**](ConflictResolution.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Conflict resolution guidance |  -  |
| **403** | Too judgmental |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

