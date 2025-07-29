# openapi_client.BackgroundAssetVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**background_asset_versions_background_asset_upload_files_get_to_many_related**](BackgroundAssetVersionsApi.md#background_asset_versions_background_asset_upload_files_get_to_many_related) | **GET** /v1/backgroundAssetVersions/{id}/backgroundAssetUploadFiles | 
[**background_asset_versions_background_asset_upload_files_get_to_many_relationship**](BackgroundAssetVersionsApi.md#background_asset_versions_background_asset_upload_files_get_to_many_relationship) | **GET** /v1/backgroundAssetVersions/{id}/relationships/backgroundAssetUploadFiles | 
[**background_asset_versions_create_instance**](BackgroundAssetVersionsApi.md#background_asset_versions_create_instance) | **POST** /v1/backgroundAssetVersions | 
[**background_asset_versions_get_instance**](BackgroundAssetVersionsApi.md#background_asset_versions_get_instance) | **GET** /v1/backgroundAssetVersions/{id} | 


# **background_asset_versions_background_asset_upload_files_get_to_many_related**
> BackgroundAssetUploadFilesResponse background_asset_versions_background_asset_upload_files_get_to_many_related(id, fields_background_asset_upload_files=fields_background_asset_upload_files, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.background_asset_upload_files_response import BackgroundAssetUploadFilesResponse
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
    api_instance = openapi_client.BackgroundAssetVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_background_asset_upload_files = ['fields_background_asset_upload_files_example'] # List[str] | the fields to include for returned resources of type backgroundAssetUploadFiles (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.background_asset_versions_background_asset_upload_files_get_to_many_related(id, fields_background_asset_upload_files=fields_background_asset_upload_files, limit=limit)
        print("The response of BackgroundAssetVersionsApi->background_asset_versions_background_asset_upload_files_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BackgroundAssetVersionsApi->background_asset_versions_background_asset_upload_files_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_background_asset_upload_files** | [**List[str]**](str.md)| the fields to include for returned resources of type backgroundAssetUploadFiles | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**BackgroundAssetUploadFilesResponse**](BackgroundAssetUploadFilesResponse.md)

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
**200** | List of BackgroundAssetUploadFiles |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **background_asset_versions_background_asset_upload_files_get_to_many_relationship**
> BackgroundAssetVersionBackgroundAssetUploadFilesLinkagesResponse background_asset_versions_background_asset_upload_files_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.background_asset_version_background_asset_upload_files_linkages_response import BackgroundAssetVersionBackgroundAssetUploadFilesLinkagesResponse
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
    api_instance = openapi_client.BackgroundAssetVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.background_asset_versions_background_asset_upload_files_get_to_many_relationship(id, limit=limit)
        print("The response of BackgroundAssetVersionsApi->background_asset_versions_background_asset_upload_files_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BackgroundAssetVersionsApi->background_asset_versions_background_asset_upload_files_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**BackgroundAssetVersionBackgroundAssetUploadFilesLinkagesResponse**](BackgroundAssetVersionBackgroundAssetUploadFilesLinkagesResponse.md)

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

# **background_asset_versions_create_instance**
> BackgroundAssetVersionResponse background_asset_versions_create_instance(background_asset_version_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.background_asset_version_create_request import BackgroundAssetVersionCreateRequest
from openapi_client.models.background_asset_version_response import BackgroundAssetVersionResponse
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
    api_instance = openapi_client.BackgroundAssetVersionsApi(api_client)
    background_asset_version_create_request = openapi_client.BackgroundAssetVersionCreateRequest() # BackgroundAssetVersionCreateRequest | BackgroundAssetVersion representation

    try:
        api_response = api_instance.background_asset_versions_create_instance(background_asset_version_create_request)
        print("The response of BackgroundAssetVersionsApi->background_asset_versions_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BackgroundAssetVersionsApi->background_asset_versions_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **background_asset_version_create_request** | [**BackgroundAssetVersionCreateRequest**](BackgroundAssetVersionCreateRequest.md)| BackgroundAssetVersion representation | 

### Return type

[**BackgroundAssetVersionResponse**](BackgroundAssetVersionResponse.md)

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
**201** | Single BackgroundAssetVersion |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **background_asset_versions_get_instance**
> BackgroundAssetVersionResponse background_asset_versions_get_instance(id, fields_background_asset_versions=fields_background_asset_versions, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.background_asset_version_response import BackgroundAssetVersionResponse
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
    api_instance = openapi_client.BackgroundAssetVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_background_asset_versions = ['fields_background_asset_versions_example'] # List[str] | the fields to include for returned resources of type backgroundAssetVersions (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.background_asset_versions_get_instance(id, fields_background_asset_versions=fields_background_asset_versions, include=include)
        print("The response of BackgroundAssetVersionsApi->background_asset_versions_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BackgroundAssetVersionsApi->background_asset_versions_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_background_asset_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type backgroundAssetVersions | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**BackgroundAssetVersionResponse**](BackgroundAssetVersionResponse.md)

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
**200** | Single BackgroundAssetVersion |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

