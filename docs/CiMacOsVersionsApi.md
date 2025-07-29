# openapi_client.CiMacOsVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ci_mac_os_versions_get_collection**](CiMacOsVersionsApi.md#ci_mac_os_versions_get_collection) | **GET** /v1/ciMacOsVersions | 
[**ci_mac_os_versions_get_instance**](CiMacOsVersionsApi.md#ci_mac_os_versions_get_instance) | **GET** /v1/ciMacOsVersions/{id} | 
[**ci_mac_os_versions_xcode_versions_get_to_many_related**](CiMacOsVersionsApi.md#ci_mac_os_versions_xcode_versions_get_to_many_related) | **GET** /v1/ciMacOsVersions/{id}/xcodeVersions | 
[**ci_mac_os_versions_xcode_versions_get_to_many_relationship**](CiMacOsVersionsApi.md#ci_mac_os_versions_xcode_versions_get_to_many_relationship) | **GET** /v1/ciMacOsVersions/{id}/relationships/xcodeVersions | 


# **ci_mac_os_versions_get_collection**
> CiMacOsVersionsResponse ci_mac_os_versions_get_collection(fields_ci_mac_os_versions=fields_ci_mac_os_versions, fields_ci_xcode_versions=fields_ci_xcode_versions, limit=limit, include=include, limit_xcode_versions=limit_xcode_versions)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_mac_os_versions_response import CiMacOsVersionsResponse
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
    api_instance = openapi_client.CiMacOsVersionsApi(api_client)
    fields_ci_mac_os_versions = ['fields_ci_mac_os_versions_example'] # List[str] | the fields to include for returned resources of type ciMacOsVersions (optional)
    fields_ci_xcode_versions = ['fields_ci_xcode_versions_example'] # List[str] | the fields to include for returned resources of type ciXcodeVersions (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_xcode_versions = 56 # int | maximum number of related xcodeVersions returned (when they are included) (optional)

    try:
        api_response = api_instance.ci_mac_os_versions_get_collection(fields_ci_mac_os_versions=fields_ci_mac_os_versions, fields_ci_xcode_versions=fields_ci_xcode_versions, limit=limit, include=include, limit_xcode_versions=limit_xcode_versions)
        print("The response of CiMacOsVersionsApi->ci_mac_os_versions_get_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiMacOsVersionsApi->ci_mac_os_versions_get_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fields_ci_mac_os_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type ciMacOsVersions | [optional] 
 **fields_ci_xcode_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type ciXcodeVersions | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_xcode_versions** | **int**| maximum number of related xcodeVersions returned (when they are included) | [optional] 

### Return type

[**CiMacOsVersionsResponse**](CiMacOsVersionsResponse.md)

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
**200** | List of CiMacOsVersions |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_mac_os_versions_get_instance**
> CiMacOsVersionResponse ci_mac_os_versions_get_instance(id, fields_ci_mac_os_versions=fields_ci_mac_os_versions, fields_ci_xcode_versions=fields_ci_xcode_versions, include=include, limit_xcode_versions=limit_xcode_versions)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_mac_os_version_response import CiMacOsVersionResponse
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
    api_instance = openapi_client.CiMacOsVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_ci_mac_os_versions = ['fields_ci_mac_os_versions_example'] # List[str] | the fields to include for returned resources of type ciMacOsVersions (optional)
    fields_ci_xcode_versions = ['fields_ci_xcode_versions_example'] # List[str] | the fields to include for returned resources of type ciXcodeVersions (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_xcode_versions = 56 # int | maximum number of related xcodeVersions returned (when they are included) (optional)

    try:
        api_response = api_instance.ci_mac_os_versions_get_instance(id, fields_ci_mac_os_versions=fields_ci_mac_os_versions, fields_ci_xcode_versions=fields_ci_xcode_versions, include=include, limit_xcode_versions=limit_xcode_versions)
        print("The response of CiMacOsVersionsApi->ci_mac_os_versions_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiMacOsVersionsApi->ci_mac_os_versions_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_ci_mac_os_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type ciMacOsVersions | [optional] 
 **fields_ci_xcode_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type ciXcodeVersions | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_xcode_versions** | **int**| maximum number of related xcodeVersions returned (when they are included) | [optional] 

### Return type

[**CiMacOsVersionResponse**](CiMacOsVersionResponse.md)

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
**200** | Single CiMacOsVersion |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_mac_os_versions_xcode_versions_get_to_many_related**
> CiXcodeVersionsResponse ci_mac_os_versions_xcode_versions_get_to_many_related(id, fields_ci_xcode_versions=fields_ci_xcode_versions, fields_ci_mac_os_versions=fields_ci_mac_os_versions, limit=limit, include=include, limit_mac_os_versions=limit_mac_os_versions)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_xcode_versions_response import CiXcodeVersionsResponse
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
    api_instance = openapi_client.CiMacOsVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_ci_xcode_versions = ['fields_ci_xcode_versions_example'] # List[str] | the fields to include for returned resources of type ciXcodeVersions (optional)
    fields_ci_mac_os_versions = ['fields_ci_mac_os_versions_example'] # List[str] | the fields to include for returned resources of type ciMacOsVersions (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_mac_os_versions = 56 # int | maximum number of related macOsVersions returned (when they are included) (optional)

    try:
        api_response = api_instance.ci_mac_os_versions_xcode_versions_get_to_many_related(id, fields_ci_xcode_versions=fields_ci_xcode_versions, fields_ci_mac_os_versions=fields_ci_mac_os_versions, limit=limit, include=include, limit_mac_os_versions=limit_mac_os_versions)
        print("The response of CiMacOsVersionsApi->ci_mac_os_versions_xcode_versions_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiMacOsVersionsApi->ci_mac_os_versions_xcode_versions_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_ci_xcode_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type ciXcodeVersions | [optional] 
 **fields_ci_mac_os_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type ciMacOsVersions | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_mac_os_versions** | **int**| maximum number of related macOsVersions returned (when they are included) | [optional] 

### Return type

[**CiXcodeVersionsResponse**](CiXcodeVersionsResponse.md)

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
**200** | List of CiXcodeVersions |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_mac_os_versions_xcode_versions_get_to_many_relationship**
> CiMacOsVersionXcodeVersionsLinkagesResponse ci_mac_os_versions_xcode_versions_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_mac_os_version_xcode_versions_linkages_response import CiMacOsVersionXcodeVersionsLinkagesResponse
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
    api_instance = openapi_client.CiMacOsVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.ci_mac_os_versions_xcode_versions_get_to_many_relationship(id, limit=limit)
        print("The response of CiMacOsVersionsApi->ci_mac_os_versions_xcode_versions_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiMacOsVersionsApi->ci_mac_os_versions_xcode_versions_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**CiMacOsVersionXcodeVersionsLinkagesResponse**](CiMacOsVersionXcodeVersionsLinkagesResponse.md)

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

