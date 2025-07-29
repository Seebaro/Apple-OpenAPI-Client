# openapi_client.ProfilesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**profiles_bundle_id_get_to_one_related**](ProfilesApi.md#profiles_bundle_id_get_to_one_related) | **GET** /v1/profiles/{id}/bundleId | 
[**profiles_bundle_id_get_to_one_relationship**](ProfilesApi.md#profiles_bundle_id_get_to_one_relationship) | **GET** /v1/profiles/{id}/relationships/bundleId | 
[**profiles_certificates_get_to_many_related**](ProfilesApi.md#profiles_certificates_get_to_many_related) | **GET** /v1/profiles/{id}/certificates | 
[**profiles_certificates_get_to_many_relationship**](ProfilesApi.md#profiles_certificates_get_to_many_relationship) | **GET** /v1/profiles/{id}/relationships/certificates | 
[**profiles_create_instance**](ProfilesApi.md#profiles_create_instance) | **POST** /v1/profiles | 
[**profiles_delete_instance**](ProfilesApi.md#profiles_delete_instance) | **DELETE** /v1/profiles/{id} | 
[**profiles_devices_get_to_many_related**](ProfilesApi.md#profiles_devices_get_to_many_related) | **GET** /v1/profiles/{id}/devices | 
[**profiles_devices_get_to_many_relationship**](ProfilesApi.md#profiles_devices_get_to_many_relationship) | **GET** /v1/profiles/{id}/relationships/devices | 
[**profiles_get_collection**](ProfilesApi.md#profiles_get_collection) | **GET** /v1/profiles | 
[**profiles_get_instance**](ProfilesApi.md#profiles_get_instance) | **GET** /v1/profiles/{id} | 


# **profiles_bundle_id_get_to_one_related**
> BundleIdWithoutIncludesResponse profiles_bundle_id_get_to_one_related(id, fields_bundle_ids=fields_bundle_ids)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.bundle_id_without_includes_response import BundleIdWithoutIncludesResponse
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
    api_instance = openapi_client.ProfilesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_bundle_ids = ['fields_bundle_ids_example'] # List[str] | the fields to include for returned resources of type bundleIds (optional)

    try:
        api_response = api_instance.profiles_bundle_id_get_to_one_related(id, fields_bundle_ids=fields_bundle_ids)
        print("The response of ProfilesApi->profiles_bundle_id_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProfilesApi->profiles_bundle_id_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_bundle_ids** | [**List[str]**](str.md)| the fields to include for returned resources of type bundleIds | [optional] 

### Return type

[**BundleIdWithoutIncludesResponse**](BundleIdWithoutIncludesResponse.md)

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
**200** | Single BundleId with get |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **profiles_bundle_id_get_to_one_relationship**
> ProfileBundleIdLinkageResponse profiles_bundle_id_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.profile_bundle_id_linkage_response import ProfileBundleIdLinkageResponse
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
    api_instance = openapi_client.ProfilesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.profiles_bundle_id_get_to_one_relationship(id)
        print("The response of ProfilesApi->profiles_bundle_id_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProfilesApi->profiles_bundle_id_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**ProfileBundleIdLinkageResponse**](ProfileBundleIdLinkageResponse.md)

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

# **profiles_certificates_get_to_many_related**
> CertificatesWithoutIncludesResponse profiles_certificates_get_to_many_related(id, fields_certificates=fields_certificates, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.certificates_without_includes_response import CertificatesWithoutIncludesResponse
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
    api_instance = openapi_client.ProfilesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_certificates = ['fields_certificates_example'] # List[str] | the fields to include for returned resources of type certificates (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.profiles_certificates_get_to_many_related(id, fields_certificates=fields_certificates, limit=limit)
        print("The response of ProfilesApi->profiles_certificates_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProfilesApi->profiles_certificates_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_certificates** | [**List[str]**](str.md)| the fields to include for returned resources of type certificates | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**CertificatesWithoutIncludesResponse**](CertificatesWithoutIncludesResponse.md)

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
**200** | List of Certificates with get |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **profiles_certificates_get_to_many_relationship**
> ProfileCertificatesLinkagesResponse profiles_certificates_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.profile_certificates_linkages_response import ProfileCertificatesLinkagesResponse
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
    api_instance = openapi_client.ProfilesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.profiles_certificates_get_to_many_relationship(id, limit=limit)
        print("The response of ProfilesApi->profiles_certificates_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProfilesApi->profiles_certificates_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**ProfileCertificatesLinkagesResponse**](ProfileCertificatesLinkagesResponse.md)

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

# **profiles_create_instance**
> ProfileResponse profiles_create_instance(profile_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.profile_create_request import ProfileCreateRequest
from openapi_client.models.profile_response import ProfileResponse
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
    api_instance = openapi_client.ProfilesApi(api_client)
    profile_create_request = openapi_client.ProfileCreateRequest() # ProfileCreateRequest | Profile representation

    try:
        api_response = api_instance.profiles_create_instance(profile_create_request)
        print("The response of ProfilesApi->profiles_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProfilesApi->profiles_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_create_request** | [**ProfileCreateRequest**](ProfileCreateRequest.md)| Profile representation | 

### Return type

[**ProfileResponse**](ProfileResponse.md)

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
**201** | Single Profile |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **profiles_delete_instance**
> profiles_delete_instance(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
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
    api_instance = openapi_client.ProfilesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.profiles_delete_instance(id)
    except Exception as e:
        print("Exception when calling ProfilesApi->profiles_delete_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

void (empty response body)

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
**409** | Request entity error(s) |  -  |
**204** | Success (no content) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **profiles_devices_get_to_many_related**
> DevicesWithoutIncludesResponse profiles_devices_get_to_many_related(id, fields_devices=fields_devices, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.devices_without_includes_response import DevicesWithoutIncludesResponse
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
    api_instance = openapi_client.ProfilesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_devices = ['fields_devices_example'] # List[str] | the fields to include for returned resources of type devices (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.profiles_devices_get_to_many_related(id, fields_devices=fields_devices, limit=limit)
        print("The response of ProfilesApi->profiles_devices_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProfilesApi->profiles_devices_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_devices** | [**List[str]**](str.md)| the fields to include for returned resources of type devices | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**DevicesWithoutIncludesResponse**](DevicesWithoutIncludesResponse.md)

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
**200** | List of Devices with get |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **profiles_devices_get_to_many_relationship**
> ProfileDevicesLinkagesResponse profiles_devices_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.profile_devices_linkages_response import ProfileDevicesLinkagesResponse
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
    api_instance = openapi_client.ProfilesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.profiles_devices_get_to_many_relationship(id, limit=limit)
        print("The response of ProfilesApi->profiles_devices_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProfilesApi->profiles_devices_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**ProfileDevicesLinkagesResponse**](ProfileDevicesLinkagesResponse.md)

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

# **profiles_get_collection**
> ProfilesResponse profiles_get_collection(filter_name=filter_name, filter_profile_type=filter_profile_type, filter_profile_state=filter_profile_state, filter_id=filter_id, sort=sort, fields_profiles=fields_profiles, fields_bundle_ids=fields_bundle_ids, fields_devices=fields_devices, fields_certificates=fields_certificates, limit=limit, include=include, limit_certificates=limit_certificates, limit_devices=limit_devices)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.profiles_response import ProfilesResponse
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
    api_instance = openapi_client.ProfilesApi(api_client)
    filter_name = ['filter_name_example'] # List[str] | filter by attribute 'name' (optional)
    filter_profile_type = ['filter_profile_type_example'] # List[str] | filter by attribute 'profileType' (optional)
    filter_profile_state = ['filter_profile_state_example'] # List[str] | filter by attribute 'profileState' (optional)
    filter_id = ['filter_id_example'] # List[str] | filter by id(s) (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; resources will be sorted as specified (optional)
    fields_profiles = ['fields_profiles_example'] # List[str] | the fields to include for returned resources of type profiles (optional)
    fields_bundle_ids = ['fields_bundle_ids_example'] # List[str] | the fields to include for returned resources of type bundleIds (optional)
    fields_devices = ['fields_devices_example'] # List[str] | the fields to include for returned resources of type devices (optional)
    fields_certificates = ['fields_certificates_example'] # List[str] | the fields to include for returned resources of type certificates (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_certificates = 56 # int | maximum number of related certificates returned (when they are included) (optional)
    limit_devices = 56 # int | maximum number of related devices returned (when they are included) (optional)

    try:
        api_response = api_instance.profiles_get_collection(filter_name=filter_name, filter_profile_type=filter_profile_type, filter_profile_state=filter_profile_state, filter_id=filter_id, sort=sort, fields_profiles=fields_profiles, fields_bundle_ids=fields_bundle_ids, fields_devices=fields_devices, fields_certificates=fields_certificates, limit=limit, include=include, limit_certificates=limit_certificates, limit_devices=limit_devices)
        print("The response of ProfilesApi->profiles_get_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProfilesApi->profiles_get_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter_name** | [**List[str]**](str.md)| filter by attribute &#39;name&#39; | [optional] 
 **filter_profile_type** | [**List[str]**](str.md)| filter by attribute &#39;profileType&#39; | [optional] 
 **filter_profile_state** | [**List[str]**](str.md)| filter by attribute &#39;profileState&#39; | [optional] 
 **filter_id** | [**List[str]**](str.md)| filter by id(s) | [optional] 
 **sort** | [**List[str]**](str.md)| comma-separated list of sort expressions; resources will be sorted as specified | [optional] 
 **fields_profiles** | [**List[str]**](str.md)| the fields to include for returned resources of type profiles | [optional] 
 **fields_bundle_ids** | [**List[str]**](str.md)| the fields to include for returned resources of type bundleIds | [optional] 
 **fields_devices** | [**List[str]**](str.md)| the fields to include for returned resources of type devices | [optional] 
 **fields_certificates** | [**List[str]**](str.md)| the fields to include for returned resources of type certificates | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_certificates** | **int**| maximum number of related certificates returned (when they are included) | [optional] 
 **limit_devices** | **int**| maximum number of related devices returned (when they are included) | [optional] 

### Return type

[**ProfilesResponse**](ProfilesResponse.md)

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
**200** | List of Profiles |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **profiles_get_instance**
> ProfileResponse profiles_get_instance(id, fields_profiles=fields_profiles, fields_bundle_ids=fields_bundle_ids, fields_devices=fields_devices, fields_certificates=fields_certificates, include=include, limit_certificates=limit_certificates, limit_devices=limit_devices)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.profile_response import ProfileResponse
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
    api_instance = openapi_client.ProfilesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_profiles = ['fields_profiles_example'] # List[str] | the fields to include for returned resources of type profiles (optional)
    fields_bundle_ids = ['fields_bundle_ids_example'] # List[str] | the fields to include for returned resources of type bundleIds (optional)
    fields_devices = ['fields_devices_example'] # List[str] | the fields to include for returned resources of type devices (optional)
    fields_certificates = ['fields_certificates_example'] # List[str] | the fields to include for returned resources of type certificates (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_certificates = 56 # int | maximum number of related certificates returned (when they are included) (optional)
    limit_devices = 56 # int | maximum number of related devices returned (when they are included) (optional)

    try:
        api_response = api_instance.profiles_get_instance(id, fields_profiles=fields_profiles, fields_bundle_ids=fields_bundle_ids, fields_devices=fields_devices, fields_certificates=fields_certificates, include=include, limit_certificates=limit_certificates, limit_devices=limit_devices)
        print("The response of ProfilesApi->profiles_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProfilesApi->profiles_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_profiles** | [**List[str]**](str.md)| the fields to include for returned resources of type profiles | [optional] 
 **fields_bundle_ids** | [**List[str]**](str.md)| the fields to include for returned resources of type bundleIds | [optional] 
 **fields_devices** | [**List[str]**](str.md)| the fields to include for returned resources of type devices | [optional] 
 **fields_certificates** | [**List[str]**](str.md)| the fields to include for returned resources of type certificates | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_certificates** | **int**| maximum number of related certificates returned (when they are included) | [optional] 
 **limit_devices** | **int**| maximum number of related devices returned (when they are included) | [optional] 

### Return type

[**ProfileResponse**](ProfileResponse.md)

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
**200** | Single Profile |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

