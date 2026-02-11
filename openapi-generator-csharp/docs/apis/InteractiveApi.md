# Org.OpenAPITools.Api.InteractiveApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BelieveEngineBelievePost**](InteractiveApi.md#believeenginebelievepost) | **POST** /believe | The Believe Engine |
| [**GetBiscuitBiscuitsBiscuitIdGet**](InteractiveApi.md#getbiscuitbiscuitsbiscuitidget) | **GET** /biscuits/{biscuit_id} | Get a Specific Biscuit |
| [**GetBiscuitsBiscuitsGet**](InteractiveApi.md#getbiscuitsbiscuitsget) | **GET** /biscuits | Biscuits as a Service |
| [**GetCoachingPrincipleCoachingPrinciplesPrincipleIdGet**](InteractiveApi.md#getcoachingprinciplecoachingprinciplesprincipleidget) | **GET** /coaching/principles/{principle_id} | Get a Specific Coaching Principle |
| [**GetCoachingPrinciplesCoachingPrinciplesGet**](InteractiveApi.md#getcoachingprinciplescoachingprinciplesget) | **GET** /coaching/principles | Get Coaching Principles |
| [**GetFreshBiscuitBiscuitsFreshGet**](InteractiveApi.md#getfreshbiscuitbiscuitsfreshget) | **GET** /biscuits/fresh | Get a Fresh Biscuit |
| [**GetRandomPrincipleCoachingPrinciplesRandomGet**](InteractiveApi.md#getrandomprinciplecoachingprinciplesrandomget) | **GET** /coaching/principles/random | Get a Random Coaching Principle |
| [**PressConferencePressPost**](InteractiveApi.md#pressconferencepresspost) | **POST** /press | Press Conference Simulator |
| [**ReframeThoughtReframePost**](InteractiveApi.md#reframethoughtreframepost) | **POST** /reframe | Reframe Negative Thoughts |
| [**ResolveConflictConflictsResolvePost**](InteractiveApi.md#resolveconflictconflictsresolvepost) | **POST** /conflicts/resolve | Resolve Conflicts |

<a id="believeenginebelievepost"></a>
# **BelieveEngineBelievePost**
> BelieveResponse BelieveEngineBelievePost (BelieveRequest believeRequest)

The Believe Engine

Submit your situation and receive Ted Lasso-style motivational guidance.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **believeRequest** | [**BelieveRequest**](BelieveRequest.md) |  |  |

### Return type

[**BelieveResponse**](BelieveResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Motivational response generated |  -  |
| **418** | You&#39;re already a believer! |  -  |
| **422** | Validation Error |  -  |
| **429** | Too much negativity detected |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getbiscuitbiscuitsbiscuitidget"></a>
# **GetBiscuitBiscuitsBiscuitIdGet**
> Biscuit GetBiscuitBiscuitsBiscuitIdGet (string biscuitId)

Get a Specific Biscuit

Get a specific type of biscuit by ID.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **biscuitId** | **string** |  |  |

### Return type

[**Biscuit**](Biscuit.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Biscuit details |  -  |
| **404** | Biscuit not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getbiscuitsbiscuitsget"></a>
# **GetBiscuitsBiscuitsGet**
> PaginatedResponseBiscuit GetBiscuitsBiscuitsGet (int skip = null, int limit = null)

Biscuits as a Service

Get a paginated list of Ted's famous homemade biscuits! Each comes with a heartwarming message.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **skip** | **int** | Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int** | Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseBiscuit**](PaginatedResponseBiscuit.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of fresh biscuits from Ted&#39;s kitchen |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getcoachingprinciplecoachingprinciplesprincipleidget"></a>
# **GetCoachingPrincipleCoachingPrinciplesPrincipleIdGet**
> CoachingPrinciple GetCoachingPrincipleCoachingPrinciplesPrincipleIdGet (string principleId)

Get a Specific Coaching Principle

Get details about a specific coaching principle.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **principleId** | **string** |  |  |

### Return type

[**CoachingPrinciple**](CoachingPrinciple.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Coaching principle details |  -  |
| **404** | Principle not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getcoachingprinciplescoachingprinciplesget"></a>
# **GetCoachingPrinciplesCoachingPrinciplesGet**
> PaginatedResponseCoachingPrinciple GetCoachingPrinciplesCoachingPrinciplesGet (int skip = null, int limit = null)

Get Coaching Principles

Get a paginated list of Ted Lasso's core coaching principles and philosophy.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **skip** | **int** | Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int** | Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseCoachingPrinciple**](PaginatedResponseCoachingPrinciple.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of coaching principles |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getfreshbiscuitbiscuitsfreshget"></a>
# **GetFreshBiscuitBiscuitsFreshGet**
> Biscuit GetFreshBiscuitBiscuitsFreshGet ()

Get a Fresh Biscuit

Get a single fresh biscuit with a personalized message from Ted.


### Parameters
This endpoint does not need any parameter.
### Return type

[**Biscuit**](Biscuit.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | A fresh biscuit from Ted&#39;s kitchen |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getrandomprinciplecoachingprinciplesrandomget"></a>
# **GetRandomPrincipleCoachingPrinciplesRandomGet**
> CoachingPrinciple GetRandomPrincipleCoachingPrinciplesRandomGet ()

Get a Random Coaching Principle

Get a random coaching principle to inspire your day.


### Parameters
This endpoint does not need any parameter.
### Return type

[**CoachingPrinciple**](CoachingPrinciple.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | A random coaching principle |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="pressconferencepresspost"></a>
# **PressConferencePressPost**
> PressConferenceResponse PressConferencePressPost (PressConferenceRequest pressConferenceRequest)

Press Conference Simulator

Get Ted's response to press conference questions.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **pressConferenceRequest** | [**PressConferenceRequest**](PressConferenceRequest.md) |  |  |

### Return type

[**PressConferenceResponse**](PressConferenceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Press conference response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="reframethoughtreframepost"></a>
# **ReframeThoughtReframePost**
> ReframeResponse ReframeThoughtReframePost (ReframeRequest reframeRequest)

Reframe Negative Thoughts

Transform negative thoughts into positive perspectives with Ted's help.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **reframeRequest** | [**ReframeRequest**](ReframeRequest.md) |  |  |

### Return type

[**ReframeResponse**](ReframeResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Reframed perspective |  -  |
| **422** | Validation Error |  -  |
| **429** | Too much negativity |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="resolveconflictconflictsresolvepost"></a>
# **ResolveConflictConflictsResolvePost**
> ConflictResolution ResolveConflictConflictsResolvePost (ConflictRequest conflictRequest)

Resolve Conflicts

Get Ted Lasso-style advice for resolving conflicts.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **conflictRequest** | [**ConflictRequest**](ConflictRequest.md) |  |  |

### Return type

[**ConflictResolution**](ConflictResolution.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Conflict resolution guidance |  -  |
| **403** | Too judgmental |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

