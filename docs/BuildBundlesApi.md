# openapi_client.BuildBundlesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**build_bundles_app_clip_domain_cache_status_get_to_one_related**](BuildBundlesApi.md#build_bundles_app_clip_domain_cache_status_get_to_one_related) | **GET** /v1/buildBundles/{id}/appClipDomainCacheStatus | 
[**build_bundles_app_clip_domain_cache_status_get_to_one_relationship**](BuildBundlesApi.md#build_bundles_app_clip_domain_cache_status_get_to_one_relationship) | **GET** /v1/buildBundles/{id}/relationships/appClipDomainCacheStatus | 
[**build_bundles_app_clip_domain_debug_status_get_to_one_related**](BuildBundlesApi.md#build_bundles_app_clip_domain_debug_status_get_to_one_related) | **GET** /v1/buildBundles/{id}/appClipDomainDebugStatus | 
[**build_bundles_app_clip_domain_debug_status_get_to_one_relationship**](BuildBundlesApi.md#build_bundles_app_clip_domain_debug_status_get_to_one_relationship) | **GET** /v1/buildBundles/{id}/relationships/appClipDomainDebugStatus | 
[**build_bundles_beta_app_clip_invocations_get_to_many_related**](BuildBundlesApi.md#build_bundles_beta_app_clip_invocations_get_to_many_related) | **GET** /v1/buildBundles/{id}/betaAppClipInvocations | 
[**build_bundles_beta_app_clip_invocations_get_to_many_relationship**](BuildBundlesApi.md#build_bundles_beta_app_clip_invocations_get_to_many_relationship) | **GET** /v1/buildBundles/{id}/relationships/betaAppClipInvocations | 
[**build_bundles_build_bundle_file_sizes_get_to_many_related**](BuildBundlesApi.md#build_bundles_build_bundle_file_sizes_get_to_many_related) | **GET** /v1/buildBundles/{id}/buildBundleFileSizes | 
[**build_bundles_build_bundle_file_sizes_get_to_many_relationship**](BuildBundlesApi.md#build_bundles_build_bundle_file_sizes_get_to_many_relationship) | **GET** /v1/buildBundles/{id}/relationships/buildBundleFileSizes | 


# **build_bundles_app_clip_domain_cache_status_get_to_one_related**
> AppClipDomainStatusResponse build_bundles_app_clip_domain_cache_status_get_to_one_related(id, fields_app_clip_domain_statuses=fields_app_clip_domain_statuses)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_domain_status_response import AppClipDomainStatusResponse
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
    api_instance = openapi_client.BuildBundlesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_clip_domain_statuses = ['fields_app_clip_domain_statuses_example'] # List[str] | the fields to include for returned resources of type appClipDomainStatuses (optional)

    try:
        api_response = api_instance.build_bundles_app_clip_domain_cache_status_get_to_one_related(id, fields_app_clip_domain_statuses=fields_app_clip_domain_statuses)
        print("The response of BuildBundlesApi->build_bundles_app_clip_domain_cache_status_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildBundlesApi->build_bundles_app_clip_domain_cache_status_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_clip_domain_statuses** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipDomainStatuses | [optional] 

### Return type

[**AppClipDomainStatusResponse**](AppClipDomainStatusResponse.md)

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
**200** | Single AppClipDomainStatus |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **build_bundles_app_clip_domain_cache_status_get_to_one_relationship**
> BuildBundleAppClipDomainCacheStatusLinkageResponse build_bundles_app_clip_domain_cache_status_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_bundle_app_clip_domain_cache_status_linkage_response import BuildBundleAppClipDomainCacheStatusLinkageResponse
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
    api_instance = openapi_client.BuildBundlesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.build_bundles_app_clip_domain_cache_status_get_to_one_relationship(id)
        print("The response of BuildBundlesApi->build_bundles_app_clip_domain_cache_status_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildBundlesApi->build_bundles_app_clip_domain_cache_status_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**BuildBundleAppClipDomainCacheStatusLinkageResponse**](BuildBundleAppClipDomainCacheStatusLinkageResponse.md)

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
**200** | Related linkage |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **build_bundles_app_clip_domain_debug_status_get_to_one_related**
> AppClipDomainStatusResponse build_bundles_app_clip_domain_debug_status_get_to_one_related(id, fields_app_clip_domain_statuses=fields_app_clip_domain_statuses)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_domain_status_response import AppClipDomainStatusResponse
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
    api_instance = openapi_client.BuildBundlesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_clip_domain_statuses = ['fields_app_clip_domain_statuses_example'] # List[str] | the fields to include for returned resources of type appClipDomainStatuses (optional)

    try:
        api_response = api_instance.build_bundles_app_clip_domain_debug_status_get_to_one_related(id, fields_app_clip_domain_statuses=fields_app_clip_domain_statuses)
        print("The response of BuildBundlesApi->build_bundles_app_clip_domain_debug_status_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildBundlesApi->build_bundles_app_clip_domain_debug_status_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_clip_domain_statuses** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipDomainStatuses | [optional] 

### Return type

[**AppClipDomainStatusResponse**](AppClipDomainStatusResponse.md)

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
**200** | Single AppClipDomainStatus |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **build_bundles_app_clip_domain_debug_status_get_to_one_relationship**
> BuildBundleAppClipDomainDebugStatusLinkageResponse build_bundles_app_clip_domain_debug_status_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_bundle_app_clip_domain_debug_status_linkage_response import BuildBundleAppClipDomainDebugStatusLinkageResponse
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
    api_instance = openapi_client.BuildBundlesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.build_bundles_app_clip_domain_debug_status_get_to_one_relationship(id)
        print("The response of BuildBundlesApi->build_bundles_app_clip_domain_debug_status_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildBundlesApi->build_bundles_app_clip_domain_debug_status_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**BuildBundleAppClipDomainDebugStatusLinkageResponse**](BuildBundleAppClipDomainDebugStatusLinkageResponse.md)

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
**200** | Related linkage |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **build_bundles_beta_app_clip_invocations_get_to_many_related**
> BetaAppClipInvocationsResponse build_bundles_beta_app_clip_invocations_get_to_many_related(id, fields_beta_app_clip_invocations=fields_beta_app_clip_invocations, fields_beta_app_clip_invocation_localizations=fields_beta_app_clip_invocation_localizations, limit=limit, include=include, limit_beta_app_clip_invocation_localizations=limit_beta_app_clip_invocation_localizations)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.beta_app_clip_invocations_response import BetaAppClipInvocationsResponse
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
    api_instance = openapi_client.BuildBundlesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_beta_app_clip_invocations = ['fields_beta_app_clip_invocations_example'] # List[str] | the fields to include for returned resources of type betaAppClipInvocations (optional)
    fields_beta_app_clip_invocation_localizations = ['fields_beta_app_clip_invocation_localizations_example'] # List[str] | the fields to include for returned resources of type betaAppClipInvocationLocalizations (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_beta_app_clip_invocation_localizations = 56 # int | maximum number of related betaAppClipInvocationLocalizations returned (when they are included) (optional)

    try:
        api_response = api_instance.build_bundles_beta_app_clip_invocations_get_to_many_related(id, fields_beta_app_clip_invocations=fields_beta_app_clip_invocations, fields_beta_app_clip_invocation_localizations=fields_beta_app_clip_invocation_localizations, limit=limit, include=include, limit_beta_app_clip_invocation_localizations=limit_beta_app_clip_invocation_localizations)
        print("The response of BuildBundlesApi->build_bundles_beta_app_clip_invocations_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildBundlesApi->build_bundles_beta_app_clip_invocations_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_beta_app_clip_invocations** | [**List[str]**](str.md)| the fields to include for returned resources of type betaAppClipInvocations | [optional] 
 **fields_beta_app_clip_invocation_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type betaAppClipInvocationLocalizations | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_beta_app_clip_invocation_localizations** | **int**| maximum number of related betaAppClipInvocationLocalizations returned (when they are included) | [optional] 

### Return type

[**BetaAppClipInvocationsResponse**](BetaAppClipInvocationsResponse.md)

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
**200** | List of BetaAppClipInvocations |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **build_bundles_beta_app_clip_invocations_get_to_many_relationship**
> BuildBundleBetaAppClipInvocationsLinkagesResponse build_bundles_beta_app_clip_invocations_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_bundle_beta_app_clip_invocations_linkages_response import BuildBundleBetaAppClipInvocationsLinkagesResponse
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
    api_instance = openapi_client.BuildBundlesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.build_bundles_beta_app_clip_invocations_get_to_many_relationship(id, limit=limit)
        print("The response of BuildBundlesApi->build_bundles_beta_app_clip_invocations_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildBundlesApi->build_bundles_beta_app_clip_invocations_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**BuildBundleBetaAppClipInvocationsLinkagesResponse**](BuildBundleBetaAppClipInvocationsLinkagesResponse.md)

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

# **build_bundles_build_bundle_file_sizes_get_to_many_related**
> BuildBundleFileSizesResponse build_bundles_build_bundle_file_sizes_get_to_many_related(id, fields_build_bundle_file_sizes=fields_build_bundle_file_sizes, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_bundle_file_sizes_response import BuildBundleFileSizesResponse
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
    api_instance = openapi_client.BuildBundlesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_build_bundle_file_sizes = ['fields_build_bundle_file_sizes_example'] # List[str] | the fields to include for returned resources of type buildBundleFileSizes (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.build_bundles_build_bundle_file_sizes_get_to_many_related(id, fields_build_bundle_file_sizes=fields_build_bundle_file_sizes, limit=limit)
        print("The response of BuildBundlesApi->build_bundles_build_bundle_file_sizes_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildBundlesApi->build_bundles_build_bundle_file_sizes_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_build_bundle_file_sizes** | [**List[str]**](str.md)| the fields to include for returned resources of type buildBundleFileSizes | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**BuildBundleFileSizesResponse**](BuildBundleFileSizesResponse.md)

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
**200** | List of BuildBundleFileSizes |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **build_bundles_build_bundle_file_sizes_get_to_many_relationship**
> BuildBundleBuildBundleFileSizesLinkagesResponse build_bundles_build_bundle_file_sizes_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_bundle_build_bundle_file_sizes_linkages_response import BuildBundleBuildBundleFileSizesLinkagesResponse
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
    api_instance = openapi_client.BuildBundlesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.build_bundles_build_bundle_file_sizes_get_to_many_relationship(id, limit=limit)
        print("The response of BuildBundlesApi->build_bundles_build_bundle_file_sizes_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildBundlesApi->build_bundles_build_bundle_file_sizes_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**BuildBundleBuildBundleFileSizesLinkagesResponse**](BuildBundleBuildBundleFileSizesLinkagesResponse.md)

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

