# openapi_client.AppCustomProductPageVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**app_custom_product_page_versions_app_custom_product_page_localizations_get_to_many_related**](AppCustomProductPageVersionsApi.md#app_custom_product_page_versions_app_custom_product_page_localizations_get_to_many_related) | **GET** /v1/appCustomProductPageVersions/{id}/appCustomProductPageLocalizations | 
[**app_custom_product_page_versions_app_custom_product_page_localizations_get_to_many_relationship**](AppCustomProductPageVersionsApi.md#app_custom_product_page_versions_app_custom_product_page_localizations_get_to_many_relationship) | **GET** /v1/appCustomProductPageVersions/{id}/relationships/appCustomProductPageLocalizations | 
[**app_custom_product_page_versions_create_instance**](AppCustomProductPageVersionsApi.md#app_custom_product_page_versions_create_instance) | **POST** /v1/appCustomProductPageVersions | 
[**app_custom_product_page_versions_get_instance**](AppCustomProductPageVersionsApi.md#app_custom_product_page_versions_get_instance) | **GET** /v1/appCustomProductPageVersions/{id} | 
[**app_custom_product_page_versions_update_instance**](AppCustomProductPageVersionsApi.md#app_custom_product_page_versions_update_instance) | **PATCH** /v1/appCustomProductPageVersions/{id} | 


# **app_custom_product_page_versions_app_custom_product_page_localizations_get_to_many_related**
> AppCustomProductPageLocalizationsResponse app_custom_product_page_versions_app_custom_product_page_localizations_get_to_many_related(id, filter_locale=filter_locale, fields_app_custom_product_page_localizations=fields_app_custom_product_page_localizations, fields_app_custom_product_page_versions=fields_app_custom_product_page_versions, fields_app_screenshot_sets=fields_app_screenshot_sets, fields_app_preview_sets=fields_app_preview_sets, limit=limit, include=include, limit_app_screenshot_sets=limit_app_screenshot_sets, limit_app_preview_sets=limit_app_preview_sets)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_custom_product_page_localizations_response import AppCustomProductPageLocalizationsResponse
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
    api_instance = openapi_client.AppCustomProductPageVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_locale = ['filter_locale_example'] # List[str] | filter by attribute 'locale' (optional)
    fields_app_custom_product_page_localizations = ['fields_app_custom_product_page_localizations_example'] # List[str] | the fields to include for returned resources of type appCustomProductPageLocalizations (optional)
    fields_app_custom_product_page_versions = ['fields_app_custom_product_page_versions_example'] # List[str] | the fields to include for returned resources of type appCustomProductPageVersions (optional)
    fields_app_screenshot_sets = ['fields_app_screenshot_sets_example'] # List[str] | the fields to include for returned resources of type appScreenshotSets (optional)
    fields_app_preview_sets = ['fields_app_preview_sets_example'] # List[str] | the fields to include for returned resources of type appPreviewSets (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_screenshot_sets = 56 # int | maximum number of related appScreenshotSets returned (when they are included) (optional)
    limit_app_preview_sets = 56 # int | maximum number of related appPreviewSets returned (when they are included) (optional)

    try:
        api_response = api_instance.app_custom_product_page_versions_app_custom_product_page_localizations_get_to_many_related(id, filter_locale=filter_locale, fields_app_custom_product_page_localizations=fields_app_custom_product_page_localizations, fields_app_custom_product_page_versions=fields_app_custom_product_page_versions, fields_app_screenshot_sets=fields_app_screenshot_sets, fields_app_preview_sets=fields_app_preview_sets, limit=limit, include=include, limit_app_screenshot_sets=limit_app_screenshot_sets, limit_app_preview_sets=limit_app_preview_sets)
        print("The response of AppCustomProductPageVersionsApi->app_custom_product_page_versions_app_custom_product_page_localizations_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppCustomProductPageVersionsApi->app_custom_product_page_versions_app_custom_product_page_localizations_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_locale** | [**List[str]**](str.md)| filter by attribute &#39;locale&#39; | [optional] 
 **fields_app_custom_product_page_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appCustomProductPageLocalizations | [optional] 
 **fields_app_custom_product_page_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type appCustomProductPageVersions | [optional] 
 **fields_app_screenshot_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type appScreenshotSets | [optional] 
 **fields_app_preview_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type appPreviewSets | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_screenshot_sets** | **int**| maximum number of related appScreenshotSets returned (when they are included) | [optional] 
 **limit_app_preview_sets** | **int**| maximum number of related appPreviewSets returned (when they are included) | [optional] 

### Return type

[**AppCustomProductPageLocalizationsResponse**](AppCustomProductPageLocalizationsResponse.md)

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
**200** | List of AppCustomProductPageLocalizations |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_custom_product_page_versions_app_custom_product_page_localizations_get_to_many_relationship**
> AppCustomProductPageVersionAppCustomProductPageLocalizationsLinkagesResponse app_custom_product_page_versions_app_custom_product_page_localizations_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_custom_product_page_version_app_custom_product_page_localizations_linkages_response import AppCustomProductPageVersionAppCustomProductPageLocalizationsLinkagesResponse
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
    api_instance = openapi_client.AppCustomProductPageVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.app_custom_product_page_versions_app_custom_product_page_localizations_get_to_many_relationship(id, limit=limit)
        print("The response of AppCustomProductPageVersionsApi->app_custom_product_page_versions_app_custom_product_page_localizations_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppCustomProductPageVersionsApi->app_custom_product_page_versions_app_custom_product_page_localizations_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AppCustomProductPageVersionAppCustomProductPageLocalizationsLinkagesResponse**](AppCustomProductPageVersionAppCustomProductPageLocalizationsLinkagesResponse.md)

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

# **app_custom_product_page_versions_create_instance**
> AppCustomProductPageVersionResponse app_custom_product_page_versions_create_instance(app_custom_product_page_version_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_custom_product_page_version_create_request import AppCustomProductPageVersionCreateRequest
from openapi_client.models.app_custom_product_page_version_response import AppCustomProductPageVersionResponse
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
    api_instance = openapi_client.AppCustomProductPageVersionsApi(api_client)
    app_custom_product_page_version_create_request = openapi_client.AppCustomProductPageVersionCreateRequest() # AppCustomProductPageVersionCreateRequest | AppCustomProductPageVersion representation

    try:
        api_response = api_instance.app_custom_product_page_versions_create_instance(app_custom_product_page_version_create_request)
        print("The response of AppCustomProductPageVersionsApi->app_custom_product_page_versions_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppCustomProductPageVersionsApi->app_custom_product_page_versions_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **app_custom_product_page_version_create_request** | [**AppCustomProductPageVersionCreateRequest**](AppCustomProductPageVersionCreateRequest.md)| AppCustomProductPageVersion representation | 

### Return type

[**AppCustomProductPageVersionResponse**](AppCustomProductPageVersionResponse.md)

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
**201** | Single AppCustomProductPageVersion |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_custom_product_page_versions_get_instance**
> AppCustomProductPageVersionResponse app_custom_product_page_versions_get_instance(id, fields_app_custom_product_page_versions=fields_app_custom_product_page_versions, fields_app_custom_product_page_localizations=fields_app_custom_product_page_localizations, include=include, limit_app_custom_product_page_localizations=limit_app_custom_product_page_localizations)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_custom_product_page_version_response import AppCustomProductPageVersionResponse
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
    api_instance = openapi_client.AppCustomProductPageVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_custom_product_page_versions = ['fields_app_custom_product_page_versions_example'] # List[str] | the fields to include for returned resources of type appCustomProductPageVersions (optional)
    fields_app_custom_product_page_localizations = ['fields_app_custom_product_page_localizations_example'] # List[str] | the fields to include for returned resources of type appCustomProductPageLocalizations (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_custom_product_page_localizations = 56 # int | maximum number of related appCustomProductPageLocalizations returned (when they are included) (optional)

    try:
        api_response = api_instance.app_custom_product_page_versions_get_instance(id, fields_app_custom_product_page_versions=fields_app_custom_product_page_versions, fields_app_custom_product_page_localizations=fields_app_custom_product_page_localizations, include=include, limit_app_custom_product_page_localizations=limit_app_custom_product_page_localizations)
        print("The response of AppCustomProductPageVersionsApi->app_custom_product_page_versions_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppCustomProductPageVersionsApi->app_custom_product_page_versions_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_custom_product_page_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type appCustomProductPageVersions | [optional] 
 **fields_app_custom_product_page_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appCustomProductPageLocalizations | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_custom_product_page_localizations** | **int**| maximum number of related appCustomProductPageLocalizations returned (when they are included) | [optional] 

### Return type

[**AppCustomProductPageVersionResponse**](AppCustomProductPageVersionResponse.md)

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
**200** | Single AppCustomProductPageVersion |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_custom_product_page_versions_update_instance**
> AppCustomProductPageVersionResponse app_custom_product_page_versions_update_instance(id, app_custom_product_page_version_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_custom_product_page_version_response import AppCustomProductPageVersionResponse
from openapi_client.models.app_custom_product_page_version_update_request import AppCustomProductPageVersionUpdateRequest
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
    api_instance = openapi_client.AppCustomProductPageVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    app_custom_product_page_version_update_request = openapi_client.AppCustomProductPageVersionUpdateRequest() # AppCustomProductPageVersionUpdateRequest | AppCustomProductPageVersion representation

    try:
        api_response = api_instance.app_custom_product_page_versions_update_instance(id, app_custom_product_page_version_update_request)
        print("The response of AppCustomProductPageVersionsApi->app_custom_product_page_versions_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppCustomProductPageVersionsApi->app_custom_product_page_versions_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **app_custom_product_page_version_update_request** | [**AppCustomProductPageVersionUpdateRequest**](AppCustomProductPageVersionUpdateRequest.md)| AppCustomProductPageVersion representation | 

### Return type

[**AppCustomProductPageVersionResponse**](AppCustomProductPageVersionResponse.md)

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
**200** | Single AppCustomProductPageVersion |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

