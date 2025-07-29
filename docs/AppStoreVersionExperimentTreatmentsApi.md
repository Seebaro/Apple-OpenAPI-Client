# openapi_client.AppStoreVersionExperimentTreatmentsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**app_store_version_experiment_treatments_app_store_version_experiment_treatment_localizations_get_to_many_related**](AppStoreVersionExperimentTreatmentsApi.md#app_store_version_experiment_treatments_app_store_version_experiment_treatment_localizations_get_to_many_related) | **GET** /v1/appStoreVersionExperimentTreatments/{id}/appStoreVersionExperimentTreatmentLocalizations | 
[**app_store_version_experiment_treatments_app_store_version_experiment_treatment_localizations_get_to_many_relationship**](AppStoreVersionExperimentTreatmentsApi.md#app_store_version_experiment_treatments_app_store_version_experiment_treatment_localizations_get_to_many_relationship) | **GET** /v1/appStoreVersionExperimentTreatments/{id}/relationships/appStoreVersionExperimentTreatmentLocalizations | 
[**app_store_version_experiment_treatments_create_instance**](AppStoreVersionExperimentTreatmentsApi.md#app_store_version_experiment_treatments_create_instance) | **POST** /v1/appStoreVersionExperimentTreatments | 
[**app_store_version_experiment_treatments_delete_instance**](AppStoreVersionExperimentTreatmentsApi.md#app_store_version_experiment_treatments_delete_instance) | **DELETE** /v1/appStoreVersionExperimentTreatments/{id} | 
[**app_store_version_experiment_treatments_get_instance**](AppStoreVersionExperimentTreatmentsApi.md#app_store_version_experiment_treatments_get_instance) | **GET** /v1/appStoreVersionExperimentTreatments/{id} | 
[**app_store_version_experiment_treatments_update_instance**](AppStoreVersionExperimentTreatmentsApi.md#app_store_version_experiment_treatments_update_instance) | **PATCH** /v1/appStoreVersionExperimentTreatments/{id} | 


# **app_store_version_experiment_treatments_app_store_version_experiment_treatment_localizations_get_to_many_related**
> AppStoreVersionExperimentTreatmentLocalizationsResponse app_store_version_experiment_treatments_app_store_version_experiment_treatment_localizations_get_to_many_related(id, filter_locale=filter_locale, fields_app_store_version_experiment_treatment_localizations=fields_app_store_version_experiment_treatment_localizations, fields_app_store_version_experiment_treatments=fields_app_store_version_experiment_treatments, fields_app_screenshot_sets=fields_app_screenshot_sets, fields_app_preview_sets=fields_app_preview_sets, limit=limit, include=include, limit_app_screenshot_sets=limit_app_screenshot_sets, limit_app_preview_sets=limit_app_preview_sets)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_experiment_treatment_localizations_response import AppStoreVersionExperimentTreatmentLocalizationsResponse
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
    api_instance = openapi_client.AppStoreVersionExperimentTreatmentsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_locale = ['filter_locale_example'] # List[str] | filter by attribute 'locale' (optional)
    fields_app_store_version_experiment_treatment_localizations = ['fields_app_store_version_experiment_treatment_localizations_example'] # List[str] | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations (optional)
    fields_app_store_version_experiment_treatments = ['fields_app_store_version_experiment_treatments_example'] # List[str] | the fields to include for returned resources of type appStoreVersionExperimentTreatments (optional)
    fields_app_screenshot_sets = ['fields_app_screenshot_sets_example'] # List[str] | the fields to include for returned resources of type appScreenshotSets (optional)
    fields_app_preview_sets = ['fields_app_preview_sets_example'] # List[str] | the fields to include for returned resources of type appPreviewSets (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_screenshot_sets = 56 # int | maximum number of related appScreenshotSets returned (when they are included) (optional)
    limit_app_preview_sets = 56 # int | maximum number of related appPreviewSets returned (when they are included) (optional)

    try:
        api_response = api_instance.app_store_version_experiment_treatments_app_store_version_experiment_treatment_localizations_get_to_many_related(id, filter_locale=filter_locale, fields_app_store_version_experiment_treatment_localizations=fields_app_store_version_experiment_treatment_localizations, fields_app_store_version_experiment_treatments=fields_app_store_version_experiment_treatments, fields_app_screenshot_sets=fields_app_screenshot_sets, fields_app_preview_sets=fields_app_preview_sets, limit=limit, include=include, limit_app_screenshot_sets=limit_app_screenshot_sets, limit_app_preview_sets=limit_app_preview_sets)
        print("The response of AppStoreVersionExperimentTreatmentsApi->app_store_version_experiment_treatments_app_store_version_experiment_treatment_localizations_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionExperimentTreatmentsApi->app_store_version_experiment_treatments_app_store_version_experiment_treatment_localizations_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_locale** | [**List[str]**](str.md)| filter by attribute &#39;locale&#39; | [optional] 
 **fields_app_store_version_experiment_treatment_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations | [optional] 
 **fields_app_store_version_experiment_treatments** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionExperimentTreatments | [optional] 
 **fields_app_screenshot_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type appScreenshotSets | [optional] 
 **fields_app_preview_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type appPreviewSets | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_screenshot_sets** | **int**| maximum number of related appScreenshotSets returned (when they are included) | [optional] 
 **limit_app_preview_sets** | **int**| maximum number of related appPreviewSets returned (when they are included) | [optional] 

### Return type

[**AppStoreVersionExperimentTreatmentLocalizationsResponse**](AppStoreVersionExperimentTreatmentLocalizationsResponse.md)

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
**200** | List of AppStoreVersionExperimentTreatmentLocalizations |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_store_version_experiment_treatments_app_store_version_experiment_treatment_localizations_get_to_many_relationship**
> AppStoreVersionExperimentTreatmentAppStoreVersionExperimentTreatmentLocalizationsLinkagesResponse app_store_version_experiment_treatments_app_store_version_experiment_treatment_localizations_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_experiment_treatment_app_store_version_experiment_treatment_localizations_linkages_response import AppStoreVersionExperimentTreatmentAppStoreVersionExperimentTreatmentLocalizationsLinkagesResponse
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
    api_instance = openapi_client.AppStoreVersionExperimentTreatmentsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.app_store_version_experiment_treatments_app_store_version_experiment_treatment_localizations_get_to_many_relationship(id, limit=limit)
        print("The response of AppStoreVersionExperimentTreatmentsApi->app_store_version_experiment_treatments_app_store_version_experiment_treatment_localizations_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionExperimentTreatmentsApi->app_store_version_experiment_treatments_app_store_version_experiment_treatment_localizations_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AppStoreVersionExperimentTreatmentAppStoreVersionExperimentTreatmentLocalizationsLinkagesResponse**](AppStoreVersionExperimentTreatmentAppStoreVersionExperimentTreatmentLocalizationsLinkagesResponse.md)

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

# **app_store_version_experiment_treatments_create_instance**
> AppStoreVersionExperimentTreatmentResponse app_store_version_experiment_treatments_create_instance(app_store_version_experiment_treatment_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_experiment_treatment_create_request import AppStoreVersionExperimentTreatmentCreateRequest
from openapi_client.models.app_store_version_experiment_treatment_response import AppStoreVersionExperimentTreatmentResponse
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
    api_instance = openapi_client.AppStoreVersionExperimentTreatmentsApi(api_client)
    app_store_version_experiment_treatment_create_request = openapi_client.AppStoreVersionExperimentTreatmentCreateRequest() # AppStoreVersionExperimentTreatmentCreateRequest | AppStoreVersionExperimentTreatment representation

    try:
        api_response = api_instance.app_store_version_experiment_treatments_create_instance(app_store_version_experiment_treatment_create_request)
        print("The response of AppStoreVersionExperimentTreatmentsApi->app_store_version_experiment_treatments_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionExperimentTreatmentsApi->app_store_version_experiment_treatments_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **app_store_version_experiment_treatment_create_request** | [**AppStoreVersionExperimentTreatmentCreateRequest**](AppStoreVersionExperimentTreatmentCreateRequest.md)| AppStoreVersionExperimentTreatment representation | 

### Return type

[**AppStoreVersionExperimentTreatmentResponse**](AppStoreVersionExperimentTreatmentResponse.md)

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
**201** | Single AppStoreVersionExperimentTreatment |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_store_version_experiment_treatments_delete_instance**
> app_store_version_experiment_treatments_delete_instance(id)

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
    api_instance = openapi_client.AppStoreVersionExperimentTreatmentsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.app_store_version_experiment_treatments_delete_instance(id)
    except Exception as e:
        print("Exception when calling AppStoreVersionExperimentTreatmentsApi->app_store_version_experiment_treatments_delete_instance: %s\n" % e)
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

# **app_store_version_experiment_treatments_get_instance**
> AppStoreVersionExperimentTreatmentResponse app_store_version_experiment_treatments_get_instance(id, fields_app_store_version_experiment_treatments=fields_app_store_version_experiment_treatments, fields_app_store_version_experiment_treatment_localizations=fields_app_store_version_experiment_treatment_localizations, include=include, limit_app_store_version_experiment_treatment_localizations=limit_app_store_version_experiment_treatment_localizations)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_experiment_treatment_response import AppStoreVersionExperimentTreatmentResponse
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
    api_instance = openapi_client.AppStoreVersionExperimentTreatmentsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_store_version_experiment_treatments = ['fields_app_store_version_experiment_treatments_example'] # List[str] | the fields to include for returned resources of type appStoreVersionExperimentTreatments (optional)
    fields_app_store_version_experiment_treatment_localizations = ['fields_app_store_version_experiment_treatment_localizations_example'] # List[str] | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_store_version_experiment_treatment_localizations = 56 # int | maximum number of related appStoreVersionExperimentTreatmentLocalizations returned (when they are included) (optional)

    try:
        api_response = api_instance.app_store_version_experiment_treatments_get_instance(id, fields_app_store_version_experiment_treatments=fields_app_store_version_experiment_treatments, fields_app_store_version_experiment_treatment_localizations=fields_app_store_version_experiment_treatment_localizations, include=include, limit_app_store_version_experiment_treatment_localizations=limit_app_store_version_experiment_treatment_localizations)
        print("The response of AppStoreVersionExperimentTreatmentsApi->app_store_version_experiment_treatments_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionExperimentTreatmentsApi->app_store_version_experiment_treatments_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_store_version_experiment_treatments** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionExperimentTreatments | [optional] 
 **fields_app_store_version_experiment_treatment_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_store_version_experiment_treatment_localizations** | **int**| maximum number of related appStoreVersionExperimentTreatmentLocalizations returned (when they are included) | [optional] 

### Return type

[**AppStoreVersionExperimentTreatmentResponse**](AppStoreVersionExperimentTreatmentResponse.md)

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
**200** | Single AppStoreVersionExperimentTreatment |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_store_version_experiment_treatments_update_instance**
> AppStoreVersionExperimentTreatmentResponse app_store_version_experiment_treatments_update_instance(id, app_store_version_experiment_treatment_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_experiment_treatment_response import AppStoreVersionExperimentTreatmentResponse
from openapi_client.models.app_store_version_experiment_treatment_update_request import AppStoreVersionExperimentTreatmentUpdateRequest
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
    api_instance = openapi_client.AppStoreVersionExperimentTreatmentsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    app_store_version_experiment_treatment_update_request = openapi_client.AppStoreVersionExperimentTreatmentUpdateRequest() # AppStoreVersionExperimentTreatmentUpdateRequest | AppStoreVersionExperimentTreatment representation

    try:
        api_response = api_instance.app_store_version_experiment_treatments_update_instance(id, app_store_version_experiment_treatment_update_request)
        print("The response of AppStoreVersionExperimentTreatmentsApi->app_store_version_experiment_treatments_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionExperimentTreatmentsApi->app_store_version_experiment_treatments_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **app_store_version_experiment_treatment_update_request** | [**AppStoreVersionExperimentTreatmentUpdateRequest**](AppStoreVersionExperimentTreatmentUpdateRequest.md)| AppStoreVersionExperimentTreatment representation | 

### Return type

[**AppStoreVersionExperimentTreatmentResponse**](AppStoreVersionExperimentTreatmentResponse.md)

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
**200** | Single AppStoreVersionExperimentTreatment |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

