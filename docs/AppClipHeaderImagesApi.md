# openapi_client.AppClipHeaderImagesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**app_clip_header_images_create_instance**](AppClipHeaderImagesApi.md#app_clip_header_images_create_instance) | **POST** /v1/appClipHeaderImages | 
[**app_clip_header_images_delete_instance**](AppClipHeaderImagesApi.md#app_clip_header_images_delete_instance) | **DELETE** /v1/appClipHeaderImages/{id} | 
[**app_clip_header_images_get_instance**](AppClipHeaderImagesApi.md#app_clip_header_images_get_instance) | **GET** /v1/appClipHeaderImages/{id} | 
[**app_clip_header_images_update_instance**](AppClipHeaderImagesApi.md#app_clip_header_images_update_instance) | **PATCH** /v1/appClipHeaderImages/{id} | 


# **app_clip_header_images_create_instance**
> AppClipHeaderImageResponse app_clip_header_images_create_instance(app_clip_header_image_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_header_image_create_request import AppClipHeaderImageCreateRequest
from openapi_client.models.app_clip_header_image_response import AppClipHeaderImageResponse
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
    api_instance = openapi_client.AppClipHeaderImagesApi(api_client)
    app_clip_header_image_create_request = openapi_client.AppClipHeaderImageCreateRequest() # AppClipHeaderImageCreateRequest | AppClipHeaderImage representation

    try:
        api_response = api_instance.app_clip_header_images_create_instance(app_clip_header_image_create_request)
        print("The response of AppClipHeaderImagesApi->app_clip_header_images_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipHeaderImagesApi->app_clip_header_images_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **app_clip_header_image_create_request** | [**AppClipHeaderImageCreateRequest**](AppClipHeaderImageCreateRequest.md)| AppClipHeaderImage representation | 

### Return type

[**AppClipHeaderImageResponse**](AppClipHeaderImageResponse.md)

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
**201** | Single AppClipHeaderImage |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_clip_header_images_delete_instance**
> app_clip_header_images_delete_instance(id)

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
    api_instance = openapi_client.AppClipHeaderImagesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.app_clip_header_images_delete_instance(id)
    except Exception as e:
        print("Exception when calling AppClipHeaderImagesApi->app_clip_header_images_delete_instance: %s\n" % e)
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

# **app_clip_header_images_get_instance**
> AppClipHeaderImageResponse app_clip_header_images_get_instance(id, fields_app_clip_header_images=fields_app_clip_header_images, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_header_image_response import AppClipHeaderImageResponse
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
    api_instance = openapi_client.AppClipHeaderImagesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_clip_header_images = ['fields_app_clip_header_images_example'] # List[str] | the fields to include for returned resources of type appClipHeaderImages (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.app_clip_header_images_get_instance(id, fields_app_clip_header_images=fields_app_clip_header_images, include=include)
        print("The response of AppClipHeaderImagesApi->app_clip_header_images_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipHeaderImagesApi->app_clip_header_images_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_clip_header_images** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipHeaderImages | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**AppClipHeaderImageResponse**](AppClipHeaderImageResponse.md)

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
**200** | Single AppClipHeaderImage |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_clip_header_images_update_instance**
> AppClipHeaderImageResponse app_clip_header_images_update_instance(id, app_clip_header_image_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_header_image_response import AppClipHeaderImageResponse
from openapi_client.models.app_clip_header_image_update_request import AppClipHeaderImageUpdateRequest
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
    api_instance = openapi_client.AppClipHeaderImagesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    app_clip_header_image_update_request = openapi_client.AppClipHeaderImageUpdateRequest() # AppClipHeaderImageUpdateRequest | AppClipHeaderImage representation

    try:
        api_response = api_instance.app_clip_header_images_update_instance(id, app_clip_header_image_update_request)
        print("The response of AppClipHeaderImagesApi->app_clip_header_images_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipHeaderImagesApi->app_clip_header_images_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **app_clip_header_image_update_request** | [**AppClipHeaderImageUpdateRequest**](AppClipHeaderImageUpdateRequest.md)| AppClipHeaderImage representation | 

### Return type

[**AppClipHeaderImageResponse**](AppClipHeaderImageResponse.md)

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
**200** | Single AppClipHeaderImage |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

