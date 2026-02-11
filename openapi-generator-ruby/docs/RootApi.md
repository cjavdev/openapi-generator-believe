# OpenapiClient::RootApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**health_check_health_get**](RootApi.md#health_check_health_get) | **GET** /health | Health Check |
| [**root_get**](RootApi.md#root_get) | **GET** / | Welcome to the Ted Lasso API |
| [**version_info_version_get**](RootApi.md#version_info_version_get) | **GET** /version | API Version Information |


## health_check_health_get

> Object health_check_health_get

Health Check

Check if the API is running and healthy.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::RootApi.new

begin
  # Health Check
  result = api_instance.health_check_health_get
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RootApi->health_check_health_get: #{e}"
end
```

#### Using the health_check_health_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> health_check_health_get_with_http_info

```ruby
begin
  # Health Check
  data, status_code, headers = api_instance.health_check_health_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue OpenapiClient::ApiError => e
  puts "Error when calling RootApi->health_check_health_get_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

**Object**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## root_get

> Object root_get

Welcome to the Ted Lasso API

Get a warm welcome and overview of available endpoints.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::RootApi.new

begin
  # Welcome to the Ted Lasso API
  result = api_instance.root_get
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RootApi->root_get: #{e}"
end
```

#### Using the root_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> root_get_with_http_info

```ruby
begin
  # Welcome to the Ted Lasso API
  data, status_code, headers = api_instance.root_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue OpenapiClient::ApiError => e
  puts "Error when calling RootApi->root_get_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

**Object**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## version_info_version_get

> Object version_info_version_get

API Version Information

Get detailed information about API versioning.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::RootApi.new

begin
  # API Version Information
  result = api_instance.version_info_version_get
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RootApi->version_info_version_get: #{e}"
end
```

#### Using the version_info_version_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> version_info_version_get_with_http_info

```ruby
begin
  # API Version Information
  data, status_code, headers = api_instance.version_info_version_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue OpenapiClient::ApiError => e
  puts "Error when calling RootApi->version_info_version_get_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

**Object**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

