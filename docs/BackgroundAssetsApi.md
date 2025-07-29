# openapi_client.BackgroundAssetsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**background_assets_create_instance**](BackgroundAssetsApi.md#background_assets_create_instance) | **POST** /v1/backgroundAssets | 
[**background_assets_get_instance**](BackgroundAssetsApi.md#background_assets_get_instance) | **GET** /v1/backgroundAssets/{id} | 
[**background_assets_versions_get_to_many_related**](BackgroundAssetsApi.md#background_assets_versions_get_to_many_related) | **GET** /v1/backgroundAssets/{id}/versions | 
[**background_assets_versions_get_to_many_relationship**](BackgroundAssetsApi.md#background_assets_versions_get_to_many_relationship) | **GET** /v1/backgroundAssets/{id}/relationships/versions | 


# **background_assets_create_instance**
> BackgroundAssetResponse background_assets_create_instance(background_asset_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.background_asset_create_request import BackgroundAssetCreateRequest
from openapi_client.models.background_asset_response import BackgroundAssetResponse
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
    api_instance = openapi_client.BackgroundAssetsApi(api_client)
    background_asset_create_request = openapi_client.BackgroundAssetCreateRequest() # BackgroundAssetCreateRequest | BackgroundAsset representation

    try:
        api_response = api_instance.background_assets_create_instance(background_asset_create_request)
        print("The response of BackgroundAssetsApi->background_assets_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BackgroundAssetsApi->background_assets_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **background_asset_create_request** | [**BackgroundAssetCreateRequest**](BackgroundAssetCreateRequest.md)| BackgroundAsset representation | 

### Return type

[**BackgroundAssetResponse**](BackgroundAssetResponse.md)

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
**201** | Single BackgroundAsset |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **background_assets_get_instance**
> BackgroundAssetResponse background_assets_get_instance(id, fields_background_assets=fields_background_assets, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.background_asset_response import BackgroundAssetResponse
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
    api_instance = openapi_client.BackgroundAssetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_background_assets = ['fields_background_assets_example'] # List[str] | the fields to include for returned resources of type backgroundAssets (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.background_assets_get_instance(id, fields_background_assets=fields_background_assets, include=include)
        print("The response of BackgroundAssetsApi->background_assets_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BackgroundAssetsApi->background_assets_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_background_assets** | [**List[str]**](str.md)| the fields to include for returned resources of type backgroundAssets | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**BackgroundAssetResponse**](BackgroundAssetResponse.md)

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
**200** | Single BackgroundAsset |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **background_assets_versions_get_to_many_related**
> BackgroundAssetVersionsResponse background_assets_versions_get_to_many_related(id, filter_state=filter_state, filter_version=filter_version, filter_internal_beta_release_state=filter_internal_beta_release_state, sort=sort, fields_background_asset_versions=fields_background_asset_versions, fields_background_asset_version_internal_beta_releases=fields_background_asset_version_internal_beta_releases, fields_background_asset_upload_files=fields_background_asset_upload_files, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.background_asset_versions_response import BackgroundAssetVersionsResponse
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
    api_instance = openapi_client.BackgroundAssetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_state = ['filter_state_example'] # List[str] | filter by attribute 'state' (optional)
    filter_version = ['filter_version_example'] # List[str] | filter by attribute 'version' (optional)
    filter_internal_beta_release_state = ['filter_internal_beta_release_state_example'] # List[str] | filter by attribute 'internalBetaRelease.state' (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; resources will be sorted as specified (optional)
    fields_background_asset_versions = ['fields_background_asset_versions_example'] # List[str] | the fields to include for returned resources of type backgroundAssetVersions (optional)
    fields_background_asset_version_internal_beta_releases = ['fields_background_asset_version_internal_beta_releases_example'] # List[str] | the fields to include for returned resources of type backgroundAssetVersionInternalBetaReleases (optional)
    fields_background_asset_upload_files = ['fields_background_asset_upload_files_example'] # List[str] | the fields to include for returned resources of type backgroundAssetUploadFiles (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.background_assets_versions_get_to_many_related(id, filter_state=filter_state, filter_version=filter_version, filter_internal_beta_release_state=filter_internal_beta_release_state, sort=sort, fields_background_asset_versions=fields_background_asset_versions, fields_background_asset_version_internal_beta_releases=fields_background_asset_version_internal_beta_releases, fields_background_asset_upload_files=fields_background_asset_upload_files, limit=limit, include=include)
        print("The response of BackgroundAssetsApi->background_assets_versions_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BackgroundAssetsApi->background_assets_versions_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_state** | [**List[str]**](str.md)| filter by attribute &#39;state&#39; | [optional] 
 **filter_version** | [**List[str]**](str.md)| filter by attribute &#39;version&#39; | [optional] 
 **filter_internal_beta_release_state** | [**List[str]**](str.md)| filter by attribute &#39;internalBetaRelease.state&#39; | [optional] 
 **sort** | [**List[str]**](str.md)| comma-separated list of sort expressions; resources will be sorted as specified | [optional] 
 **fields_background_asset_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type backgroundAssetVersions | [optional] 
 **fields_background_asset_version_internal_beta_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type backgroundAssetVersionInternalBetaReleases | [optional] 
 **fields_background_asset_upload_files** | [**List[str]**](str.md)| the fields to include for returned resources of type backgroundAssetUploadFiles | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**BackgroundAssetVersionsResponse**](BackgroundAssetVersionsResponse.md)

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
**200** | List of BackgroundAssetVersions |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **background_assets_versions_get_to_many_relationship**
> BackgroundAssetVersionsLinkagesResponse background_assets_versions_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.background_asset_versions_linkages_response import BackgroundAssetVersionsLinkagesResponse
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
    api_instance = openapi_client.BackgroundAssetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.background_assets_versions_get_to_many_relationship(id, limit=limit)
        print("The response of BackgroundAssetsApi->background_assets_versions_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BackgroundAssetsApi->background_assets_versions_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**BackgroundAssetVersionsLinkagesResponse**](BackgroundAssetVersionsLinkagesResponse.md)

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

