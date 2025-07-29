# openapi_client.AppClipsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**app_clips_app_clip_advanced_experiences_get_to_many_related**](AppClipsApi.md#app_clips_app_clip_advanced_experiences_get_to_many_related) | **GET** /v1/appClips/{id}/appClipAdvancedExperiences | 
[**app_clips_app_clip_advanced_experiences_get_to_many_relationship**](AppClipsApi.md#app_clips_app_clip_advanced_experiences_get_to_many_relationship) | **GET** /v1/appClips/{id}/relationships/appClipAdvancedExperiences | 
[**app_clips_app_clip_default_experiences_get_to_many_related**](AppClipsApi.md#app_clips_app_clip_default_experiences_get_to_many_related) | **GET** /v1/appClips/{id}/appClipDefaultExperiences | 
[**app_clips_app_clip_default_experiences_get_to_many_relationship**](AppClipsApi.md#app_clips_app_clip_default_experiences_get_to_many_relationship) | **GET** /v1/appClips/{id}/relationships/appClipDefaultExperiences | 
[**app_clips_get_instance**](AppClipsApi.md#app_clips_get_instance) | **GET** /v1/appClips/{id} | 


# **app_clips_app_clip_advanced_experiences_get_to_many_related**
> AppClipAdvancedExperiencesResponse app_clips_app_clip_advanced_experiences_get_to_many_related(id, filter_status=filter_status, filter_place_status=filter_place_status, filter_action=filter_action, fields_app_clip_advanced_experiences=fields_app_clip_advanced_experiences, fields_app_clips=fields_app_clips, fields_app_clip_advanced_experience_images=fields_app_clip_advanced_experience_images, fields_app_clip_advanced_experience_localizations=fields_app_clip_advanced_experience_localizations, limit=limit, include=include, limit_localizations=limit_localizations)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_advanced_experiences_response import AppClipAdvancedExperiencesResponse
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
    api_instance = openapi_client.AppClipsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_status = ['filter_status_example'] # List[str] | filter by attribute 'status' (optional)
    filter_place_status = ['filter_place_status_example'] # List[str] | filter by attribute 'placeStatus' (optional)
    filter_action = ['filter_action_example'] # List[str] | filter by attribute 'action' (optional)
    fields_app_clip_advanced_experiences = ['fields_app_clip_advanced_experiences_example'] # List[str] | the fields to include for returned resources of type appClipAdvancedExperiences (optional)
    fields_app_clips = ['fields_app_clips_example'] # List[str] | the fields to include for returned resources of type appClips (optional)
    fields_app_clip_advanced_experience_images = ['fields_app_clip_advanced_experience_images_example'] # List[str] | the fields to include for returned resources of type appClipAdvancedExperienceImages (optional)
    fields_app_clip_advanced_experience_localizations = ['fields_app_clip_advanced_experience_localizations_example'] # List[str] | the fields to include for returned resources of type appClipAdvancedExperienceLocalizations (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_localizations = 56 # int | maximum number of related localizations returned (when they are included) (optional)

    try:
        api_response = api_instance.app_clips_app_clip_advanced_experiences_get_to_many_related(id, filter_status=filter_status, filter_place_status=filter_place_status, filter_action=filter_action, fields_app_clip_advanced_experiences=fields_app_clip_advanced_experiences, fields_app_clips=fields_app_clips, fields_app_clip_advanced_experience_images=fields_app_clip_advanced_experience_images, fields_app_clip_advanced_experience_localizations=fields_app_clip_advanced_experience_localizations, limit=limit, include=include, limit_localizations=limit_localizations)
        print("The response of AppClipsApi->app_clips_app_clip_advanced_experiences_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipsApi->app_clips_app_clip_advanced_experiences_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_status** | [**List[str]**](str.md)| filter by attribute &#39;status&#39; | [optional] 
 **filter_place_status** | [**List[str]**](str.md)| filter by attribute &#39;placeStatus&#39; | [optional] 
 **filter_action** | [**List[str]**](str.md)| filter by attribute &#39;action&#39; | [optional] 
 **fields_app_clip_advanced_experiences** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipAdvancedExperiences | [optional] 
 **fields_app_clips** | [**List[str]**](str.md)| the fields to include for returned resources of type appClips | [optional] 
 **fields_app_clip_advanced_experience_images** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipAdvancedExperienceImages | [optional] 
 **fields_app_clip_advanced_experience_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipAdvancedExperienceLocalizations | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_localizations** | **int**| maximum number of related localizations returned (when they are included) | [optional] 

### Return type

[**AppClipAdvancedExperiencesResponse**](AppClipAdvancedExperiencesResponse.md)

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
**200** | List of AppClipAdvancedExperiences |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_clips_app_clip_advanced_experiences_get_to_many_relationship**
> AppClipAppClipAdvancedExperiencesLinkagesResponse app_clips_app_clip_advanced_experiences_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_app_clip_advanced_experiences_linkages_response import AppClipAppClipAdvancedExperiencesLinkagesResponse
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
    api_instance = openapi_client.AppClipsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.app_clips_app_clip_advanced_experiences_get_to_many_relationship(id, limit=limit)
        print("The response of AppClipsApi->app_clips_app_clip_advanced_experiences_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipsApi->app_clips_app_clip_advanced_experiences_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AppClipAppClipAdvancedExperiencesLinkagesResponse**](AppClipAppClipAdvancedExperiencesLinkagesResponse.md)

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

# **app_clips_app_clip_default_experiences_get_to_many_related**
> AppClipDefaultExperiencesResponse app_clips_app_clip_default_experiences_get_to_many_related(id, exists_release_with_app_store_version=exists_release_with_app_store_version, fields_app_clip_default_experiences=fields_app_clip_default_experiences, fields_app_clips=fields_app_clips, fields_app_store_versions=fields_app_store_versions, fields_app_clip_default_experience_localizations=fields_app_clip_default_experience_localizations, fields_app_clip_app_store_review_details=fields_app_clip_app_store_review_details, limit=limit, include=include, limit_app_clip_default_experience_localizations=limit_app_clip_default_experience_localizations)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_default_experiences_response import AppClipDefaultExperiencesResponse
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
    api_instance = openapi_client.AppClipsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    exists_release_with_app_store_version = True # bool | filter by existence or non-existence of related 'releaseWithAppStoreVersion' (optional)
    fields_app_clip_default_experiences = ['fields_app_clip_default_experiences_example'] # List[str] | the fields to include for returned resources of type appClipDefaultExperiences (optional)
    fields_app_clips = ['fields_app_clips_example'] # List[str] | the fields to include for returned resources of type appClips (optional)
    fields_app_store_versions = ['fields_app_store_versions_example'] # List[str] | the fields to include for returned resources of type appStoreVersions (optional)
    fields_app_clip_default_experience_localizations = ['fields_app_clip_default_experience_localizations_example'] # List[str] | the fields to include for returned resources of type appClipDefaultExperienceLocalizations (optional)
    fields_app_clip_app_store_review_details = ['fields_app_clip_app_store_review_details_example'] # List[str] | the fields to include for returned resources of type appClipAppStoreReviewDetails (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_clip_default_experience_localizations = 56 # int | maximum number of related appClipDefaultExperienceLocalizations returned (when they are included) (optional)

    try:
        api_response = api_instance.app_clips_app_clip_default_experiences_get_to_many_related(id, exists_release_with_app_store_version=exists_release_with_app_store_version, fields_app_clip_default_experiences=fields_app_clip_default_experiences, fields_app_clips=fields_app_clips, fields_app_store_versions=fields_app_store_versions, fields_app_clip_default_experience_localizations=fields_app_clip_default_experience_localizations, fields_app_clip_app_store_review_details=fields_app_clip_app_store_review_details, limit=limit, include=include, limit_app_clip_default_experience_localizations=limit_app_clip_default_experience_localizations)
        print("The response of AppClipsApi->app_clips_app_clip_default_experiences_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipsApi->app_clips_app_clip_default_experiences_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **exists_release_with_app_store_version** | **bool**| filter by existence or non-existence of related &#39;releaseWithAppStoreVersion&#39; | [optional] 
 **fields_app_clip_default_experiences** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipDefaultExperiences | [optional] 
 **fields_app_clips** | [**List[str]**](str.md)| the fields to include for returned resources of type appClips | [optional] 
 **fields_app_store_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersions | [optional] 
 **fields_app_clip_default_experience_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipDefaultExperienceLocalizations | [optional] 
 **fields_app_clip_app_store_review_details** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipAppStoreReviewDetails | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_clip_default_experience_localizations** | **int**| maximum number of related appClipDefaultExperienceLocalizations returned (when they are included) | [optional] 

### Return type

[**AppClipDefaultExperiencesResponse**](AppClipDefaultExperiencesResponse.md)

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
**200** | List of AppClipDefaultExperiences |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_clips_app_clip_default_experiences_get_to_many_relationship**
> AppClipAppClipDefaultExperiencesLinkagesResponse app_clips_app_clip_default_experiences_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_app_clip_default_experiences_linkages_response import AppClipAppClipDefaultExperiencesLinkagesResponse
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
    api_instance = openapi_client.AppClipsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.app_clips_app_clip_default_experiences_get_to_many_relationship(id, limit=limit)
        print("The response of AppClipsApi->app_clips_app_clip_default_experiences_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipsApi->app_clips_app_clip_default_experiences_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AppClipAppClipDefaultExperiencesLinkagesResponse**](AppClipAppClipDefaultExperiencesLinkagesResponse.md)

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

# **app_clips_get_instance**
> AppClipResponse app_clips_get_instance(id, fields_app_clips=fields_app_clips, fields_app_clip_default_experiences=fields_app_clip_default_experiences, include=include, limit_app_clip_default_experiences=limit_app_clip_default_experiences)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_response import AppClipResponse
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
    api_instance = openapi_client.AppClipsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_clips = ['fields_app_clips_example'] # List[str] | the fields to include for returned resources of type appClips (optional)
    fields_app_clip_default_experiences = ['fields_app_clip_default_experiences_example'] # List[str] | the fields to include for returned resources of type appClipDefaultExperiences (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_clip_default_experiences = 56 # int | maximum number of related appClipDefaultExperiences returned (when they are included) (optional)

    try:
        api_response = api_instance.app_clips_get_instance(id, fields_app_clips=fields_app_clips, fields_app_clip_default_experiences=fields_app_clip_default_experiences, include=include, limit_app_clip_default_experiences=limit_app_clip_default_experiences)
        print("The response of AppClipsApi->app_clips_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipsApi->app_clips_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_clips** | [**List[str]**](str.md)| the fields to include for returned resources of type appClips | [optional] 
 **fields_app_clip_default_experiences** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipDefaultExperiences | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_clip_default_experiences** | **int**| maximum number of related appClipDefaultExperiences returned (when they are included) | [optional] 

### Return type

[**AppClipResponse**](AppClipResponse.md)

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
**200** | Single AppClip |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

