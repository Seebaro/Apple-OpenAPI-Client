# openapi_client.BackgroundAssetUploadFilesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**background_asset_upload_files_create_instance**](BackgroundAssetUploadFilesApi.md#background_asset_upload_files_create_instance) | **POST** /v1/backgroundAssetUploadFiles | 
[**background_asset_upload_files_get_instance**](BackgroundAssetUploadFilesApi.md#background_asset_upload_files_get_instance) | **GET** /v1/backgroundAssetUploadFiles/{id} | 
[**background_asset_upload_files_update_instance**](BackgroundAssetUploadFilesApi.md#background_asset_upload_files_update_instance) | **PATCH** /v1/backgroundAssetUploadFiles/{id} | 


# **background_asset_upload_files_create_instance**
> BackgroundAssetUploadFileResponse background_asset_upload_files_create_instance(background_asset_upload_file_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.background_asset_upload_file_create_request import BackgroundAssetUploadFileCreateRequest
from openapi_client.models.background_asset_upload_file_response import BackgroundAssetUploadFileResponse
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
    api_instance = openapi_client.BackgroundAssetUploadFilesApi(api_client)
    background_asset_upload_file_create_request = openapi_client.BackgroundAssetUploadFileCreateRequest() # BackgroundAssetUploadFileCreateRequest | BackgroundAssetUploadFile representation

    try:
        api_response = api_instance.background_asset_upload_files_create_instance(background_asset_upload_file_create_request)
        print("The response of BackgroundAssetUploadFilesApi->background_asset_upload_files_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BackgroundAssetUploadFilesApi->background_asset_upload_files_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **background_asset_upload_file_create_request** | [**BackgroundAssetUploadFileCreateRequest**](BackgroundAssetUploadFileCreateRequest.md)| BackgroundAssetUploadFile representation | 

### Return type

[**BackgroundAssetUploadFileResponse**](BackgroundAssetUploadFileResponse.md)

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
**201** | Single BackgroundAssetUploadFile |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **background_asset_upload_files_get_instance**
> BackgroundAssetUploadFileResponse background_asset_upload_files_get_instance(id, fields_background_asset_upload_files=fields_background_asset_upload_files)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.background_asset_upload_file_response import BackgroundAssetUploadFileResponse
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
    api_instance = openapi_client.BackgroundAssetUploadFilesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_background_asset_upload_files = ['fields_background_asset_upload_files_example'] # List[str] | the fields to include for returned resources of type backgroundAssetUploadFiles (optional)

    try:
        api_response = api_instance.background_asset_upload_files_get_instance(id, fields_background_asset_upload_files=fields_background_asset_upload_files)
        print("The response of BackgroundAssetUploadFilesApi->background_asset_upload_files_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BackgroundAssetUploadFilesApi->background_asset_upload_files_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_background_asset_upload_files** | [**List[str]**](str.md)| the fields to include for returned resources of type backgroundAssetUploadFiles | [optional] 

### Return type

[**BackgroundAssetUploadFileResponse**](BackgroundAssetUploadFileResponse.md)

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
**200** | Single BackgroundAssetUploadFile |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **background_asset_upload_files_update_instance**
> BackgroundAssetUploadFileResponse background_asset_upload_files_update_instance(id, background_asset_upload_file_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.background_asset_upload_file_response import BackgroundAssetUploadFileResponse
from openapi_client.models.background_asset_upload_file_update_request import BackgroundAssetUploadFileUpdateRequest
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
    api_instance = openapi_client.BackgroundAssetUploadFilesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    background_asset_upload_file_update_request = openapi_client.BackgroundAssetUploadFileUpdateRequest() # BackgroundAssetUploadFileUpdateRequest | BackgroundAssetUploadFile representation

    try:
        api_response = api_instance.background_asset_upload_files_update_instance(id, background_asset_upload_file_update_request)
        print("The response of BackgroundAssetUploadFilesApi->background_asset_upload_files_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BackgroundAssetUploadFilesApi->background_asset_upload_files_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **background_asset_upload_file_update_request** | [**BackgroundAssetUploadFileUpdateRequest**](BackgroundAssetUploadFileUpdateRequest.md)| BackgroundAssetUploadFile representation | 

### Return type

[**BackgroundAssetUploadFileResponse**](BackgroundAssetUploadFileResponse.md)

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
**404** | Not found error |  -  |
**422** | Unprocessable request entity error(s) |  -  |
**200** | Single BackgroundAssetUploadFile |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

