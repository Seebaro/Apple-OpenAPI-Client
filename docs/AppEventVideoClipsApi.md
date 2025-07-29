# openapi_client.AppEventVideoClipsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**app_event_video_clips_create_instance**](AppEventVideoClipsApi.md#app_event_video_clips_create_instance) | **POST** /v1/appEventVideoClips | 
[**app_event_video_clips_delete_instance**](AppEventVideoClipsApi.md#app_event_video_clips_delete_instance) | **DELETE** /v1/appEventVideoClips/{id} | 
[**app_event_video_clips_get_instance**](AppEventVideoClipsApi.md#app_event_video_clips_get_instance) | **GET** /v1/appEventVideoClips/{id} | 
[**app_event_video_clips_update_instance**](AppEventVideoClipsApi.md#app_event_video_clips_update_instance) | **PATCH** /v1/appEventVideoClips/{id} | 


# **app_event_video_clips_create_instance**
> AppEventVideoClipResponse app_event_video_clips_create_instance(app_event_video_clip_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_event_video_clip_create_request import AppEventVideoClipCreateRequest
from openapi_client.models.app_event_video_clip_response import AppEventVideoClipResponse
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
    api_instance = openapi_client.AppEventVideoClipsApi(api_client)
    app_event_video_clip_create_request = openapi_client.AppEventVideoClipCreateRequest() # AppEventVideoClipCreateRequest | AppEventVideoClip representation

    try:
        api_response = api_instance.app_event_video_clips_create_instance(app_event_video_clip_create_request)
        print("The response of AppEventVideoClipsApi->app_event_video_clips_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEventVideoClipsApi->app_event_video_clips_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **app_event_video_clip_create_request** | [**AppEventVideoClipCreateRequest**](AppEventVideoClipCreateRequest.md)| AppEventVideoClip representation | 

### Return type

[**AppEventVideoClipResponse**](AppEventVideoClipResponse.md)

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
**201** | Single AppEventVideoClip |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_event_video_clips_delete_instance**
> app_event_video_clips_delete_instance(id)

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
    api_instance = openapi_client.AppEventVideoClipsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.app_event_video_clips_delete_instance(id)
    except Exception as e:
        print("Exception when calling AppEventVideoClipsApi->app_event_video_clips_delete_instance: %s\n" % e)
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

# **app_event_video_clips_get_instance**
> AppEventVideoClipResponse app_event_video_clips_get_instance(id, fields_app_event_video_clips=fields_app_event_video_clips, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_event_video_clip_response import AppEventVideoClipResponse
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
    api_instance = openapi_client.AppEventVideoClipsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_event_video_clips = ['fields_app_event_video_clips_example'] # List[str] | the fields to include for returned resources of type appEventVideoClips (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.app_event_video_clips_get_instance(id, fields_app_event_video_clips=fields_app_event_video_clips, include=include)
        print("The response of AppEventVideoClipsApi->app_event_video_clips_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEventVideoClipsApi->app_event_video_clips_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_event_video_clips** | [**List[str]**](str.md)| the fields to include for returned resources of type appEventVideoClips | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**AppEventVideoClipResponse**](AppEventVideoClipResponse.md)

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
**200** | Single AppEventVideoClip |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_event_video_clips_update_instance**
> AppEventVideoClipResponse app_event_video_clips_update_instance(id, app_event_video_clip_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_event_video_clip_response import AppEventVideoClipResponse
from openapi_client.models.app_event_video_clip_update_request import AppEventVideoClipUpdateRequest
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
    api_instance = openapi_client.AppEventVideoClipsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    app_event_video_clip_update_request = openapi_client.AppEventVideoClipUpdateRequest() # AppEventVideoClipUpdateRequest | AppEventVideoClip representation

    try:
        api_response = api_instance.app_event_video_clips_update_instance(id, app_event_video_clip_update_request)
        print("The response of AppEventVideoClipsApi->app_event_video_clips_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEventVideoClipsApi->app_event_video_clips_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **app_event_video_clip_update_request** | [**AppEventVideoClipUpdateRequest**](AppEventVideoClipUpdateRequest.md)| AppEventVideoClip representation | 

### Return type

[**AppEventVideoClipResponse**](AppEventVideoClipResponse.md)

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
**200** | Single AppEventVideoClip |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

