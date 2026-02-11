# InteractiveApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**believeEngineBelievePost**](InteractiveApi.md#believeEngineBelievePost) | **POST** /believe | The Believe Engine |
| [**getBiscuitBiscuitsBiscuitIdGet**](InteractiveApi.md#getBiscuitBiscuitsBiscuitIdGet) | **GET** /biscuits/{biscuit_id} | Get a Specific Biscuit |
| [**getBiscuitsBiscuitsGet**](InteractiveApi.md#getBiscuitsBiscuitsGet) | **GET** /biscuits | Biscuits as a Service |
| [**getCoachingPrincipleCoachingPrinciplesPrincipleIdGet**](InteractiveApi.md#getCoachingPrincipleCoachingPrinciplesPrincipleIdGet) | **GET** /coaching/principles/{principle_id} | Get a Specific Coaching Principle |
| [**getCoachingPrinciplesCoachingPrinciplesGet**](InteractiveApi.md#getCoachingPrinciplesCoachingPrinciplesGet) | **GET** /coaching/principles | Get Coaching Principles |
| [**getFreshBiscuitBiscuitsFreshGet**](InteractiveApi.md#getFreshBiscuitBiscuitsFreshGet) | **GET** /biscuits/fresh | Get a Fresh Biscuit |
| [**getRandomPrincipleCoachingPrinciplesRandomGet**](InteractiveApi.md#getRandomPrincipleCoachingPrinciplesRandomGet) | **GET** /coaching/principles/random | Get a Random Coaching Principle |
| [**pressConferencePressPost**](InteractiveApi.md#pressConferencePressPost) | **POST** /press | Press Conference Simulator |
| [**reframeThoughtReframePost**](InteractiveApi.md#reframeThoughtReframePost) | **POST** /reframe | Reframe Negative Thoughts |
| [**resolveConflictConflictsResolvePost**](InteractiveApi.md#resolveConflictConflictsResolvePost) | **POST** /conflicts/resolve | Resolve Conflicts |


<a id="believeEngineBelievePost"></a>
# **believeEngineBelievePost**
> BelieveResponse believeEngineBelievePost(believeRequest)

The Believe Engine

Submit your situation and receive Ted Lasso-style motivational guidance.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InteractiveApi()
val believeRequest : BelieveRequest =  // BelieveRequest | 
try {
    val result : BelieveResponse = apiInstance.believeEngineBelievePost(believeRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InteractiveApi#believeEngineBelievePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InteractiveApi#believeEngineBelievePost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **believeRequest** | [**BelieveRequest**](BelieveRequest.md)|  | |

### Return type

[**BelieveResponse**](BelieveResponse.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="getBiscuitBiscuitsBiscuitIdGet"></a>
# **getBiscuitBiscuitsBiscuitIdGet**
> Biscuit getBiscuitBiscuitsBiscuitIdGet(biscuitId)

Get a Specific Biscuit

Get a specific type of biscuit by ID.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InteractiveApi()
val biscuitId : kotlin.String = biscuitId_example // kotlin.String | 
try {
    val result : Biscuit = apiInstance.getBiscuitBiscuitsBiscuitIdGet(biscuitId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InteractiveApi#getBiscuitBiscuitsBiscuitIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InteractiveApi#getBiscuitBiscuitsBiscuitIdGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **biscuitId** | **kotlin.String**|  | |

### Return type

[**Biscuit**](Biscuit.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getBiscuitsBiscuitsGet"></a>
# **getBiscuitsBiscuitsGet**
> PaginatedResponseBiscuit getBiscuitsBiscuitsGet(skip, limit)

Biscuits as a Service

Get a paginated list of Ted&#39;s famous homemade biscuits! Each comes with a heartwarming message.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InteractiveApi()
val skip : kotlin.Int = 56 // kotlin.Int | Number of items to skip (offset)
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return (max: 100)
try {
    val result : PaginatedResponseBiscuit = apiInstance.getBiscuitsBiscuitsGet(skip, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InteractiveApi#getBiscuitsBiscuitsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InteractiveApi#getBiscuitsBiscuitsGet")
    e.printStackTrace()
}
```

### Parameters
| **skip** | **kotlin.Int**| Number of items to skip (offset) | [optional] [default to 0] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseBiscuit**](PaginatedResponseBiscuit.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getCoachingPrincipleCoachingPrinciplesPrincipleIdGet"></a>
# **getCoachingPrincipleCoachingPrinciplesPrincipleIdGet**
> CoachingPrinciple getCoachingPrincipleCoachingPrinciplesPrincipleIdGet(principleId)

Get a Specific Coaching Principle

Get details about a specific coaching principle.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InteractiveApi()
val principleId : kotlin.String = principleId_example // kotlin.String | 
try {
    val result : CoachingPrinciple = apiInstance.getCoachingPrincipleCoachingPrinciplesPrincipleIdGet(principleId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InteractiveApi#getCoachingPrincipleCoachingPrinciplesPrincipleIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InteractiveApi#getCoachingPrincipleCoachingPrinciplesPrincipleIdGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **principleId** | **kotlin.String**|  | |

### Return type

[**CoachingPrinciple**](CoachingPrinciple.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getCoachingPrinciplesCoachingPrinciplesGet"></a>
# **getCoachingPrinciplesCoachingPrinciplesGet**
> PaginatedResponseCoachingPrinciple getCoachingPrinciplesCoachingPrinciplesGet(skip, limit)

Get Coaching Principles

Get a paginated list of Ted Lasso&#39;s core coaching principles and philosophy.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InteractiveApi()
val skip : kotlin.Int = 56 // kotlin.Int | Number of items to skip (offset)
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return (max: 100)
try {
    val result : PaginatedResponseCoachingPrinciple = apiInstance.getCoachingPrinciplesCoachingPrinciplesGet(skip, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InteractiveApi#getCoachingPrinciplesCoachingPrinciplesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InteractiveApi#getCoachingPrinciplesCoachingPrinciplesGet")
    e.printStackTrace()
}
```

### Parameters
| **skip** | **kotlin.Int**| Number of items to skip (offset) | [optional] [default to 0] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseCoachingPrinciple**](PaginatedResponseCoachingPrinciple.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getFreshBiscuitBiscuitsFreshGet"></a>
# **getFreshBiscuitBiscuitsFreshGet**
> Biscuit getFreshBiscuitBiscuitsFreshGet()

Get a Fresh Biscuit

Get a single fresh biscuit with a personalized message from Ted.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InteractiveApi()
try {
    val result : Biscuit = apiInstance.getFreshBiscuitBiscuitsFreshGet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InteractiveApi#getFreshBiscuitBiscuitsFreshGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InteractiveApi#getFreshBiscuitBiscuitsFreshGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**Biscuit**](Biscuit.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getRandomPrincipleCoachingPrinciplesRandomGet"></a>
# **getRandomPrincipleCoachingPrinciplesRandomGet**
> CoachingPrinciple getRandomPrincipleCoachingPrinciplesRandomGet()

Get a Random Coaching Principle

Get a random coaching principle to inspire your day.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InteractiveApi()
try {
    val result : CoachingPrinciple = apiInstance.getRandomPrincipleCoachingPrinciplesRandomGet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InteractiveApi#getRandomPrincipleCoachingPrinciplesRandomGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InteractiveApi#getRandomPrincipleCoachingPrinciplesRandomGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CoachingPrinciple**](CoachingPrinciple.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="pressConferencePressPost"></a>
# **pressConferencePressPost**
> PressConferenceResponse pressConferencePressPost(pressConferenceRequest)

Press Conference Simulator

Get Ted&#39;s response to press conference questions.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InteractiveApi()
val pressConferenceRequest : PressConferenceRequest =  // PressConferenceRequest | 
try {
    val result : PressConferenceResponse = apiInstance.pressConferencePressPost(pressConferenceRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InteractiveApi#pressConferencePressPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InteractiveApi#pressConferencePressPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pressConferenceRequest** | [**PressConferenceRequest**](PressConferenceRequest.md)|  | |

### Return type

[**PressConferenceResponse**](PressConferenceResponse.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="reframeThoughtReframePost"></a>
# **reframeThoughtReframePost**
> ReframeResponse reframeThoughtReframePost(reframeRequest)

Reframe Negative Thoughts

Transform negative thoughts into positive perspectives with Ted&#39;s help.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InteractiveApi()
val reframeRequest : ReframeRequest =  // ReframeRequest | 
try {
    val result : ReframeResponse = apiInstance.reframeThoughtReframePost(reframeRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InteractiveApi#reframeThoughtReframePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InteractiveApi#reframeThoughtReframePost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **reframeRequest** | [**ReframeRequest**](ReframeRequest.md)|  | |

### Return type

[**ReframeResponse**](ReframeResponse.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="resolveConflictConflictsResolvePost"></a>
# **resolveConflictConflictsResolvePost**
> ConflictResolution resolveConflictConflictsResolvePost(conflictRequest)

Resolve Conflicts

Get Ted Lasso-style advice for resolving conflicts.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InteractiveApi()
val conflictRequest : ConflictRequest =  // ConflictRequest | 
try {
    val result : ConflictResolution = apiInstance.resolveConflictConflictsResolvePost(conflictRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InteractiveApi#resolveConflictConflictsResolvePost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InteractiveApi#resolveConflictConflictsResolvePost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **conflictRequest** | [**ConflictRequest**](ConflictRequest.md)|  | |

### Return type

[**ConflictResolution**](ConflictResolution.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

