# openapi_client.AppClipDefaultExperiencesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**app_clip_default_experiences_app_clip_app_store_review_detail_get_to_one_related**](AppClipDefaultExperiencesApi.md#app_clip_default_experiences_app_clip_app_store_review_detail_get_to_one_related) | **GET** /v1/appClipDefaultExperiences/{id}/appClipAppStoreReviewDetail | 
[**app_clip_default_experiences_app_clip_app_store_review_detail_get_to_one_relationship**](AppClipDefaultExperiencesApi.md#app_clip_default_experiences_app_clip_app_store_review_detail_get_to_one_relationship) | **GET** /v1/appClipDefaultExperiences/{id}/relationships/appClipAppStoreReviewDetail | 
[**app_clip_default_experiences_app_clip_default_experience_localizations_get_to_many_related**](AppClipDefaultExperiencesApi.md#app_clip_default_experiences_app_clip_default_experience_localizations_get_to_many_related) | **GET** /v1/appClipDefaultExperiences/{id}/appClipDefaultExperienceLocalizations | 
[**app_clip_default_experiences_app_clip_default_experience_localizations_get_to_many_relationship**](AppClipDefaultExperiencesApi.md#app_clip_default_experiences_app_clip_default_experience_localizations_get_to_many_relationship) | **GET** /v1/appClipDefaultExperiences/{id}/relationships/appClipDefaultExperienceLocalizations | 
[**app_clip_default_experiences_create_instance**](AppClipDefaultExperiencesApi.md#app_clip_default_experiences_create_instance) | **POST** /v1/appClipDefaultExperiences | 
[**app_clip_default_experiences_delete_instance**](AppClipDefaultExperiencesApi.md#app_clip_default_experiences_delete_instance) | **DELETE** /v1/appClipDefaultExperiences/{id} | 
[**app_clip_default_experiences_get_instance**](AppClipDefaultExperiencesApi.md#app_clip_default_experiences_get_instance) | **GET** /v1/appClipDefaultExperiences/{id} | 
[**app_clip_default_experiences_release_with_app_store_version_get_to_one_related**](AppClipDefaultExperiencesApi.md#app_clip_default_experiences_release_with_app_store_version_get_to_one_related) | **GET** /v1/appClipDefaultExperiences/{id}/releaseWithAppStoreVersion | 
[**app_clip_default_experiences_release_with_app_store_version_get_to_one_relationship**](AppClipDefaultExperiencesApi.md#app_clip_default_experiences_release_with_app_store_version_get_to_one_relationship) | **GET** /v1/appClipDefaultExperiences/{id}/relationships/releaseWithAppStoreVersion | 
[**app_clip_default_experiences_release_with_app_store_version_update_to_one_relationship**](AppClipDefaultExperiencesApi.md#app_clip_default_experiences_release_with_app_store_version_update_to_one_relationship) | **PATCH** /v1/appClipDefaultExperiences/{id}/relationships/releaseWithAppStoreVersion | 
[**app_clip_default_experiences_update_instance**](AppClipDefaultExperiencesApi.md#app_clip_default_experiences_update_instance) | **PATCH** /v1/appClipDefaultExperiences/{id} | 


# **app_clip_default_experiences_app_clip_app_store_review_detail_get_to_one_related**
> AppClipAppStoreReviewDetailResponse app_clip_default_experiences_app_clip_app_store_review_detail_get_to_one_related(id, fields_app_clip_app_store_review_details=fields_app_clip_app_store_review_details, fields_app_clip_default_experiences=fields_app_clip_default_experiences, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_app_store_review_detail_response import AppClipAppStoreReviewDetailResponse
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
    api_instance = openapi_client.AppClipDefaultExperiencesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_clip_app_store_review_details = ['fields_app_clip_app_store_review_details_example'] # List[str] | the fields to include for returned resources of type appClipAppStoreReviewDetails (optional)
    fields_app_clip_default_experiences = ['fields_app_clip_default_experiences_example'] # List[str] | the fields to include for returned resources of type appClipDefaultExperiences (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.app_clip_default_experiences_app_clip_app_store_review_detail_get_to_one_related(id, fields_app_clip_app_store_review_details=fields_app_clip_app_store_review_details, fields_app_clip_default_experiences=fields_app_clip_default_experiences, include=include)
        print("The response of AppClipDefaultExperiencesApi->app_clip_default_experiences_app_clip_app_store_review_detail_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipDefaultExperiencesApi->app_clip_default_experiences_app_clip_app_store_review_detail_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_clip_app_store_review_details** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipAppStoreReviewDetails | [optional] 
 **fields_app_clip_default_experiences** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipDefaultExperiences | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**AppClipAppStoreReviewDetailResponse**](AppClipAppStoreReviewDetailResponse.md)

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
**200** | Single AppClipAppStoreReviewDetail |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_clip_default_experiences_app_clip_app_store_review_detail_get_to_one_relationship**
> AppClipDefaultExperienceAppClipAppStoreReviewDetailLinkageResponse app_clip_default_experiences_app_clip_app_store_review_detail_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_default_experience_app_clip_app_store_review_detail_linkage_response import AppClipDefaultExperienceAppClipAppStoreReviewDetailLinkageResponse
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
    api_instance = openapi_client.AppClipDefaultExperiencesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.app_clip_default_experiences_app_clip_app_store_review_detail_get_to_one_relationship(id)
        print("The response of AppClipDefaultExperiencesApi->app_clip_default_experiences_app_clip_app_store_review_detail_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipDefaultExperiencesApi->app_clip_default_experiences_app_clip_app_store_review_detail_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**AppClipDefaultExperienceAppClipAppStoreReviewDetailLinkageResponse**](AppClipDefaultExperienceAppClipAppStoreReviewDetailLinkageResponse.md)

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

# **app_clip_default_experiences_app_clip_default_experience_localizations_get_to_many_related**
> AppClipDefaultExperienceLocalizationsResponse app_clip_default_experiences_app_clip_default_experience_localizations_get_to_many_related(id, filter_locale=filter_locale, fields_app_clip_default_experience_localizations=fields_app_clip_default_experience_localizations, fields_app_clip_default_experiences=fields_app_clip_default_experiences, fields_app_clip_header_images=fields_app_clip_header_images, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_default_experience_localizations_response import AppClipDefaultExperienceLocalizationsResponse
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
    api_instance = openapi_client.AppClipDefaultExperiencesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_locale = ['filter_locale_example'] # List[str] | filter by attribute 'locale' (optional)
    fields_app_clip_default_experience_localizations = ['fields_app_clip_default_experience_localizations_example'] # List[str] | the fields to include for returned resources of type appClipDefaultExperienceLocalizations (optional)
    fields_app_clip_default_experiences = ['fields_app_clip_default_experiences_example'] # List[str] | the fields to include for returned resources of type appClipDefaultExperiences (optional)
    fields_app_clip_header_images = ['fields_app_clip_header_images_example'] # List[str] | the fields to include for returned resources of type appClipHeaderImages (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.app_clip_default_experiences_app_clip_default_experience_localizations_get_to_many_related(id, filter_locale=filter_locale, fields_app_clip_default_experience_localizations=fields_app_clip_default_experience_localizations, fields_app_clip_default_experiences=fields_app_clip_default_experiences, fields_app_clip_header_images=fields_app_clip_header_images, limit=limit, include=include)
        print("The response of AppClipDefaultExperiencesApi->app_clip_default_experiences_app_clip_default_experience_localizations_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipDefaultExperiencesApi->app_clip_default_experiences_app_clip_default_experience_localizations_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_locale** | [**List[str]**](str.md)| filter by attribute &#39;locale&#39; | [optional] 
 **fields_app_clip_default_experience_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipDefaultExperienceLocalizations | [optional] 
 **fields_app_clip_default_experiences** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipDefaultExperiences | [optional] 
 **fields_app_clip_header_images** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipHeaderImages | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**AppClipDefaultExperienceLocalizationsResponse**](AppClipDefaultExperienceLocalizationsResponse.md)

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
**200** | List of AppClipDefaultExperienceLocalizations |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_clip_default_experiences_app_clip_default_experience_localizations_get_to_many_relationship**
> AppClipDefaultExperienceAppClipDefaultExperienceLocalizationsLinkagesResponse app_clip_default_experiences_app_clip_default_experience_localizations_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_default_experience_app_clip_default_experience_localizations_linkages_response import AppClipDefaultExperienceAppClipDefaultExperienceLocalizationsLinkagesResponse
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
    api_instance = openapi_client.AppClipDefaultExperiencesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.app_clip_default_experiences_app_clip_default_experience_localizations_get_to_many_relationship(id, limit=limit)
        print("The response of AppClipDefaultExperiencesApi->app_clip_default_experiences_app_clip_default_experience_localizations_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipDefaultExperiencesApi->app_clip_default_experiences_app_clip_default_experience_localizations_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AppClipDefaultExperienceAppClipDefaultExperienceLocalizationsLinkagesResponse**](AppClipDefaultExperienceAppClipDefaultExperienceLocalizationsLinkagesResponse.md)

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

# **app_clip_default_experiences_create_instance**
> AppClipDefaultExperienceResponse app_clip_default_experiences_create_instance(app_clip_default_experience_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_default_experience_create_request import AppClipDefaultExperienceCreateRequest
from openapi_client.models.app_clip_default_experience_response import AppClipDefaultExperienceResponse
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
    api_instance = openapi_client.AppClipDefaultExperiencesApi(api_client)
    app_clip_default_experience_create_request = openapi_client.AppClipDefaultExperienceCreateRequest() # AppClipDefaultExperienceCreateRequest | AppClipDefaultExperience representation

    try:
        api_response = api_instance.app_clip_default_experiences_create_instance(app_clip_default_experience_create_request)
        print("The response of AppClipDefaultExperiencesApi->app_clip_default_experiences_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipDefaultExperiencesApi->app_clip_default_experiences_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **app_clip_default_experience_create_request** | [**AppClipDefaultExperienceCreateRequest**](AppClipDefaultExperienceCreateRequest.md)| AppClipDefaultExperience representation | 

### Return type

[**AppClipDefaultExperienceResponse**](AppClipDefaultExperienceResponse.md)

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
**201** | Single AppClipDefaultExperience |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_clip_default_experiences_delete_instance**
> app_clip_default_experiences_delete_instance(id)

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
    api_instance = openapi_client.AppClipDefaultExperiencesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.app_clip_default_experiences_delete_instance(id)
    except Exception as e:
        print("Exception when calling AppClipDefaultExperiencesApi->app_clip_default_experiences_delete_instance: %s\n" % e)
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

# **app_clip_default_experiences_get_instance**
> AppClipDefaultExperienceResponse app_clip_default_experiences_get_instance(id, fields_app_clip_default_experiences=fields_app_clip_default_experiences, fields_app_store_versions=fields_app_store_versions, fields_app_clip_default_experience_localizations=fields_app_clip_default_experience_localizations, fields_app_clip_app_store_review_details=fields_app_clip_app_store_review_details, include=include, limit_app_clip_default_experience_localizations=limit_app_clip_default_experience_localizations)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_default_experience_response import AppClipDefaultExperienceResponse
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
    api_instance = openapi_client.AppClipDefaultExperiencesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_clip_default_experiences = ['fields_app_clip_default_experiences_example'] # List[str] | the fields to include for returned resources of type appClipDefaultExperiences (optional)
    fields_app_store_versions = ['fields_app_store_versions_example'] # List[str] | the fields to include for returned resources of type appStoreVersions (optional)
    fields_app_clip_default_experience_localizations = ['fields_app_clip_default_experience_localizations_example'] # List[str] | the fields to include for returned resources of type appClipDefaultExperienceLocalizations (optional)
    fields_app_clip_app_store_review_details = ['fields_app_clip_app_store_review_details_example'] # List[str] | the fields to include for returned resources of type appClipAppStoreReviewDetails (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_clip_default_experience_localizations = 56 # int | maximum number of related appClipDefaultExperienceLocalizations returned (when they are included) (optional)

    try:
        api_response = api_instance.app_clip_default_experiences_get_instance(id, fields_app_clip_default_experiences=fields_app_clip_default_experiences, fields_app_store_versions=fields_app_store_versions, fields_app_clip_default_experience_localizations=fields_app_clip_default_experience_localizations, fields_app_clip_app_store_review_details=fields_app_clip_app_store_review_details, include=include, limit_app_clip_default_experience_localizations=limit_app_clip_default_experience_localizations)
        print("The response of AppClipDefaultExperiencesApi->app_clip_default_experiences_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipDefaultExperiencesApi->app_clip_default_experiences_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_clip_default_experiences** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipDefaultExperiences | [optional] 
 **fields_app_store_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersions | [optional] 
 **fields_app_clip_default_experience_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipDefaultExperienceLocalizations | [optional] 
 **fields_app_clip_app_store_review_details** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipAppStoreReviewDetails | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_clip_default_experience_localizations** | **int**| maximum number of related appClipDefaultExperienceLocalizations returned (when they are included) | [optional] 

### Return type

[**AppClipDefaultExperienceResponse**](AppClipDefaultExperienceResponse.md)

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
**200** | Single AppClipDefaultExperience |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_clip_default_experiences_release_with_app_store_version_get_to_one_related**
> AppStoreVersionResponse app_clip_default_experiences_release_with_app_store_version_get_to_one_related(id, fields_app_store_versions=fields_app_store_versions, fields_apps=fields_apps, fields_age_rating_declarations=fields_age_rating_declarations, fields_app_store_version_localizations=fields_app_store_version_localizations, fields_builds=fields_builds, fields_app_store_version_phased_releases=fields_app_store_version_phased_releases, fields_game_center_app_versions=fields_game_center_app_versions, fields_routing_app_coverages=fields_routing_app_coverages, fields_app_store_review_details=fields_app_store_review_details, fields_app_store_version_submissions=fields_app_store_version_submissions, fields_app_clip_default_experiences=fields_app_clip_default_experiences, fields_app_store_version_experiments=fields_app_store_version_experiments, fields_alternative_distribution_packages=fields_alternative_distribution_packages, include=include, limit_app_store_version_localizations=limit_app_store_version_localizations, limit_app_store_version_experiments=limit_app_store_version_experiments, limit_app_store_version_experiments_v2=limit_app_store_version_experiments_v2)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_response import AppStoreVersionResponse
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
    api_instance = openapi_client.AppClipDefaultExperiencesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_store_versions = ['fields_app_store_versions_example'] # List[str] | the fields to include for returned resources of type appStoreVersions (optional)
    fields_apps = ['fields_apps_example'] # List[str] | the fields to include for returned resources of type apps (optional)
    fields_age_rating_declarations = ['fields_age_rating_declarations_example'] # List[str] | the fields to include for returned resources of type ageRatingDeclarations (optional)
    fields_app_store_version_localizations = ['fields_app_store_version_localizations_example'] # List[str] | the fields to include for returned resources of type appStoreVersionLocalizations (optional)
    fields_builds = ['fields_builds_example'] # List[str] | the fields to include for returned resources of type builds (optional)
    fields_app_store_version_phased_releases = ['fields_app_store_version_phased_releases_example'] # List[str] | the fields to include for returned resources of type appStoreVersionPhasedReleases (optional)
    fields_game_center_app_versions = ['fields_game_center_app_versions_example'] # List[str] | the fields to include for returned resources of type gameCenterAppVersions (optional)
    fields_routing_app_coverages = ['fields_routing_app_coverages_example'] # List[str] | the fields to include for returned resources of type routingAppCoverages (optional)
    fields_app_store_review_details = ['fields_app_store_review_details_example'] # List[str] | the fields to include for returned resources of type appStoreReviewDetails (optional)
    fields_app_store_version_submissions = ['fields_app_store_version_submissions_example'] # List[str] | the fields to include for returned resources of type appStoreVersionSubmissions (optional)
    fields_app_clip_default_experiences = ['fields_app_clip_default_experiences_example'] # List[str] | the fields to include for returned resources of type appClipDefaultExperiences (optional)
    fields_app_store_version_experiments = ['fields_app_store_version_experiments_example'] # List[str] | the fields to include for returned resources of type appStoreVersionExperiments (optional)
    fields_alternative_distribution_packages = ['fields_alternative_distribution_packages_example'] # List[str] | the fields to include for returned resources of type alternativeDistributionPackages (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_store_version_localizations = 56 # int | maximum number of related appStoreVersionLocalizations returned (when they are included) (optional)
    limit_app_store_version_experiments = 56 # int | maximum number of related appStoreVersionExperiments returned (when they are included) (optional)
    limit_app_store_version_experiments_v2 = 56 # int | maximum number of related appStoreVersionExperimentsV2 returned (when they are included) (optional)

    try:
        api_response = api_instance.app_clip_default_experiences_release_with_app_store_version_get_to_one_related(id, fields_app_store_versions=fields_app_store_versions, fields_apps=fields_apps, fields_age_rating_declarations=fields_age_rating_declarations, fields_app_store_version_localizations=fields_app_store_version_localizations, fields_builds=fields_builds, fields_app_store_version_phased_releases=fields_app_store_version_phased_releases, fields_game_center_app_versions=fields_game_center_app_versions, fields_routing_app_coverages=fields_routing_app_coverages, fields_app_store_review_details=fields_app_store_review_details, fields_app_store_version_submissions=fields_app_store_version_submissions, fields_app_clip_default_experiences=fields_app_clip_default_experiences, fields_app_store_version_experiments=fields_app_store_version_experiments, fields_alternative_distribution_packages=fields_alternative_distribution_packages, include=include, limit_app_store_version_localizations=limit_app_store_version_localizations, limit_app_store_version_experiments=limit_app_store_version_experiments, limit_app_store_version_experiments_v2=limit_app_store_version_experiments_v2)
        print("The response of AppClipDefaultExperiencesApi->app_clip_default_experiences_release_with_app_store_version_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipDefaultExperiencesApi->app_clip_default_experiences_release_with_app_store_version_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_store_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersions | [optional] 
 **fields_apps** | [**List[str]**](str.md)| the fields to include for returned resources of type apps | [optional] 
 **fields_age_rating_declarations** | [**List[str]**](str.md)| the fields to include for returned resources of type ageRatingDeclarations | [optional] 
 **fields_app_store_version_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionLocalizations | [optional] 
 **fields_builds** | [**List[str]**](str.md)| the fields to include for returned resources of type builds | [optional] 
 **fields_app_store_version_phased_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionPhasedReleases | [optional] 
 **fields_game_center_app_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAppVersions | [optional] 
 **fields_routing_app_coverages** | [**List[str]**](str.md)| the fields to include for returned resources of type routingAppCoverages | [optional] 
 **fields_app_store_review_details** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreReviewDetails | [optional] 
 **fields_app_store_version_submissions** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionSubmissions | [optional] 
 **fields_app_clip_default_experiences** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipDefaultExperiences | [optional] 
 **fields_app_store_version_experiments** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionExperiments | [optional] 
 **fields_alternative_distribution_packages** | [**List[str]**](str.md)| the fields to include for returned resources of type alternativeDistributionPackages | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_store_version_localizations** | **int**| maximum number of related appStoreVersionLocalizations returned (when they are included) | [optional] 
 **limit_app_store_version_experiments** | **int**| maximum number of related appStoreVersionExperiments returned (when they are included) | [optional] 
 **limit_app_store_version_experiments_v2** | **int**| maximum number of related appStoreVersionExperimentsV2 returned (when they are included) | [optional] 

### Return type

[**AppStoreVersionResponse**](AppStoreVersionResponse.md)

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
**200** | Single AppStoreVersion |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_clip_default_experiences_release_with_app_store_version_get_to_one_relationship**
> AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageResponse app_clip_default_experiences_release_with_app_store_version_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_default_experience_release_with_app_store_version_linkage_response import AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageResponse
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
    api_instance = openapi_client.AppClipDefaultExperiencesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.app_clip_default_experiences_release_with_app_store_version_get_to_one_relationship(id)
        print("The response of AppClipDefaultExperiencesApi->app_clip_default_experiences_release_with_app_store_version_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipDefaultExperiencesApi->app_clip_default_experiences_release_with_app_store_version_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageResponse**](AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageResponse.md)

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

# **app_clip_default_experiences_release_with_app_store_version_update_to_one_relationship**
> app_clip_default_experiences_release_with_app_store_version_update_to_one_relationship(id, app_clip_default_experience_release_with_app_store_version_linkage_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_default_experience_release_with_app_store_version_linkage_request import AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageRequest
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
    api_instance = openapi_client.AppClipDefaultExperiencesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    app_clip_default_experience_release_with_app_store_version_linkage_request = openapi_client.AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageRequest() # AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageRequest | Related linkage

    try:
        api_instance.app_clip_default_experiences_release_with_app_store_version_update_to_one_relationship(id, app_clip_default_experience_release_with_app_store_version_linkage_request)
    except Exception as e:
        print("Exception when calling AppClipDefaultExperiencesApi->app_clip_default_experiences_release_with_app_store_version_update_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **app_clip_default_experience_release_with_app_store_version_linkage_request** | [**AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageRequest**](AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageRequest.md)| Related linkage | 

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**422** | Unprocessable request entity error(s) |  -  |
**409** | Request entity error(s) |  -  |
**204** | Success (no content) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_clip_default_experiences_update_instance**
> AppClipDefaultExperienceResponse app_clip_default_experiences_update_instance(id, app_clip_default_experience_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_default_experience_response import AppClipDefaultExperienceResponse
from openapi_client.models.app_clip_default_experience_update_request import AppClipDefaultExperienceUpdateRequest
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
    api_instance = openapi_client.AppClipDefaultExperiencesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    app_clip_default_experience_update_request = openapi_client.AppClipDefaultExperienceUpdateRequest() # AppClipDefaultExperienceUpdateRequest | AppClipDefaultExperience representation

    try:
        api_response = api_instance.app_clip_default_experiences_update_instance(id, app_clip_default_experience_update_request)
        print("The response of AppClipDefaultExperiencesApi->app_clip_default_experiences_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipDefaultExperiencesApi->app_clip_default_experiences_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **app_clip_default_experience_update_request** | [**AppClipDefaultExperienceUpdateRequest**](AppClipDefaultExperienceUpdateRequest.md)| AppClipDefaultExperience representation | 

### Return type

[**AppClipDefaultExperienceResponse**](AppClipDefaultExperienceResponse.md)

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
**200** | Single AppClipDefaultExperience |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

