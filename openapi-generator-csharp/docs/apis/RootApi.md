# Org.OpenAPITools.Api.RootApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**HealthCheckHealthGet**](RootApi.md#healthcheckhealthget) | **GET** /health | Health Check |
| [**RootGet**](RootApi.md#rootget) | **GET** / | Welcome to the Ted Lasso API |
| [**VersionInfoVersionGet**](RootApi.md#versioninfoversionget) | **GET** /version | API Version Information |

<a id="healthcheckhealthget"></a>
# **HealthCheckHealthGet**
> Object HealthCheckHealthGet ()

Health Check

Check if the API is running and healthy.


### Parameters
This endpoint does not need any parameter.
### Return type

**Object**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | API health status |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="rootget"></a>
# **RootGet**
> Object RootGet ()

Welcome to the Ted Lasso API

Get a warm welcome and overview of available endpoints.


### Parameters
This endpoint does not need any parameter.
### Return type

**Object**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Welcome message and API overview |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="versioninfoversionget"></a>
# **VersionInfoVersionGet**
> Object VersionInfoVersionGet ()

API Version Information

Get detailed information about API versioning.


### Parameters
This endpoint does not need any parameter.
### Return type

**Object**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

