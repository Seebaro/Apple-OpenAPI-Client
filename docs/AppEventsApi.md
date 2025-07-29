# openapi_client.AppEventsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**app_events_create_instance**](AppEventsApi.md#app_events_create_instance) | **POST** /v1/appEvents | 
[**app_events_delete_instance**](AppEventsApi.md#app_events_delete_instance) | **DELETE** /v1/appEvents/{id} | 
[**app_events_get_instance**](AppEventsApi.md#app_events_get_instance) | **GET** /v1/appEvents/{id} | 
[**app_events_localizations_get_to_many_related**](AppEventsApi.md#app_events_localizations_get_to_many_related) | **GET** /v1/appEvents/{id}/localizations | 
[**app_events_localizations_get_to_many_relationship**](AppEventsApi.md#app_events_localizations_get_to_many_relationship) | **GET** /v1/appEvents/{id}/relationships/localizations | 
[**app_events_update_instance**](AppEventsApi.md#app_events_update_instance) | **PATCH** /v1/appEvents/{id} | 


# **app_events_create_instance**
> AppEventResponse app_events_create_instance(app_event_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_event_create_request import AppEventCreateRequest
from openapi_client.models.app_event_response import AppEventResponse
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
    api_instance = openapi_client.AppEventsApi(api_client)
    app_event_create_request = openapi_client.AppEventCreateRequest() # AppEventCreateRequest | AppEvent representation

    try:
        api_response = api_instance.app_events_create_instance(app_event_create_request)
        print("The response of AppEventsApi->app_events_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEventsApi->app_events_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **app_event_create_request** | [**AppEventCreateRequest**](AppEventCreateRequest.md)| AppEvent representation | 

### Return type

[**AppEventResponse**](AppEventResponse.md)

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
**201** | Single AppEvent |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_events_delete_instance**
> app_events_delete_instance(id)

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
    api_instance = openapi_client.AppEventsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.app_events_delete_instance(id)
    except Exception as e:
        print("Exception when calling AppEventsApi->app_events_delete_instance: %s\n" % e)
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

# **app_events_get_instance**
> AppEventResponse app_events_get_instance(id, fields_app_events=fields_app_events, fields_app_event_localizations=fields_app_event_localizations, include=include, limit_localizations=limit_localizations)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_event_response import AppEventResponse
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
    api_instance = openapi_client.AppEventsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_events = ['fields_app_events_example'] # List[str] | the fields to include for returned resources of type appEvents (optional)
    fields_app_event_localizations = ['fields_app_event_localizations_example'] # List[str] | the fields to include for returned resources of type appEventLocalizations (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_localizations = 56 # int | maximum number of related localizations returned (when they are included) (optional)

    try:
        api_response = api_instance.app_events_get_instance(id, fields_app_events=fields_app_events, fields_app_event_localizations=fields_app_event_localizations, include=include, limit_localizations=limit_localizations)
        print("The response of AppEventsApi->app_events_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEventsApi->app_events_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_events** | [**List[str]**](str.md)| the fields to include for returned resources of type appEvents | [optional] 
 **fields_app_event_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appEventLocalizations | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_localizations** | **int**| maximum number of related localizations returned (when they are included) | [optional] 

### Return type

[**AppEventResponse**](AppEventResponse.md)

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
**200** | Single AppEvent |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_events_localizations_get_to_many_related**
> AppEventLocalizationsResponse app_events_localizations_get_to_many_related(id, fields_app_event_localizations=fields_app_event_localizations, fields_app_events=fields_app_events, fields_app_event_screenshots=fields_app_event_screenshots, fields_app_event_video_clips=fields_app_event_video_clips, limit=limit, include=include, limit_app_event_screenshots=limit_app_event_screenshots, limit_app_event_video_clips=limit_app_event_video_clips)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_event_localizations_response import AppEventLocalizationsResponse
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
    api_instance = openapi_client.AppEventsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_event_localizations = ['fields_app_event_localizations_example'] # List[str] | the fields to include for returned resources of type appEventLocalizations (optional)
    fields_app_events = ['fields_app_events_example'] # List[str] | the fields to include for returned resources of type appEvents (optional)
    fields_app_event_screenshots = ['fields_app_event_screenshots_example'] # List[str] | the fields to include for returned resources of type appEventScreenshots (optional)
    fields_app_event_video_clips = ['fields_app_event_video_clips_example'] # List[str] | the fields to include for returned resources of type appEventVideoClips (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_event_screenshots = 56 # int | maximum number of related appEventScreenshots returned (when they are included) (optional)
    limit_app_event_video_clips = 56 # int | maximum number of related appEventVideoClips returned (when they are included) (optional)

    try:
        api_response = api_instance.app_events_localizations_get_to_many_related(id, fields_app_event_localizations=fields_app_event_localizations, fields_app_events=fields_app_events, fields_app_event_screenshots=fields_app_event_screenshots, fields_app_event_video_clips=fields_app_event_video_clips, limit=limit, include=include, limit_app_event_screenshots=limit_app_event_screenshots, limit_app_event_video_clips=limit_app_event_video_clips)
        print("The response of AppEventsApi->app_events_localizations_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEventsApi->app_events_localizations_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_event_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appEventLocalizations | [optional] 
 **fields_app_events** | [**List[str]**](str.md)| the fields to include for returned resources of type appEvents | [optional] 
 **fields_app_event_screenshots** | [**List[str]**](str.md)| the fields to include for returned resources of type appEventScreenshots | [optional] 
 **fields_app_event_video_clips** | [**List[str]**](str.md)| the fields to include for returned resources of type appEventVideoClips | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_event_screenshots** | **int**| maximum number of related appEventScreenshots returned (when they are included) | [optional] 
 **limit_app_event_video_clips** | **int**| maximum number of related appEventVideoClips returned (when they are included) | [optional] 

### Return type

[**AppEventLocalizationsResponse**](AppEventLocalizationsResponse.md)

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
**200** | List of AppEventLocalizations |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_events_localizations_get_to_many_relationship**
> AppEventLocalizationsLinkagesResponse app_events_localizations_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_event_localizations_linkages_response import AppEventLocalizationsLinkagesResponse
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
    api_instance = openapi_client.AppEventsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.app_events_localizations_get_to_many_relationship(id, limit=limit)
        print("The response of AppEventsApi->app_events_localizations_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEventsApi->app_events_localizations_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AppEventLocalizationsLinkagesResponse**](AppEventLocalizationsLinkagesResponse.md)

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

# **app_events_update_instance**
> AppEventResponse app_events_update_instance(id, app_event_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_event_response import AppEventResponse
from openapi_client.models.app_event_update_request import AppEventUpdateRequest
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
    api_instance = openapi_client.AppEventsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    app_event_update_request = openapi_client.AppEventUpdateRequest() # AppEventUpdateRequest | AppEvent representation

    try:
        api_response = api_instance.app_events_update_instance(id, app_event_update_request)
        print("The response of AppEventsApi->app_events_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEventsApi->app_events_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **app_event_update_request** | [**AppEventUpdateRequest**](AppEventUpdateRequest.md)| AppEvent representation | 

### Return type

[**AppEventResponse**](AppEventResponse.md)

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
**200** | Single AppEvent |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

