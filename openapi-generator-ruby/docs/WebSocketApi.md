# OpenapiClient::WebSocketApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**live_match_websocket**](WebSocketApi.md#live_match_websocket) | **GET** /matches/live | Live Match Simulation WebSocket |
| [**websocket_test**](WebSocketApi.md#websocket_test) | **GET** /ws/test | WebSocket Test Endpoint |


## live_match_websocket

> live_match_websocket(opts)

Live Match Simulation WebSocket

WebSocket endpoint for real-time live match simulation.  Connect to receive a stream of match events as they happen in a simulated football match.  ## Connection  Connect via WebSocket with optional query parameters to customize the simulation.  ## Example WebSocket URL  ``` ws://localhost:8000/matches/live?home_team=AFC%20Richmond&away_team=Manchester%20City&speed=2.0&excitement_level=7 ```  ## Server Messages  The server sends JSON messages with these types: - `match_start` - When the match begins - `match_event` - For each match event (goals, fouls, cards, etc.) - `match_end` - When the match concludes - `error` - If an error occurs - `pong` - Response to client ping  ## Client Messages  Send JSON to control the simulation: - `{\"action\": \"ping\"}` - Keep-alive, server responds with `{\"type\": \"pong\"}` - `{\"action\": \"pause\"}` - Pause the simulation - `{\"action\": \"resume\"}` - Resume a paused simulation - `{\"action\": \"set_speed\", \"speed\": 2.0}` - Change playback speed (0.1-10.0) - `{\"action\": \"get_status\"}` - Request current match status 

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebSocketApi.new
opts = {
  home_team: 'home_team_example', # String | Home team name
  away_team: 'away_team_example', # String | Away team name
  speed: 8.14, # Float | Simulation speed multiplier (1.0 = real-time)
  excitement_level: 56 # Integer | How eventful the match should be (1=boring, 10=chaos)
}

begin
  # Live Match Simulation WebSocket
  api_instance.live_match_websocket(opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebSocketApi->live_match_websocket: #{e}"
end
```

#### Using the live_match_websocket_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> live_match_websocket_with_http_info(opts)

```ruby
begin
  # Live Match Simulation WebSocket
  data, status_code, headers = api_instance.live_match_websocket_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebSocketApi->live_match_websocket_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **home_team** | **String** | Home team name | [optional][default to &#39;AFC Richmond&#39;] |
| **away_team** | **String** | Away team name | [optional][default to &#39;West Ham United&#39;] |
| **speed** | **Float** | Simulation speed multiplier (1.0 &#x3D; real-time) | [optional][default to 1.0] |
| **excitement_level** | **Integer** | How eventful the match should be (1&#x3D;boring, 10&#x3D;chaos) | [optional][default to 5] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## websocket_test

> websocket_test

WebSocket Test Endpoint

Simple WebSocket test endpoint for connectivity testing.  Connect to test WebSocket functionality. The server will: 1. Send a welcome message on connection 2. Echo back any message you send  ## Example  ```javascript const ws = new WebSocket('ws://localhost:8000/ws/test'); ws.onmessage = (event) => console.log(event.data); ws.send('Hello!');  // Server responds with echo ``` 

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebSocketApi.new

begin
  # WebSocket Test Endpoint
  api_instance.websocket_test
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebSocketApi->websocket_test: #{e}"
end
```

#### Using the websocket_test_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> websocket_test_with_http_info

```ruby
begin
  # WebSocket Test Endpoint
  data, status_code, headers = api_instance.websocket_test_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebSocketApi->websocket_test_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

