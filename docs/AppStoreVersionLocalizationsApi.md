# openapi_client.AppStoreVersionLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**app_store_version_localizations_app_preview_sets_get_to_many_related**](AppStoreVersionLocalizationsApi.md#app_store_version_localizations_app_preview_sets_get_to_many_related) | **GET** /v1/appStoreVersionLocalizations/{id}/appPreviewSets | 
[**app_store_version_localizations_app_preview_sets_get_to_many_relationship**](AppStoreVersionLocalizationsApi.md#app_store_version_localizations_app_preview_sets_get_to_many_relationship) | **GET** /v1/appStoreVersionLocalizations/{id}/relationships/appPreviewSets | 
[**app_store_version_localizations_app_screenshot_sets_get_to_many_related**](AppStoreVersionLocalizationsApi.md#app_store_version_localizations_app_screenshot_sets_get_to_many_related) | **GET** /v1/appStoreVersionLocalizations/{id}/appScreenshotSets | 
[**app_store_version_localizations_app_screenshot_sets_get_to_many_relationship**](AppStoreVersionLocalizationsApi.md#app_store_version_localizations_app_screenshot_sets_get_to_many_relationship) | **GET** /v1/appStoreVersionLocalizations/{id}/relationships/appScreenshotSets | 
[**app_store_version_localizations_create_instance**](AppStoreVersionLocalizationsApi.md#app_store_version_localizations_create_instance) | **POST** /v1/appStoreVersionLocalizations | 
[**app_store_version_localizations_delete_instance**](AppStoreVersionLocalizationsApi.md#app_store_version_localizations_delete_instance) | **DELETE** /v1/appStoreVersionLocalizations/{id} | 
[**app_store_version_localizations_get_instance**](AppStoreVersionLocalizationsApi.md#app_store_version_localizations_get_instance) | **GET** /v1/appStoreVersionLocalizations/{id} | 
[**app_store_version_localizations_update_instance**](AppStoreVersionLocalizationsApi.md#app_store_version_localizations_update_instance) | **PATCH** /v1/appStoreVersionLocalizations/{id} | 


# **app_store_version_localizations_app_preview_sets_get_to_many_related**
> AppPreviewSetsResponse app_store_version_localizations_app_preview_sets_get_to_many_related(id, filter_preview_type=filter_preview_type, filter_app_custom_product_page_localization=filter_app_custom_product_page_localization, filter_app_store_version_experiment_treatment_localization=filter_app_store_version_experiment_treatment_localization, fields_app_preview_sets=fields_app_preview_sets, fields_app_store_version_localizations=fields_app_store_version_localizations, fields_app_custom_product_page_localizations=fields_app_custom_product_page_localizations, fields_app_store_version_experiment_treatment_localizations=fields_app_store_version_experiment_treatment_localizations, fields_app_previews=fields_app_previews, limit=limit, include=include, limit_app_previews=limit_app_previews)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_preview_sets_response import AppPreviewSetsResponse
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
    api_instance = openapi_client.AppStoreVersionLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_preview_type = ['filter_preview_type_example'] # List[str] | filter by attribute 'previewType' (optional)
    filter_app_custom_product_page_localization = ['filter_app_custom_product_page_localization_example'] # List[str] | filter by id(s) of related 'appCustomProductPageLocalization' (optional)
    filter_app_store_version_experiment_treatment_localization = ['filter_app_store_version_experiment_treatment_localization_example'] # List[str] | filter by id(s) of related 'appStoreVersionExperimentTreatmentLocalization' (optional)
    fields_app_preview_sets = ['fields_app_preview_sets_example'] # List[str] | the fields to include for returned resources of type appPreviewSets (optional)
    fields_app_store_version_localizations = ['fields_app_store_version_localizations_example'] # List[str] | the fields to include for returned resources of type appStoreVersionLocalizations (optional)
    fields_app_custom_product_page_localizations = ['fields_app_custom_product_page_localizations_example'] # List[str] | the fields to include for returned resources of type appCustomProductPageLocalizations (optional)
    fields_app_store_version_experiment_treatment_localizations = ['fields_app_store_version_experiment_treatment_localizations_example'] # List[str] | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations (optional)
    fields_app_previews = ['fields_app_previews_example'] # List[str] | the fields to include for returned resources of type appPreviews (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_previews = 56 # int | maximum number of related appPreviews returned (when they are included) (optional)

    try:
        api_response = api_instance.app_store_version_localizations_app_preview_sets_get_to_many_related(id, filter_preview_type=filter_preview_type, filter_app_custom_product_page_localization=filter_app_custom_product_page_localization, filter_app_store_version_experiment_treatment_localization=filter_app_store_version_experiment_treatment_localization, fields_app_preview_sets=fields_app_preview_sets, fields_app_store_version_localizations=fields_app_store_version_localizations, fields_app_custom_product_page_localizations=fields_app_custom_product_page_localizations, fields_app_store_version_experiment_treatment_localizations=fields_app_store_version_experiment_treatment_localizations, fields_app_previews=fields_app_previews, limit=limit, include=include, limit_app_previews=limit_app_previews)
        print("The response of AppStoreVersionLocalizationsApi->app_store_version_localizations_app_preview_sets_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionLocalizationsApi->app_store_version_localizations_app_preview_sets_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_preview_type** | [**List[str]**](str.md)| filter by attribute &#39;previewType&#39; | [optional] 
 **filter_app_custom_product_page_localization** | [**List[str]**](str.md)| filter by id(s) of related &#39;appCustomProductPageLocalization&#39; | [optional] 
 **filter_app_store_version_experiment_treatment_localization** | [**List[str]**](str.md)| filter by id(s) of related &#39;appStoreVersionExperimentTreatmentLocalization&#39; | [optional] 
 **fields_app_preview_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type appPreviewSets | [optional] 
 **fields_app_store_version_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionLocalizations | [optional] 
 **fields_app_custom_product_page_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appCustomProductPageLocalizations | [optional] 
 **fields_app_store_version_experiment_treatment_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations | [optional] 
 **fields_app_previews** | [**List[str]**](str.md)| the fields to include for returned resources of type appPreviews | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_previews** | **int**| maximum number of related appPreviews returned (when they are included) | [optional] 

### Return type

[**AppPreviewSetsResponse**](AppPreviewSetsResponse.md)

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
**200** | List of AppPreviewSets |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_store_version_localizations_app_preview_sets_get_to_many_relationship**
> AppStoreVersionLocalizationAppPreviewSetsLinkagesResponse app_store_version_localizations_app_preview_sets_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_localization_app_preview_sets_linkages_response import AppStoreVersionLocalizationAppPreviewSetsLinkagesResponse
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
    api_instance = openapi_client.AppStoreVersionLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.app_store_version_localizations_app_preview_sets_get_to_many_relationship(id, limit=limit)
        print("The response of AppStoreVersionLocalizationsApi->app_store_version_localizations_app_preview_sets_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionLocalizationsApi->app_store_version_localizations_app_preview_sets_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AppStoreVersionLocalizationAppPreviewSetsLinkagesResponse**](AppStoreVersionLocalizationAppPreviewSetsLinkagesResponse.md)

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

# **app_store_version_localizations_app_screenshot_sets_get_to_many_related**
> AppScreenshotSetsResponse app_store_version_localizations_app_screenshot_sets_get_to_many_related(id, filter_screenshot_display_type=filter_screenshot_display_type, filter_app_custom_product_page_localization=filter_app_custom_product_page_localization, filter_app_store_version_experiment_treatment_localization=filter_app_store_version_experiment_treatment_localization, fields_app_screenshot_sets=fields_app_screenshot_sets, fields_app_store_version_localizations=fields_app_store_version_localizations, fields_app_custom_product_page_localizations=fields_app_custom_product_page_localizations, fields_app_store_version_experiment_treatment_localizations=fields_app_store_version_experiment_treatment_localizations, fields_app_screenshots=fields_app_screenshots, limit=limit, include=include, limit_app_screenshots=limit_app_screenshots)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_screenshot_sets_response import AppScreenshotSetsResponse
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
    api_instance = openapi_client.AppStoreVersionLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_screenshot_display_type = ['filter_screenshot_display_type_example'] # List[str] | filter by attribute 'screenshotDisplayType' (optional)
    filter_app_custom_product_page_localization = ['filter_app_custom_product_page_localization_example'] # List[str] | filter by id(s) of related 'appCustomProductPageLocalization' (optional)
    filter_app_store_version_experiment_treatment_localization = ['filter_app_store_version_experiment_treatment_localization_example'] # List[str] | filter by id(s) of related 'appStoreVersionExperimentTreatmentLocalization' (optional)
    fields_app_screenshot_sets = ['fields_app_screenshot_sets_example'] # List[str] | the fields to include for returned resources of type appScreenshotSets (optional)
    fields_app_store_version_localizations = ['fields_app_store_version_localizations_example'] # List[str] | the fields to include for returned resources of type appStoreVersionLocalizations (optional)
    fields_app_custom_product_page_localizations = ['fields_app_custom_product_page_localizations_example'] # List[str] | the fields to include for returned resources of type appCustomProductPageLocalizations (optional)
    fields_app_store_version_experiment_treatment_localizations = ['fields_app_store_version_experiment_treatment_localizations_example'] # List[str] | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations (optional)
    fields_app_screenshots = ['fields_app_screenshots_example'] # List[str] | the fields to include for returned resources of type appScreenshots (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_screenshots = 56 # int | maximum number of related appScreenshots returned (when they are included) (optional)

    try:
        api_response = api_instance.app_store_version_localizations_app_screenshot_sets_get_to_many_related(id, filter_screenshot_display_type=filter_screenshot_display_type, filter_app_custom_product_page_localization=filter_app_custom_product_page_localization, filter_app_store_version_experiment_treatment_localization=filter_app_store_version_experiment_treatment_localization, fields_app_screenshot_sets=fields_app_screenshot_sets, fields_app_store_version_localizations=fields_app_store_version_localizations, fields_app_custom_product_page_localizations=fields_app_custom_product_page_localizations, fields_app_store_version_experiment_treatment_localizations=fields_app_store_version_experiment_treatment_localizations, fields_app_screenshots=fields_app_screenshots, limit=limit, include=include, limit_app_screenshots=limit_app_screenshots)
        print("The response of AppStoreVersionLocalizationsApi->app_store_version_localizations_app_screenshot_sets_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionLocalizationsApi->app_store_version_localizations_app_screenshot_sets_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_screenshot_display_type** | [**List[str]**](str.md)| filter by attribute &#39;screenshotDisplayType&#39; | [optional] 
 **filter_app_custom_product_page_localization** | [**List[str]**](str.md)| filter by id(s) of related &#39;appCustomProductPageLocalization&#39; | [optional] 
 **filter_app_store_version_experiment_treatment_localization** | [**List[str]**](str.md)| filter by id(s) of related &#39;appStoreVersionExperimentTreatmentLocalization&#39; | [optional] 
 **fields_app_screenshot_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type appScreenshotSets | [optional] 
 **fields_app_store_version_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionLocalizations | [optional] 
 **fields_app_custom_product_page_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appCustomProductPageLocalizations | [optional] 
 **fields_app_store_version_experiment_treatment_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations | [optional] 
 **fields_app_screenshots** | [**List[str]**](str.md)| the fields to include for returned resources of type appScreenshots | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_screenshots** | **int**| maximum number of related appScreenshots returned (when they are included) | [optional] 

### Return type

[**AppScreenshotSetsResponse**](AppScreenshotSetsResponse.md)

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
**200** | List of AppScreenshotSets |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_store_version_localizations_app_screenshot_sets_get_to_many_relationship**
> AppStoreVersionLocalizationAppScreenshotSetsLinkagesResponse app_store_version_localizations_app_screenshot_sets_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_localization_app_screenshot_sets_linkages_response import AppStoreVersionLocalizationAppScreenshotSetsLinkagesResponse
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
    api_instance = openapi_client.AppStoreVersionLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.app_store_version_localizations_app_screenshot_sets_get_to_many_relationship(id, limit=limit)
        print("The response of AppStoreVersionLocalizationsApi->app_store_version_localizations_app_screenshot_sets_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionLocalizationsApi->app_store_version_localizations_app_screenshot_sets_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AppStoreVersionLocalizationAppScreenshotSetsLinkagesResponse**](AppStoreVersionLocalizationAppScreenshotSetsLinkagesResponse.md)

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

# **app_store_version_localizations_create_instance**
> AppStoreVersionLocalizationResponse app_store_version_localizations_create_instance(app_store_version_localization_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_localization_create_request import AppStoreVersionLocalizationCreateRequest
from openapi_client.models.app_store_version_localization_response import AppStoreVersionLocalizationResponse
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
    api_instance = openapi_client.AppStoreVersionLocalizationsApi(api_client)
    app_store_version_localization_create_request = openapi_client.AppStoreVersionLocalizationCreateRequest() # AppStoreVersionLocalizationCreateRequest | AppStoreVersionLocalization representation

    try:
        api_response = api_instance.app_store_version_localizations_create_instance(app_store_version_localization_create_request)
        print("The response of AppStoreVersionLocalizationsApi->app_store_version_localizations_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionLocalizationsApi->app_store_version_localizations_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **app_store_version_localization_create_request** | [**AppStoreVersionLocalizationCreateRequest**](AppStoreVersionLocalizationCreateRequest.md)| AppStoreVersionLocalization representation | 

### Return type

[**AppStoreVersionLocalizationResponse**](AppStoreVersionLocalizationResponse.md)

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
**201** | Single AppStoreVersionLocalization |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_store_version_localizations_delete_instance**
> app_store_version_localizations_delete_instance(id)

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
    api_instance = openapi_client.AppStoreVersionLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.app_store_version_localizations_delete_instance(id)
    except Exception as e:
        print("Exception when calling AppStoreVersionLocalizationsApi->app_store_version_localizations_delete_instance: %s\n" % e)
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

# **app_store_version_localizations_get_instance**
> AppStoreVersionLocalizationResponse app_store_version_localizations_get_instance(id, fields_app_store_version_localizations=fields_app_store_version_localizations, fields_app_screenshot_sets=fields_app_screenshot_sets, fields_app_preview_sets=fields_app_preview_sets, include=include, limit_app_preview_sets=limit_app_preview_sets, limit_app_screenshot_sets=limit_app_screenshot_sets)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_localization_response import AppStoreVersionLocalizationResponse
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
    api_instance = openapi_client.AppStoreVersionLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_store_version_localizations = ['fields_app_store_version_localizations_example'] # List[str] | the fields to include for returned resources of type appStoreVersionLocalizations (optional)
    fields_app_screenshot_sets = ['fields_app_screenshot_sets_example'] # List[str] | the fields to include for returned resources of type appScreenshotSets (optional)
    fields_app_preview_sets = ['fields_app_preview_sets_example'] # List[str] | the fields to include for returned resources of type appPreviewSets (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_preview_sets = 56 # int | maximum number of related appPreviewSets returned (when they are included) (optional)
    limit_app_screenshot_sets = 56 # int | maximum number of related appScreenshotSets returned (when they are included) (optional)

    try:
        api_response = api_instance.app_store_version_localizations_get_instance(id, fields_app_store_version_localizations=fields_app_store_version_localizations, fields_app_screenshot_sets=fields_app_screenshot_sets, fields_app_preview_sets=fields_app_preview_sets, include=include, limit_app_preview_sets=limit_app_preview_sets, limit_app_screenshot_sets=limit_app_screenshot_sets)
        print("The response of AppStoreVersionLocalizationsApi->app_store_version_localizations_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionLocalizationsApi->app_store_version_localizations_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_store_version_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionLocalizations | [optional] 
 **fields_app_screenshot_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type appScreenshotSets | [optional] 
 **fields_app_preview_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type appPreviewSets | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_preview_sets** | **int**| maximum number of related appPreviewSets returned (when they are included) | [optional] 
 **limit_app_screenshot_sets** | **int**| maximum number of related appScreenshotSets returned (when they are included) | [optional] 

### Return type

[**AppStoreVersionLocalizationResponse**](AppStoreVersionLocalizationResponse.md)

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
**200** | Single AppStoreVersionLocalization |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_store_version_localizations_update_instance**
> AppStoreVersionLocalizationResponse app_store_version_localizations_update_instance(id, app_store_version_localization_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_localization_response import AppStoreVersionLocalizationResponse
from openapi_client.models.app_store_version_localization_update_request import AppStoreVersionLocalizationUpdateRequest
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
    api_instance = openapi_client.AppStoreVersionLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    app_store_version_localization_update_request = openapi_client.AppStoreVersionLocalizationUpdateRequest() # AppStoreVersionLocalizationUpdateRequest | AppStoreVersionLocalization representation

    try:
        api_response = api_instance.app_store_version_localizations_update_instance(id, app_store_version_localization_update_request)
        print("The response of AppStoreVersionLocalizationsApi->app_store_version_localizations_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionLocalizationsApi->app_store_version_localizations_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **app_store_version_localization_update_request** | [**AppStoreVersionLocalizationUpdateRequest**](AppStoreVersionLocalizationUpdateRequest.md)| AppStoreVersionLocalization representation | 

### Return type

[**AppStoreVersionLocalizationResponse**](AppStoreVersionLocalizationResponse.md)

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
**200** | Single AppStoreVersionLocalization |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

