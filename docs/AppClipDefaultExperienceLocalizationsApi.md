# openapi_client.AppClipDefaultExperienceLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**app_clip_default_experience_localizations_app_clip_header_image_get_to_one_related**](AppClipDefaultExperienceLocalizationsApi.md#app_clip_default_experience_localizations_app_clip_header_image_get_to_one_related) | **GET** /v1/appClipDefaultExperienceLocalizations/{id}/appClipHeaderImage | 
[**app_clip_default_experience_localizations_app_clip_header_image_get_to_one_relationship**](AppClipDefaultExperienceLocalizationsApi.md#app_clip_default_experience_localizations_app_clip_header_image_get_to_one_relationship) | **GET** /v1/appClipDefaultExperienceLocalizations/{id}/relationships/appClipHeaderImage | 
[**app_clip_default_experience_localizations_create_instance**](AppClipDefaultExperienceLocalizationsApi.md#app_clip_default_experience_localizations_create_instance) | **POST** /v1/appClipDefaultExperienceLocalizations | 
[**app_clip_default_experience_localizations_delete_instance**](AppClipDefaultExperienceLocalizationsApi.md#app_clip_default_experience_localizations_delete_instance) | **DELETE** /v1/appClipDefaultExperienceLocalizations/{id} | 
[**app_clip_default_experience_localizations_get_instance**](AppClipDefaultExperienceLocalizationsApi.md#app_clip_default_experience_localizations_get_instance) | **GET** /v1/appClipDefaultExperienceLocalizations/{id} | 
[**app_clip_default_experience_localizations_update_instance**](AppClipDefaultExperienceLocalizationsApi.md#app_clip_default_experience_localizations_update_instance) | **PATCH** /v1/appClipDefaultExperienceLocalizations/{id} | 


# **app_clip_default_experience_localizations_app_clip_header_image_get_to_one_related**
> AppClipHeaderImageResponse app_clip_default_experience_localizations_app_clip_header_image_get_to_one_related(id, fields_app_clip_header_images=fields_app_clip_header_images, fields_app_clip_default_experience_localizations=fields_app_clip_default_experience_localizations, include=include)

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
    api_instance = openapi_client.AppClipDefaultExperienceLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_clip_header_images = ['fields_app_clip_header_images_example'] # List[str] | the fields to include for returned resources of type appClipHeaderImages (optional)
    fields_app_clip_default_experience_localizations = ['fields_app_clip_default_experience_localizations_example'] # List[str] | the fields to include for returned resources of type appClipDefaultExperienceLocalizations (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.app_clip_default_experience_localizations_app_clip_header_image_get_to_one_related(id, fields_app_clip_header_images=fields_app_clip_header_images, fields_app_clip_default_experience_localizations=fields_app_clip_default_experience_localizations, include=include)
        print("The response of AppClipDefaultExperienceLocalizationsApi->app_clip_default_experience_localizations_app_clip_header_image_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipDefaultExperienceLocalizationsApi->app_clip_default_experience_localizations_app_clip_header_image_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_clip_header_images** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipHeaderImages | [optional] 
 **fields_app_clip_default_experience_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipDefaultExperienceLocalizations | [optional] 
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

# **app_clip_default_experience_localizations_app_clip_header_image_get_to_one_relationship**
> AppClipDefaultExperienceLocalizationAppClipHeaderImageLinkageResponse app_clip_default_experience_localizations_app_clip_header_image_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_default_experience_localization_app_clip_header_image_linkage_response import AppClipDefaultExperienceLocalizationAppClipHeaderImageLinkageResponse
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
    api_instance = openapi_client.AppClipDefaultExperienceLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.app_clip_default_experience_localizations_app_clip_header_image_get_to_one_relationship(id)
        print("The response of AppClipDefaultExperienceLocalizationsApi->app_clip_default_experience_localizations_app_clip_header_image_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipDefaultExperienceLocalizationsApi->app_clip_default_experience_localizations_app_clip_header_image_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**AppClipDefaultExperienceLocalizationAppClipHeaderImageLinkageResponse**](AppClipDefaultExperienceLocalizationAppClipHeaderImageLinkageResponse.md)

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

# **app_clip_default_experience_localizations_create_instance**
> AppClipDefaultExperienceLocalizationResponse app_clip_default_experience_localizations_create_instance(app_clip_default_experience_localization_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_default_experience_localization_create_request import AppClipDefaultExperienceLocalizationCreateRequest
from openapi_client.models.app_clip_default_experience_localization_response import AppClipDefaultExperienceLocalizationResponse
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
    api_instance = openapi_client.AppClipDefaultExperienceLocalizationsApi(api_client)
    app_clip_default_experience_localization_create_request = openapi_client.AppClipDefaultExperienceLocalizationCreateRequest() # AppClipDefaultExperienceLocalizationCreateRequest | AppClipDefaultExperienceLocalization representation

    try:
        api_response = api_instance.app_clip_default_experience_localizations_create_instance(app_clip_default_experience_localization_create_request)
        print("The response of AppClipDefaultExperienceLocalizationsApi->app_clip_default_experience_localizations_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipDefaultExperienceLocalizationsApi->app_clip_default_experience_localizations_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **app_clip_default_experience_localization_create_request** | [**AppClipDefaultExperienceLocalizationCreateRequest**](AppClipDefaultExperienceLocalizationCreateRequest.md)| AppClipDefaultExperienceLocalization representation | 

### Return type

[**AppClipDefaultExperienceLocalizationResponse**](AppClipDefaultExperienceLocalizationResponse.md)

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
**201** | Single AppClipDefaultExperienceLocalization |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_clip_default_experience_localizations_delete_instance**
> app_clip_default_experience_localizations_delete_instance(id)

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
    api_instance = openapi_client.AppClipDefaultExperienceLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.app_clip_default_experience_localizations_delete_instance(id)
    except Exception as e:
        print("Exception when calling AppClipDefaultExperienceLocalizationsApi->app_clip_default_experience_localizations_delete_instance: %s\n" % e)
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

# **app_clip_default_experience_localizations_get_instance**
> AppClipDefaultExperienceLocalizationResponse app_clip_default_experience_localizations_get_instance(id, fields_app_clip_default_experience_localizations=fields_app_clip_default_experience_localizations, fields_app_clip_header_images=fields_app_clip_header_images, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_default_experience_localization_response import AppClipDefaultExperienceLocalizationResponse
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
    api_instance = openapi_client.AppClipDefaultExperienceLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_clip_default_experience_localizations = ['fields_app_clip_default_experience_localizations_example'] # List[str] | the fields to include for returned resources of type appClipDefaultExperienceLocalizations (optional)
    fields_app_clip_header_images = ['fields_app_clip_header_images_example'] # List[str] | the fields to include for returned resources of type appClipHeaderImages (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.app_clip_default_experience_localizations_get_instance(id, fields_app_clip_default_experience_localizations=fields_app_clip_default_experience_localizations, fields_app_clip_header_images=fields_app_clip_header_images, include=include)
        print("The response of AppClipDefaultExperienceLocalizationsApi->app_clip_default_experience_localizations_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipDefaultExperienceLocalizationsApi->app_clip_default_experience_localizations_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_clip_default_experience_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipDefaultExperienceLocalizations | [optional] 
 **fields_app_clip_header_images** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipHeaderImages | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**AppClipDefaultExperienceLocalizationResponse**](AppClipDefaultExperienceLocalizationResponse.md)

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
**200** | Single AppClipDefaultExperienceLocalization |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_clip_default_experience_localizations_update_instance**
> AppClipDefaultExperienceLocalizationResponse app_clip_default_experience_localizations_update_instance(id, app_clip_default_experience_localization_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_clip_default_experience_localization_response import AppClipDefaultExperienceLocalizationResponse
from openapi_client.models.app_clip_default_experience_localization_update_request import AppClipDefaultExperienceLocalizationUpdateRequest
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
    api_instance = openapi_client.AppClipDefaultExperienceLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    app_clip_default_experience_localization_update_request = openapi_client.AppClipDefaultExperienceLocalizationUpdateRequest() # AppClipDefaultExperienceLocalizationUpdateRequest | AppClipDefaultExperienceLocalization representation

    try:
        api_response = api_instance.app_clip_default_experience_localizations_update_instance(id, app_clip_default_experience_localization_update_request)
        print("The response of AppClipDefaultExperienceLocalizationsApi->app_clip_default_experience_localizations_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppClipDefaultExperienceLocalizationsApi->app_clip_default_experience_localizations_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **app_clip_default_experience_localization_update_request** | [**AppClipDefaultExperienceLocalizationUpdateRequest**](AppClipDefaultExperienceLocalizationUpdateRequest.md)| AppClipDefaultExperienceLocalization representation | 

### Return type

[**AppClipDefaultExperienceLocalizationResponse**](AppClipDefaultExperienceLocalizationResponse.md)

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
**200** | Single AppClipDefaultExperienceLocalization |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

