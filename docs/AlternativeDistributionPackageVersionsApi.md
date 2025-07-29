# openapi_client.AlternativeDistributionPackageVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**alternative_distribution_package_versions_deltas_get_to_many_related**](AlternativeDistributionPackageVersionsApi.md#alternative_distribution_package_versions_deltas_get_to_many_related) | **GET** /v1/alternativeDistributionPackageVersions/{id}/deltas | 
[**alternative_distribution_package_versions_deltas_get_to_many_relationship**](AlternativeDistributionPackageVersionsApi.md#alternative_distribution_package_versions_deltas_get_to_many_relationship) | **GET** /v1/alternativeDistributionPackageVersions/{id}/relationships/deltas | 
[**alternative_distribution_package_versions_get_instance**](AlternativeDistributionPackageVersionsApi.md#alternative_distribution_package_versions_get_instance) | **GET** /v1/alternativeDistributionPackageVersions/{id} | 
[**alternative_distribution_package_versions_variants_get_to_many_related**](AlternativeDistributionPackageVersionsApi.md#alternative_distribution_package_versions_variants_get_to_many_related) | **GET** /v1/alternativeDistributionPackageVersions/{id}/variants | 
[**alternative_distribution_package_versions_variants_get_to_many_relationship**](AlternativeDistributionPackageVersionsApi.md#alternative_distribution_package_versions_variants_get_to_many_relationship) | **GET** /v1/alternativeDistributionPackageVersions/{id}/relationships/variants | 


# **alternative_distribution_package_versions_deltas_get_to_many_related**
> AlternativeDistributionPackageDeltasResponse alternative_distribution_package_versions_deltas_get_to_many_related(id, fields_alternative_distribution_package_deltas=fields_alternative_distribution_package_deltas, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.alternative_distribution_package_deltas_response import AlternativeDistributionPackageDeltasResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.AlternativeDistributionPackageVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_alternative_distribution_package_deltas = ['fields_alternative_distribution_package_deltas_example'] # List[str] | the fields to include for returned resources of type alternativeDistributionPackageDeltas (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.alternative_distribution_package_versions_deltas_get_to_many_related(id, fields_alternative_distribution_package_deltas=fields_alternative_distribution_package_deltas, limit=limit)
        print("The response of AlternativeDistributionPackageVersionsApi->alternative_distribution_package_versions_deltas_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlternativeDistributionPackageVersionsApi->alternative_distribution_package_versions_deltas_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_alternative_distribution_package_deltas** | [**List[str]**](str.md)| the fields to include for returned resources of type alternativeDistributionPackageDeltas | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AlternativeDistributionPackageDeltasResponse**](AlternativeDistributionPackageDeltasResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of AlternativeDistributionPackageDeltas |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **alternative_distribution_package_versions_deltas_get_to_many_relationship**
> AlternativeDistributionPackageVersionDeltasLinkagesResponse alternative_distribution_package_versions_deltas_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.alternative_distribution_package_version_deltas_linkages_response import AlternativeDistributionPackageVersionDeltasLinkagesResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.AlternativeDistributionPackageVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.alternative_distribution_package_versions_deltas_get_to_many_relationship(id, limit=limit)
        print("The response of AlternativeDistributionPackageVersionsApi->alternative_distribution_package_versions_deltas_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlternativeDistributionPackageVersionsApi->alternative_distribution_package_versions_deltas_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AlternativeDistributionPackageVersionDeltasLinkagesResponse**](AlternativeDistributionPackageVersionDeltasLinkagesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of related linkages |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **alternative_distribution_package_versions_get_instance**
> AlternativeDistributionPackageVersionResponse alternative_distribution_package_versions_get_instance(id, fields_alternative_distribution_package_versions=fields_alternative_distribution_package_versions, fields_alternative_distribution_package_variants=fields_alternative_distribution_package_variants, fields_alternative_distribution_package_deltas=fields_alternative_distribution_package_deltas, include=include, limit_deltas=limit_deltas, limit_variants=limit_variants)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.alternative_distribution_package_version_response import AlternativeDistributionPackageVersionResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.AlternativeDistributionPackageVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_alternative_distribution_package_versions = ['fields_alternative_distribution_package_versions_example'] # List[str] | the fields to include for returned resources of type alternativeDistributionPackageVersions (optional)
    fields_alternative_distribution_package_variants = ['fields_alternative_distribution_package_variants_example'] # List[str] | the fields to include for returned resources of type alternativeDistributionPackageVariants (optional)
    fields_alternative_distribution_package_deltas = ['fields_alternative_distribution_package_deltas_example'] # List[str] | the fields to include for returned resources of type alternativeDistributionPackageDeltas (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_deltas = 56 # int | maximum number of related deltas returned (when they are included) (optional)
    limit_variants = 56 # int | maximum number of related variants returned (when they are included) (optional)

    try:
        api_response = api_instance.alternative_distribution_package_versions_get_instance(id, fields_alternative_distribution_package_versions=fields_alternative_distribution_package_versions, fields_alternative_distribution_package_variants=fields_alternative_distribution_package_variants, fields_alternative_distribution_package_deltas=fields_alternative_distribution_package_deltas, include=include, limit_deltas=limit_deltas, limit_variants=limit_variants)
        print("The response of AlternativeDistributionPackageVersionsApi->alternative_distribution_package_versions_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlternativeDistributionPackageVersionsApi->alternative_distribution_package_versions_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_alternative_distribution_package_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type alternativeDistributionPackageVersions | [optional] 
 **fields_alternative_distribution_package_variants** | [**List[str]**](str.md)| the fields to include for returned resources of type alternativeDistributionPackageVariants | [optional] 
 **fields_alternative_distribution_package_deltas** | [**List[str]**](str.md)| the fields to include for returned resources of type alternativeDistributionPackageDeltas | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_deltas** | **int**| maximum number of related deltas returned (when they are included) | [optional] 
 **limit_variants** | **int**| maximum number of related variants returned (when they are included) | [optional] 

### Return type

[**AlternativeDistributionPackageVersionResponse**](AlternativeDistributionPackageVersionResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Single AlternativeDistributionPackageVersion |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **alternative_distribution_package_versions_variants_get_to_many_related**
> AlternativeDistributionPackageVariantsResponse alternative_distribution_package_versions_variants_get_to_many_related(id, fields_alternative_distribution_package_variants=fields_alternative_distribution_package_variants, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.alternative_distribution_package_variants_response import AlternativeDistributionPackageVariantsResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.AlternativeDistributionPackageVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_alternative_distribution_package_variants = ['fields_alternative_distribution_package_variants_example'] # List[str] | the fields to include for returned resources of type alternativeDistributionPackageVariants (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.alternative_distribution_package_versions_variants_get_to_many_related(id, fields_alternative_distribution_package_variants=fields_alternative_distribution_package_variants, limit=limit)
        print("The response of AlternativeDistributionPackageVersionsApi->alternative_distribution_package_versions_variants_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlternativeDistributionPackageVersionsApi->alternative_distribution_package_versions_variants_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_alternative_distribution_package_variants** | [**List[str]**](str.md)| the fields to include for returned resources of type alternativeDistributionPackageVariants | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AlternativeDistributionPackageVariantsResponse**](AlternativeDistributionPackageVariantsResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of AlternativeDistributionPackageVariants |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **alternative_distribution_package_versions_variants_get_to_many_relationship**
> AlternativeDistributionPackageVersionVariantsLinkagesResponse alternative_distribution_package_versions_variants_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.alternative_distribution_package_version_variants_linkages_response import AlternativeDistributionPackageVersionVariantsLinkagesResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.AlternativeDistributionPackageVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.alternative_distribution_package_versions_variants_get_to_many_relationship(id, limit=limit)
        print("The response of AlternativeDistributionPackageVersionsApi->alternative_distribution_package_versions_variants_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlternativeDistributionPackageVersionsApi->alternative_distribution_package_versions_variants_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AlternativeDistributionPackageVersionVariantsLinkagesResponse**](AlternativeDistributionPackageVersionVariantsLinkagesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of related linkages |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

