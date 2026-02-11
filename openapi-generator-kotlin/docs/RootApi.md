# RootApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**healthCheckHealthGet**](RootApi.md#healthCheckHealthGet) | **GET** /health | Health Check |
| [**rootGet**](RootApi.md#rootGet) | **GET** / | Welcome to the Ted Lasso API |
| [**versionInfoVersionGet**](RootApi.md#versionInfoVersionGet) | **GET** /version | API Version Information |


<a id="healthCheckHealthGet"></a>
# **healthCheckHealthGet**
> kotlin.Any healthCheckHealthGet()

Health Check

Check if the API is running and healthy.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RootApi()
try {
    val result : kotlin.Any = apiInstance.healthCheckHealthGet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RootApi#healthCheckHealthGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RootApi#healthCheckHealthGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="rootGet"></a>
# **rootGet**
> kotlin.Any rootGet()

Welcome to the Ted Lasso API

Get a warm welcome and overview of available endpoints.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RootApi()
try {
    val result : kotlin.Any = apiInstance.rootGet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RootApi#rootGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RootApi#rootGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="versionInfoVersionGet"></a>
# **versionInfoVersionGet**
> kotlin.Any versionInfoVersionGet()

API Version Information

Get detailed information about API versioning.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RootApi()
try {
    val result : kotlin.Any = apiInstance.versionInfoVersionGet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RootApi#versionInfoVersionGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RootApi#versionInfoVersionGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

