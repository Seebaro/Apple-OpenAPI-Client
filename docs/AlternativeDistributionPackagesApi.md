# openapi_client.AlternativeDistributionPackagesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**alternative_distribution_packages_create_instance**](AlternativeDistributionPackagesApi.md#alternative_distribution_packages_create_instance) | **POST** /v1/alternativeDistributionPackages | 
[**alternative_distribution_packages_get_instance**](AlternativeDistributionPackagesApi.md#alternative_distribution_packages_get_instance) | **GET** /v1/alternativeDistributionPackages/{id} | 
[**alternative_distribution_packages_versions_get_to_many_related**](AlternativeDistributionPackagesApi.md#alternative_distribution_packages_versions_get_to_many_related) | **GET** /v1/alternativeDistributionPackages/{id}/versions | 
[**alternative_distribution_packages_versions_get_to_many_relationship**](AlternativeDistributionPackagesApi.md#alternative_distribution_packages_versions_get_to_many_relationship) | **GET** /v1/alternativeDistributionPackages/{id}/relationships/versions | 


# **alternative_distribution_packages_create_instance**
> AlternativeDistributionPackageResponse alternative_distribution_packages_create_instance(alternative_distribution_package_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.alternative_distribution_package_create_request import AlternativeDistributionPackageCreateRequest
from openapi_client.models.alternative_distribution_package_response import AlternativeDistributionPackageResponse
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
    api_instance = openapi_client.AlternativeDistributionPackagesApi(api_client)
    alternative_distribution_package_create_request = openapi_client.AlternativeDistributionPackageCreateRequest() # AlternativeDistributionPackageCreateRequest | AlternativeDistributionPackage representation

    try:
        api_response = api_instance.alternative_distribution_packages_create_instance(alternative_distribution_package_create_request)
        print("The response of AlternativeDistributionPackagesApi->alternative_distribution_packages_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlternativeDistributionPackagesApi->alternative_distribution_packages_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **alternative_distribution_package_create_request** | [**AlternativeDistributionPackageCreateRequest**](AlternativeDistributionPackageCreateRequest.md)| AlternativeDistributionPackage representation | 

### Return type

[**AlternativeDistributionPackageResponse**](AlternativeDistributionPackageResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**422** | Unprocessable request entity error(s) |  -  |
**201** | Single AlternativeDistributionPackage |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **alternative_distribution_packages_get_instance**
> AlternativeDistributionPackageResponse alternative_distribution_packages_get_instance(id, fields_alternative_distribution_packages=fields_alternative_distribution_packages, fields_alternative_distribution_package_versions=fields_alternative_distribution_package_versions, include=include, limit_versions=limit_versions)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.alternative_distribution_package_response import AlternativeDistributionPackageResponse
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
    api_instance = openapi_client.AlternativeDistributionPackagesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_alternative_distribution_packages = ['fields_alternative_distribution_packages_example'] # List[str] | the fields to include for returned resources of type alternativeDistributionPackages (optional)
    fields_alternative_distribution_package_versions = ['fields_alternative_distribution_package_versions_example'] # List[str] | the fields to include for returned resources of type alternativeDistributionPackageVersions (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_versions = 56 # int | maximum number of related versions returned (when they are included) (optional)

    try:
        api_response = api_instance.alternative_distribution_packages_get_instance(id, fields_alternative_distribution_packages=fields_alternative_distribution_packages, fields_alternative_distribution_package_versions=fields_alternative_distribution_package_versions, include=include, limit_versions=limit_versions)
        print("The response of AlternativeDistributionPackagesApi->alternative_distribution_packages_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlternativeDistributionPackagesApi->alternative_distribution_packages_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_alternative_distribution_packages** | [**List[str]**](str.md)| the fields to include for returned resources of type alternativeDistributionPackages | [optional] 
 **fields_alternative_distribution_package_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type alternativeDistributionPackageVersions | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_versions** | **int**| maximum number of related versions returned (when they are included) | [optional] 

### Return type

[**AlternativeDistributionPackageResponse**](AlternativeDistributionPackageResponse.md)

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
**200** | Single AlternativeDistributionPackage |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **alternative_distribution_packages_versions_get_to_many_related**
> AlternativeDistributionPackageVersionsResponse alternative_distribution_packages_versions_get_to_many_related(id, filter_state=filter_state, fields_alternative_distribution_package_versions=fields_alternative_distribution_package_versions, fields_alternative_distribution_package_variants=fields_alternative_distribution_package_variants, fields_alternative_distribution_package_deltas=fields_alternative_distribution_package_deltas, fields_alternative_distribution_packages=fields_alternative_distribution_packages, limit=limit, include=include, limit_variants=limit_variants, limit_deltas=limit_deltas)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.alternative_distribution_package_versions_response import AlternativeDistributionPackageVersionsResponse
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
    api_instance = openapi_client.AlternativeDistributionPackagesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_state = ['filter_state_example'] # List[str] | filter by attribute 'state' (optional)
    fields_alternative_distribution_package_versions = ['fields_alternative_distribution_package_versions_example'] # List[str] | the fields to include for returned resources of type alternativeDistributionPackageVersions (optional)
    fields_alternative_distribution_package_variants = ['fields_alternative_distribution_package_variants_example'] # List[str] | the fields to include for returned resources of type alternativeDistributionPackageVariants (optional)
    fields_alternative_distribution_package_deltas = ['fields_alternative_distribution_package_deltas_example'] # List[str] | the fields to include for returned resources of type alternativeDistributionPackageDeltas (optional)
    fields_alternative_distribution_packages = ['fields_alternative_distribution_packages_example'] # List[str] | the fields to include for returned resources of type alternativeDistributionPackages (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_variants = 56 # int | maximum number of related variants returned (when they are included) (optional)
    limit_deltas = 56 # int | maximum number of related deltas returned (when they are included) (optional)

    try:
        api_response = api_instance.alternative_distribution_packages_versions_get_to_many_related(id, filter_state=filter_state, fields_alternative_distribution_package_versions=fields_alternative_distribution_package_versions, fields_alternative_distribution_package_variants=fields_alternative_distribution_package_variants, fields_alternative_distribution_package_deltas=fields_alternative_distribution_package_deltas, fields_alternative_distribution_packages=fields_alternative_distribution_packages, limit=limit, include=include, limit_variants=limit_variants, limit_deltas=limit_deltas)
        print("The response of AlternativeDistributionPackagesApi->alternative_distribution_packages_versions_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlternativeDistributionPackagesApi->alternative_distribution_packages_versions_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_state** | [**List[str]**](str.md)| filter by attribute &#39;state&#39; | [optional] 
 **fields_alternative_distribution_package_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type alternativeDistributionPackageVersions | [optional] 
 **fields_alternative_distribution_package_variants** | [**List[str]**](str.md)| the fields to include for returned resources of type alternativeDistributionPackageVariants | [optional] 
 **fields_alternative_distribution_package_deltas** | [**List[str]**](str.md)| the fields to include for returned resources of type alternativeDistributionPackageDeltas | [optional] 
 **fields_alternative_distribution_packages** | [**List[str]**](str.md)| the fields to include for returned resources of type alternativeDistributionPackages | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_variants** | **int**| maximum number of related variants returned (when they are included) | [optional] 
 **limit_deltas** | **int**| maximum number of related deltas returned (when they are included) | [optional] 

### Return type

[**AlternativeDistributionPackageVersionsResponse**](AlternativeDistributionPackageVersionsResponse.md)

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
**200** | List of AlternativeDistributionPackageVersions |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **alternative_distribution_packages_versions_get_to_many_relationship**
> AlternativeDistributionPackageVersionsLinkagesResponse alternative_distribution_packages_versions_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.alternative_distribution_package_versions_linkages_response import AlternativeDistributionPackageVersionsLinkagesResponse
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
    api_instance = openapi_client.AlternativeDistributionPackagesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.alternative_distribution_packages_versions_get_to_many_relationship(id, limit=limit)
        print("The response of AlternativeDistributionPackagesApi->alternative_distribution_packages_versions_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlternativeDistributionPackagesApi->alternative_distribution_packages_versions_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AlternativeDistributionPackageVersionsLinkagesResponse**](AlternativeDistributionPackageVersionsLinkagesResponse.md)

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

