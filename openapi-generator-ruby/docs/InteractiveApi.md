# OpenapiClient::InteractiveApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**believe_engine_believe_post**](InteractiveApi.md#believe_engine_believe_post) | **POST** /believe | The Believe Engine |
| [**get_biscuit_biscuits_biscuit_id_get**](InteractiveApi.md#get_biscuit_biscuits_biscuit_id_get) | **GET** /biscuits/{biscuit_id} | Get a Specific Biscuit |
| [**get_biscuits_biscuits_get**](InteractiveApi.md#get_biscuits_biscuits_get) | **GET** /biscuits | Biscuits as a Service |
| [**get_coaching_principle_coaching_principles_principle_id_get**](InteractiveApi.md#get_coaching_principle_coaching_principles_principle_id_get) | **GET** /coaching/principles/{principle_id} | Get a Specific Coaching Principle |
| [**get_coaching_principles_coaching_principles_get**](InteractiveApi.md#get_coaching_principles_coaching_principles_get) | **GET** /coaching/principles | Get Coaching Principles |
| [**get_fresh_biscuit_biscuits_fresh_get**](InteractiveApi.md#get_fresh_biscuit_biscuits_fresh_get) | **GET** /biscuits/fresh | Get a Fresh Biscuit |
| [**get_random_principle_coaching_principles_random_get**](InteractiveApi.md#get_random_principle_coaching_principles_random_get) | **GET** /coaching/principles/random | Get a Random Coaching Principle |
| [**press_conference_press_post**](InteractiveApi.md#press_conference_press_post) | **POST** /press | Press Conference Simulator |
| [**reframe_thought_reframe_post**](InteractiveApi.md#reframe_thought_reframe_post) | **POST** /reframe | Reframe Negative Thoughts |
| [**resolve_conflict_conflicts_resolve_post**](InteractiveApi.md#resolve_conflict_conflicts_resolve_post) | **POST** /conflicts/resolve | Resolve Conflicts |


## believe_engine_believe_post

> <BelieveResponse> believe_engine_believe_post(believe_request)

The Believe Engine

Submit your situation and receive Ted Lasso-style motivational guidance.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::InteractiveApi.new
believe_request = OpenapiClient::BelieveRequest.new({situation: 'I just got passed over for a promotion I've been working toward for two years.', situation_type: OpenapiClient::SituationType::WORK_CHALLENGE}) # BelieveRequest | 

begin
  # The Believe Engine
  result = api_instance.believe_engine_believe_post(believe_request)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InteractiveApi->believe_engine_believe_post: #{e}"
end
```

#### Using the believe_engine_believe_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BelieveResponse>, Integer, Hash)> believe_engine_believe_post_with_http_info(believe_request)

```ruby
begin
  # The Believe Engine
  data, status_code, headers = api_instance.believe_engine_believe_post_with_http_info(believe_request)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BelieveResponse>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InteractiveApi->believe_engine_believe_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **believe_request** | [**BelieveRequest**](BelieveRequest.md) |  |  |

### Return type

[**BelieveResponse**](BelieveResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## get_biscuit_biscuits_biscuit_id_get

> <Biscuit> get_biscuit_biscuits_biscuit_id_get(biscuit_id)

Get a Specific Biscuit

Get a specific type of biscuit by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::InteractiveApi.new
biscuit_id = 'biscuit_id_example' # String | 

begin
  # Get a Specific Biscuit
  result = api_instance.get_biscuit_biscuits_biscuit_id_get(biscuit_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InteractiveApi->get_biscuit_biscuits_biscuit_id_get: #{e}"
end
```

#### Using the get_biscuit_biscuits_biscuit_id_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Biscuit>, Integer, Hash)> get_biscuit_biscuits_biscuit_id_get_with_http_info(biscuit_id)

```ruby
begin
  # Get a Specific Biscuit
  data, status_code, headers = api_instance.get_biscuit_biscuits_biscuit_id_get_with_http_info(biscuit_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Biscuit>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InteractiveApi->get_biscuit_biscuits_biscuit_id_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **biscuit_id** | **String** |  |  |

### Return type

[**Biscuit**](Biscuit.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_biscuits_biscuits_get

> <PaginatedResponseBiscuit> get_biscuits_biscuits_get(opts)

Biscuits as a Service

Get a paginated list of Ted's famous homemade biscuits! Each comes with a heartwarming message.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::InteractiveApi.new
opts = {
  skip: 56, # Integer | Number of items to skip (offset)
  limit: 56 # Integer | Maximum number of items to return (max: 100)
}

begin
  # Biscuits as a Service
  result = api_instance.get_biscuits_biscuits_get(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InteractiveApi->get_biscuits_biscuits_get: #{e}"
end
```

#### Using the get_biscuits_biscuits_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaginatedResponseBiscuit>, Integer, Hash)> get_biscuits_biscuits_get_with_http_info(opts)

```ruby
begin
  # Biscuits as a Service
  data, status_code, headers = api_instance.get_biscuits_biscuits_get_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaginatedResponseBiscuit>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InteractiveApi->get_biscuits_biscuits_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **skip** | **Integer** | Number of items to skip (offset) | [optional][default to 0] |
| **limit** | **Integer** | Maximum number of items to return (max: 100) | [optional][default to 20] |

### Return type

[**PaginatedResponseBiscuit**](PaginatedResponseBiscuit.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_coaching_principle_coaching_principles_principle_id_get

> <CoachingPrinciple> get_coaching_principle_coaching_principles_principle_id_get(principle_id)

Get a Specific Coaching Principle

Get details about a specific coaching principle.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::InteractiveApi.new
principle_id = 'principle_id_example' # String | 

begin
  # Get a Specific Coaching Principle
  result = api_instance.get_coaching_principle_coaching_principles_principle_id_get(principle_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InteractiveApi->get_coaching_principle_coaching_principles_principle_id_get: #{e}"
end
```

#### Using the get_coaching_principle_coaching_principles_principle_id_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CoachingPrinciple>, Integer, Hash)> get_coaching_principle_coaching_principles_principle_id_get_with_http_info(principle_id)

```ruby
begin
  # Get a Specific Coaching Principle
  data, status_code, headers = api_instance.get_coaching_principle_coaching_principles_principle_id_get_with_http_info(principle_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CoachingPrinciple>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InteractiveApi->get_coaching_principle_coaching_principles_principle_id_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **principle_id** | **String** |  |  |

### Return type

[**CoachingPrinciple**](CoachingPrinciple.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_coaching_principles_coaching_principles_get

> <PaginatedResponseCoachingPrinciple> get_coaching_principles_coaching_principles_get(opts)

Get Coaching Principles

Get a paginated list of Ted Lasso's core coaching principles and philosophy.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::InteractiveApi.new
opts = {
  skip: 56, # Integer | Number of items to skip (offset)
  limit: 56 # Integer | Maximum number of items to return (max: 100)
}

begin
  # Get Coaching Principles
  result = api_instance.get_coaching_principles_coaching_principles_get(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InteractiveApi->get_coaching_principles_coaching_principles_get: #{e}"
end
```

#### Using the get_coaching_principles_coaching_principles_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaginatedResponseCoachingPrinciple>, Integer, Hash)> get_coaching_principles_coaching_principles_get_with_http_info(opts)

```ruby
begin
  # Get Coaching Principles
  data, status_code, headers = api_instance.get_coaching_principles_coaching_principles_get_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaginatedResponseCoachingPrinciple>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InteractiveApi->get_coaching_principles_coaching_principles_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **skip** | **Integer** | Number of items to skip (offset) | [optional][default to 0] |
| **limit** | **Integer** | Maximum number of items to return (max: 100) | [optional][default to 20] |

### Return type

[**PaginatedResponseCoachingPrinciple**](PaginatedResponseCoachingPrinciple.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_fresh_biscuit_biscuits_fresh_get

> <Biscuit> get_fresh_biscuit_biscuits_fresh_get

Get a Fresh Biscuit

Get a single fresh biscuit with a personalized message from Ted.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::InteractiveApi.new

begin
  # Get a Fresh Biscuit
  result = api_instance.get_fresh_biscuit_biscuits_fresh_get
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InteractiveApi->get_fresh_biscuit_biscuits_fresh_get: #{e}"
end
```

#### Using the get_fresh_biscuit_biscuits_fresh_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Biscuit>, Integer, Hash)> get_fresh_biscuit_biscuits_fresh_get_with_http_info

```ruby
begin
  # Get a Fresh Biscuit
  data, status_code, headers = api_instance.get_fresh_biscuit_biscuits_fresh_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Biscuit>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InteractiveApi->get_fresh_biscuit_biscuits_fresh_get_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**Biscuit**](Biscuit.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_random_principle_coaching_principles_random_get

> <CoachingPrinciple> get_random_principle_coaching_principles_random_get

Get a Random Coaching Principle

Get a random coaching principle to inspire your day.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::InteractiveApi.new

begin
  # Get a Random Coaching Principle
  result = api_instance.get_random_principle_coaching_principles_random_get
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InteractiveApi->get_random_principle_coaching_principles_random_get: #{e}"
end
```

#### Using the get_random_principle_coaching_principles_random_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CoachingPrinciple>, Integer, Hash)> get_random_principle_coaching_principles_random_get_with_http_info

```ruby
begin
  # Get a Random Coaching Principle
  data, status_code, headers = api_instance.get_random_principle_coaching_principles_random_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CoachingPrinciple>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InteractiveApi->get_random_principle_coaching_principles_random_get_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**CoachingPrinciple**](CoachingPrinciple.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## press_conference_press_post

> <PressConferenceResponse> press_conference_press_post(press_conference_request)

Press Conference Simulator

Get Ted's response to press conference questions.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::InteractiveApi.new
press_conference_request = OpenapiClient::PressConferenceRequest.new({question: 'Ted, your team just lost 5-0. How do you explain this embarrassing defeat?'}) # PressConferenceRequest | 

begin
  # Press Conference Simulator
  result = api_instance.press_conference_press_post(press_conference_request)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InteractiveApi->press_conference_press_post: #{e}"
end
```

#### Using the press_conference_press_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PressConferenceResponse>, Integer, Hash)> press_conference_press_post_with_http_info(press_conference_request)

```ruby
begin
  # Press Conference Simulator
  data, status_code, headers = api_instance.press_conference_press_post_with_http_info(press_conference_request)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PressConferenceResponse>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InteractiveApi->press_conference_press_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **press_conference_request** | [**PressConferenceRequest**](PressConferenceRequest.md) |  |  |

### Return type

[**PressConferenceResponse**](PressConferenceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## reframe_thought_reframe_post

> <ReframeResponse> reframe_thought_reframe_post(reframe_request)

Reframe Negative Thoughts

Transform negative thoughts into positive perspectives with Ted's help.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::InteractiveApi.new
reframe_request = OpenapiClient::ReframeRequest.new({negative_thought: 'I'm not good enough for this job.'}) # ReframeRequest | 

begin
  # Reframe Negative Thoughts
  result = api_instance.reframe_thought_reframe_post(reframe_request)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InteractiveApi->reframe_thought_reframe_post: #{e}"
end
```

#### Using the reframe_thought_reframe_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ReframeResponse>, Integer, Hash)> reframe_thought_reframe_post_with_http_info(reframe_request)

```ruby
begin
  # Reframe Negative Thoughts
  data, status_code, headers = api_instance.reframe_thought_reframe_post_with_http_info(reframe_request)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ReframeResponse>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InteractiveApi->reframe_thought_reframe_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **reframe_request** | [**ReframeRequest**](ReframeRequest.md) |  |  |

### Return type

[**ReframeResponse**](ReframeResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## resolve_conflict_conflicts_resolve_post

> <ConflictResolution> resolve_conflict_conflicts_resolve_post(conflict_request)

Resolve Conflicts

Get Ted Lasso-style advice for resolving conflicts.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::InteractiveApi.new
conflict_request = OpenapiClient::ConflictRequest.new({conflict_type: OpenapiClient::ConflictType::INTERPERSONAL, description: 'Alex keeps taking credit for my ideas in meetings and I'm getting resentful.', parties_involved: [Me,  My teammate Alex]}) # ConflictRequest | 

begin
  # Resolve Conflicts
  result = api_instance.resolve_conflict_conflicts_resolve_post(conflict_request)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InteractiveApi->resolve_conflict_conflicts_resolve_post: #{e}"
end
```

#### Using the resolve_conflict_conflicts_resolve_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ConflictResolution>, Integer, Hash)> resolve_conflict_conflicts_resolve_post_with_http_info(conflict_request)

```ruby
begin
  # Resolve Conflicts
  data, status_code, headers = api_instance.resolve_conflict_conflicts_resolve_post_with_http_info(conflict_request)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ConflictResolution>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InteractiveApi->resolve_conflict_conflicts_resolve_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **conflict_request** | [**ConflictRequest**](ConflictRequest.md) |  |  |

### Return type

[**ConflictResolution**](ConflictResolution.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

