# openapi_client.AppEventLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**app_event_localizations_app_event_screenshots_get_to_many_related**](AppEventLocalizationsApi.md#app_event_localizations_app_event_screenshots_get_to_many_related) | **GET** /v1/appEventLocalizations/{id}/appEventScreenshots | 
[**app_event_localizations_app_event_screenshots_get_to_many_relationship**](AppEventLocalizationsApi.md#app_event_localizations_app_event_screenshots_get_to_many_relationship) | **GET** /v1/appEventLocalizations/{id}/relationships/appEventScreenshots | 
[**app_event_localizations_app_event_video_clips_get_to_many_related**](AppEventLocalizationsApi.md#app_event_localizations_app_event_video_clips_get_to_many_related) | **GET** /v1/appEventLocalizations/{id}/appEventVideoClips | 
[**app_event_localizations_app_event_video_clips_get_to_many_relationship**](AppEventLocalizationsApi.md#app_event_localizations_app_event_video_clips_get_to_many_relationship) | **GET** /v1/appEventLocalizations/{id}/relationships/appEventVideoClips | 
[**app_event_localizations_create_instance**](AppEventLocalizationsApi.md#app_event_localizations_create_instance) | **POST** /v1/appEventLocalizations | 
[**app_event_localizations_delete_instance**](AppEventLocalizationsApi.md#app_event_localizations_delete_instance) | **DELETE** /v1/appEventLocalizations/{id} | 
[**app_event_localizations_get_instance**](AppEventLocalizationsApi.md#app_event_localizations_get_instance) | **GET** /v1/appEventLocalizations/{id} | 
[**app_event_localizations_update_instance**](AppEventLocalizationsApi.md#app_event_localizations_update_instance) | **PATCH** /v1/appEventLocalizations/{id} | 


# **app_event_localizations_app_event_screenshots_get_to_many_related**
> AppEventScreenshotsResponse app_event_localizations_app_event_screenshots_get_to_many_related(id, fields_app_event_screenshots=fields_app_event_screenshots, fields_app_event_localizations=fields_app_event_localizations, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_event_screenshots_response import AppEventScreenshotsResponse
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
    api_instance = openapi_client.AppEventLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_event_screenshots = ['fields_app_event_screenshots_example'] # List[str] | the fields to include for returned resources of type appEventScreenshots (optional)
    fields_app_event_localizations = ['fields_app_event_localizations_example'] # List[str] | the fields to include for returned resources of type appEventLocalizations (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.app_event_localizations_app_event_screenshots_get_to_many_related(id, fields_app_event_screenshots=fields_app_event_screenshots, fields_app_event_localizations=fields_app_event_localizations, limit=limit, include=include)
        print("The response of AppEventLocalizationsApi->app_event_localizations_app_event_screenshots_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEventLocalizationsApi->app_event_localizations_app_event_screenshots_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_event_screenshots** | [**List[str]**](str.md)| the fields to include for returned resources of type appEventScreenshots | [optional] 
 **fields_app_event_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appEventLocalizations | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**AppEventScreenshotsResponse**](AppEventScreenshotsResponse.md)

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
**200** | List of AppEventScreenshots |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_event_localizations_app_event_screenshots_get_to_many_relationship**
> AppEventLocalizationAppEventScreenshotsLinkagesResponse app_event_localizations_app_event_screenshots_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_event_localization_app_event_screenshots_linkages_response import AppEventLocalizationAppEventScreenshotsLinkagesResponse
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
    api_instance = openapi_client.AppEventLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.app_event_localizations_app_event_screenshots_get_to_many_relationship(id, limit=limit)
        print("The response of AppEventLocalizationsApi->app_event_localizations_app_event_screenshots_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEventLocalizationsApi->app_event_localizations_app_event_screenshots_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AppEventLocalizationAppEventScreenshotsLinkagesResponse**](AppEventLocalizationAppEventScreenshotsLinkagesResponse.md)

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

# **app_event_localizations_app_event_video_clips_get_to_many_related**
> AppEventVideoClipsResponse app_event_localizations_app_event_video_clips_get_to_many_related(id, fields_app_event_video_clips=fields_app_event_video_clips, fields_app_event_localizations=fields_app_event_localizations, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_event_video_clips_response import AppEventVideoClipsResponse
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
    api_instance = openapi_client.AppEventLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_event_video_clips = ['fields_app_event_video_clips_example'] # List[str] | the fields to include for returned resources of type appEventVideoClips (optional)
    fields_app_event_localizations = ['fields_app_event_localizations_example'] # List[str] | the fields to include for returned resources of type appEventLocalizations (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.app_event_localizations_app_event_video_clips_get_to_many_related(id, fields_app_event_video_clips=fields_app_event_video_clips, fields_app_event_localizations=fields_app_event_localizations, limit=limit, include=include)
        print("The response of AppEventLocalizationsApi->app_event_localizations_app_event_video_clips_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEventLocalizationsApi->app_event_localizations_app_event_video_clips_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_event_video_clips** | [**List[str]**](str.md)| the fields to include for returned resources of type appEventVideoClips | [optional] 
 **fields_app_event_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appEventLocalizations | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**AppEventVideoClipsResponse**](AppEventVideoClipsResponse.md)

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
**200** | List of AppEventVideoClips |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_event_localizations_app_event_video_clips_get_to_many_relationship**
> AppEventLocalizationAppEventVideoClipsLinkagesResponse app_event_localizations_app_event_video_clips_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_event_localization_app_event_video_clips_linkages_response import AppEventLocalizationAppEventVideoClipsLinkagesResponse
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
    api_instance = openapi_client.AppEventLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.app_event_localizations_app_event_video_clips_get_to_many_relationship(id, limit=limit)
        print("The response of AppEventLocalizationsApi->app_event_localizations_app_event_video_clips_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEventLocalizationsApi->app_event_localizations_app_event_video_clips_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AppEventLocalizationAppEventVideoClipsLinkagesResponse**](AppEventLocalizationAppEventVideoClipsLinkagesResponse.md)

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

# **app_event_localizations_create_instance**
> AppEventLocalizationResponse app_event_localizations_create_instance(app_event_localization_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_event_localization_create_request import AppEventLocalizationCreateRequest
from openapi_client.models.app_event_localization_response import AppEventLocalizationResponse
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
    api_instance = openapi_client.AppEventLocalizationsApi(api_client)
    app_event_localization_create_request = openapi_client.AppEventLocalizationCreateRequest() # AppEventLocalizationCreateRequest | AppEventLocalization representation

    try:
        api_response = api_instance.app_event_localizations_create_instance(app_event_localization_create_request)
        print("The response of AppEventLocalizationsApi->app_event_localizations_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEventLocalizationsApi->app_event_localizations_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **app_event_localization_create_request** | [**AppEventLocalizationCreateRequest**](AppEventLocalizationCreateRequest.md)| AppEventLocalization representation | 

### Return type

[**AppEventLocalizationResponse**](AppEventLocalizationResponse.md)

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
**201** | Single AppEventLocalization |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_event_localizations_delete_instance**
> app_event_localizations_delete_instance(id)

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
    api_instance = openapi_client.AppEventLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.app_event_localizations_delete_instance(id)
    except Exception as e:
        print("Exception when calling AppEventLocalizationsApi->app_event_localizations_delete_instance: %s\n" % e)
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

# **app_event_localizations_get_instance**
> AppEventLocalizationResponse app_event_localizations_get_instance(id, fields_app_event_localizations=fields_app_event_localizations, fields_app_event_screenshots=fields_app_event_screenshots, fields_app_event_video_clips=fields_app_event_video_clips, include=include, limit_app_event_screenshots=limit_app_event_screenshots, limit_app_event_video_clips=limit_app_event_video_clips)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_event_localization_response import AppEventLocalizationResponse
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
    api_instance = openapi_client.AppEventLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_event_localizations = ['fields_app_event_localizations_example'] # List[str] | the fields to include for returned resources of type appEventLocalizations (optional)
    fields_app_event_screenshots = ['fields_app_event_screenshots_example'] # List[str] | the fields to include for returned resources of type appEventScreenshots (optional)
    fields_app_event_video_clips = ['fields_app_event_video_clips_example'] # List[str] | the fields to include for returned resources of type appEventVideoClips (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_event_screenshots = 56 # int | maximum number of related appEventScreenshots returned (when they are included) (optional)
    limit_app_event_video_clips = 56 # int | maximum number of related appEventVideoClips returned (when they are included) (optional)

    try:
        api_response = api_instance.app_event_localizations_get_instance(id, fields_app_event_localizations=fields_app_event_localizations, fields_app_event_screenshots=fields_app_event_screenshots, fields_app_event_video_clips=fields_app_event_video_clips, include=include, limit_app_event_screenshots=limit_app_event_screenshots, limit_app_event_video_clips=limit_app_event_video_clips)
        print("The response of AppEventLocalizationsApi->app_event_localizations_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEventLocalizationsApi->app_event_localizations_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_event_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appEventLocalizations | [optional] 
 **fields_app_event_screenshots** | [**List[str]**](str.md)| the fields to include for returned resources of type appEventScreenshots | [optional] 
 **fields_app_event_video_clips** | [**List[str]**](str.md)| the fields to include for returned resources of type appEventVideoClips | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_event_screenshots** | **int**| maximum number of related appEventScreenshots returned (when they are included) | [optional] 
 **limit_app_event_video_clips** | **int**| maximum number of related appEventVideoClips returned (when they are included) | [optional] 

### Return type

[**AppEventLocalizationResponse**](AppEventLocalizationResponse.md)

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
**200** | Single AppEventLocalization |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_event_localizations_update_instance**
> AppEventLocalizationResponse app_event_localizations_update_instance(id, app_event_localization_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_event_localization_response import AppEventLocalizationResponse
from openapi_client.models.app_event_localization_update_request import AppEventLocalizationUpdateRequest
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
    api_instance = openapi_client.AppEventLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    app_event_localization_update_request = openapi_client.AppEventLocalizationUpdateRequest() # AppEventLocalizationUpdateRequest | AppEventLocalization representation

    try:
        api_response = api_instance.app_event_localizations_update_instance(id, app_event_localization_update_request)
        print("The response of AppEventLocalizationsApi->app_event_localizations_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEventLocalizationsApi->app_event_localizations_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **app_event_localization_update_request** | [**AppEventLocalizationUpdateRequest**](AppEventLocalizationUpdateRequest.md)| AppEventLocalization representation | 

### Return type

[**AppEventLocalizationResponse**](AppEventLocalizationResponse.md)

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
**200** | Single AppEventLocalization |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

