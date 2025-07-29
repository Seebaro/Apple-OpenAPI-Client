# openapi_client.AppStoreVersionExperimentsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**app_store_version_experiments_app_store_version_experiment_treatments_get_to_many_related**](AppStoreVersionExperimentsApi.md#app_store_version_experiments_app_store_version_experiment_treatments_get_to_many_related) | **GET** /v1/appStoreVersionExperiments/{id}/appStoreVersionExperimentTreatments | 
[**app_store_version_experiments_app_store_version_experiment_treatments_get_to_many_relationship**](AppStoreVersionExperimentsApi.md#app_store_version_experiments_app_store_version_experiment_treatments_get_to_many_relationship) | **GET** /v1/appStoreVersionExperiments/{id}/relationships/appStoreVersionExperimentTreatments | 
[**app_store_version_experiments_create_instance**](AppStoreVersionExperimentsApi.md#app_store_version_experiments_create_instance) | **POST** /v1/appStoreVersionExperiments | 
[**app_store_version_experiments_delete_instance**](AppStoreVersionExperimentsApi.md#app_store_version_experiments_delete_instance) | **DELETE** /v1/appStoreVersionExperiments/{id} | 
[**app_store_version_experiments_get_instance**](AppStoreVersionExperimentsApi.md#app_store_version_experiments_get_instance) | **GET** /v1/appStoreVersionExperiments/{id} | 
[**app_store_version_experiments_update_instance**](AppStoreVersionExperimentsApi.md#app_store_version_experiments_update_instance) | **PATCH** /v1/appStoreVersionExperiments/{id} | 
[**app_store_version_experiments_v2_app_store_version_experiment_treatments_get_to_many_related**](AppStoreVersionExperimentsApi.md#app_store_version_experiments_v2_app_store_version_experiment_treatments_get_to_many_related) | **GET** /v2/appStoreVersionExperiments/{id}/appStoreVersionExperimentTreatments | 
[**app_store_version_experiments_v2_app_store_version_experiment_treatments_get_to_many_relationship**](AppStoreVersionExperimentsApi.md#app_store_version_experiments_v2_app_store_version_experiment_treatments_get_to_many_relationship) | **GET** /v2/appStoreVersionExperiments/{id}/relationships/appStoreVersionExperimentTreatments | 
[**app_store_version_experiments_v2_create_instance**](AppStoreVersionExperimentsApi.md#app_store_version_experiments_v2_create_instance) | **POST** /v2/appStoreVersionExperiments | 
[**app_store_version_experiments_v2_delete_instance**](AppStoreVersionExperimentsApi.md#app_store_version_experiments_v2_delete_instance) | **DELETE** /v2/appStoreVersionExperiments/{id} | 
[**app_store_version_experiments_v2_get_instance**](AppStoreVersionExperimentsApi.md#app_store_version_experiments_v2_get_instance) | **GET** /v2/appStoreVersionExperiments/{id} | 
[**app_store_version_experiments_v2_update_instance**](AppStoreVersionExperimentsApi.md#app_store_version_experiments_v2_update_instance) | **PATCH** /v2/appStoreVersionExperiments/{id} | 


# **app_store_version_experiments_app_store_version_experiment_treatments_get_to_many_related**
> AppStoreVersionExperimentTreatmentsResponse app_store_version_experiments_app_store_version_experiment_treatments_get_to_many_related(id, fields_app_store_version_experiment_treatments=fields_app_store_version_experiment_treatments, fields_app_store_version_experiments=fields_app_store_version_experiments, fields_app_store_version_experiment_treatment_localizations=fields_app_store_version_experiment_treatment_localizations, limit=limit, include=include, limit_app_store_version_experiment_treatment_localizations=limit_app_store_version_experiment_treatment_localizations)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_experiment_treatments_response import AppStoreVersionExperimentTreatmentsResponse
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
    api_instance = openapi_client.AppStoreVersionExperimentsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_store_version_experiment_treatments = ['fields_app_store_version_experiment_treatments_example'] # List[str] | the fields to include for returned resources of type appStoreVersionExperimentTreatments (optional)
    fields_app_store_version_experiments = ['fields_app_store_version_experiments_example'] # List[str] | the fields to include for returned resources of type appStoreVersionExperiments (optional)
    fields_app_store_version_experiment_treatment_localizations = ['fields_app_store_version_experiment_treatment_localizations_example'] # List[str] | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_store_version_experiment_treatment_localizations = 56 # int | maximum number of related appStoreVersionExperimentTreatmentLocalizations returned (when they are included) (optional)

    try:
        api_response = api_instance.app_store_version_experiments_app_store_version_experiment_treatments_get_to_many_related(id, fields_app_store_version_experiment_treatments=fields_app_store_version_experiment_treatments, fields_app_store_version_experiments=fields_app_store_version_experiments, fields_app_store_version_experiment_treatment_localizations=fields_app_store_version_experiment_treatment_localizations, limit=limit, include=include, limit_app_store_version_experiment_treatment_localizations=limit_app_store_version_experiment_treatment_localizations)
        print("The response of AppStoreVersionExperimentsApi->app_store_version_experiments_app_store_version_experiment_treatments_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionExperimentsApi->app_store_version_experiments_app_store_version_experiment_treatments_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_store_version_experiment_treatments** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionExperimentTreatments | [optional] 
 **fields_app_store_version_experiments** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionExperiments | [optional] 
 **fields_app_store_version_experiment_treatment_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_store_version_experiment_treatment_localizations** | **int**| maximum number of related appStoreVersionExperimentTreatmentLocalizations returned (when they are included) | [optional] 

### Return type

[**AppStoreVersionExperimentTreatmentsResponse**](AppStoreVersionExperimentTreatmentsResponse.md)

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
**200** | List of AppStoreVersionExperimentTreatments |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_store_version_experiments_app_store_version_experiment_treatments_get_to_many_relationship**
> AppStoreVersionExperimentAppStoreVersionExperimentTreatmentsLinkagesResponse app_store_version_experiments_app_store_version_experiment_treatments_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_experiment_app_store_version_experiment_treatments_linkages_response import AppStoreVersionExperimentAppStoreVersionExperimentTreatmentsLinkagesResponse
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
    api_instance = openapi_client.AppStoreVersionExperimentsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.app_store_version_experiments_app_store_version_experiment_treatments_get_to_many_relationship(id, limit=limit)
        print("The response of AppStoreVersionExperimentsApi->app_store_version_experiments_app_store_version_experiment_treatments_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionExperimentsApi->app_store_version_experiments_app_store_version_experiment_treatments_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AppStoreVersionExperimentAppStoreVersionExperimentTreatmentsLinkagesResponse**](AppStoreVersionExperimentAppStoreVersionExperimentTreatmentsLinkagesResponse.md)

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

# **app_store_version_experiments_create_instance**
> AppStoreVersionExperimentResponse app_store_version_experiments_create_instance(app_store_version_experiment_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_experiment_create_request import AppStoreVersionExperimentCreateRequest
from openapi_client.models.app_store_version_experiment_response import AppStoreVersionExperimentResponse
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
    api_instance = openapi_client.AppStoreVersionExperimentsApi(api_client)
    app_store_version_experiment_create_request = openapi_client.AppStoreVersionExperimentCreateRequest() # AppStoreVersionExperimentCreateRequest | AppStoreVersionExperiment representation

    try:
        api_response = api_instance.app_store_version_experiments_create_instance(app_store_version_experiment_create_request)
        print("The response of AppStoreVersionExperimentsApi->app_store_version_experiments_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionExperimentsApi->app_store_version_experiments_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **app_store_version_experiment_create_request** | [**AppStoreVersionExperimentCreateRequest**](AppStoreVersionExperimentCreateRequest.md)| AppStoreVersionExperiment representation | 

### Return type

[**AppStoreVersionExperimentResponse**](AppStoreVersionExperimentResponse.md)

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
**201** | Single AppStoreVersionExperiment |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_store_version_experiments_delete_instance**
> app_store_version_experiments_delete_instance(id)

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
    api_instance = openapi_client.AppStoreVersionExperimentsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.app_store_version_experiments_delete_instance(id)
    except Exception as e:
        print("Exception when calling AppStoreVersionExperimentsApi->app_store_version_experiments_delete_instance: %s\n" % e)
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

# **app_store_version_experiments_get_instance**
> AppStoreVersionExperimentResponse app_store_version_experiments_get_instance(id, fields_app_store_version_experiments=fields_app_store_version_experiments, fields_app_store_version_experiment_treatments=fields_app_store_version_experiment_treatments, include=include, limit_app_store_version_experiment_treatments=limit_app_store_version_experiment_treatments)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_experiment_response import AppStoreVersionExperimentResponse
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
    api_instance = openapi_client.AppStoreVersionExperimentsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_store_version_experiments = ['fields_app_store_version_experiments_example'] # List[str] | the fields to include for returned resources of type appStoreVersionExperiments (optional)
    fields_app_store_version_experiment_treatments = ['fields_app_store_version_experiment_treatments_example'] # List[str] | the fields to include for returned resources of type appStoreVersionExperimentTreatments (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_store_version_experiment_treatments = 56 # int | maximum number of related appStoreVersionExperimentTreatments returned (when they are included) (optional)

    try:
        api_response = api_instance.app_store_version_experiments_get_instance(id, fields_app_store_version_experiments=fields_app_store_version_experiments, fields_app_store_version_experiment_treatments=fields_app_store_version_experiment_treatments, include=include, limit_app_store_version_experiment_treatments=limit_app_store_version_experiment_treatments)
        print("The response of AppStoreVersionExperimentsApi->app_store_version_experiments_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionExperimentsApi->app_store_version_experiments_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_store_version_experiments** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionExperiments | [optional] 
 **fields_app_store_version_experiment_treatments** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionExperimentTreatments | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_store_version_experiment_treatments** | **int**| maximum number of related appStoreVersionExperimentTreatments returned (when they are included) | [optional] 

### Return type

[**AppStoreVersionExperimentResponse**](AppStoreVersionExperimentResponse.md)

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
**200** | Single AppStoreVersionExperiment |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_store_version_experiments_update_instance**
> AppStoreVersionExperimentResponse app_store_version_experiments_update_instance(id, app_store_version_experiment_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_experiment_response import AppStoreVersionExperimentResponse
from openapi_client.models.app_store_version_experiment_update_request import AppStoreVersionExperimentUpdateRequest
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
    api_instance = openapi_client.AppStoreVersionExperimentsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    app_store_version_experiment_update_request = openapi_client.AppStoreVersionExperimentUpdateRequest() # AppStoreVersionExperimentUpdateRequest | AppStoreVersionExperiment representation

    try:
        api_response = api_instance.app_store_version_experiments_update_instance(id, app_store_version_experiment_update_request)
        print("The response of AppStoreVersionExperimentsApi->app_store_version_experiments_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionExperimentsApi->app_store_version_experiments_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **app_store_version_experiment_update_request** | [**AppStoreVersionExperimentUpdateRequest**](AppStoreVersionExperimentUpdateRequest.md)| AppStoreVersionExperiment representation | 

### Return type

[**AppStoreVersionExperimentResponse**](AppStoreVersionExperimentResponse.md)

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
**200** | Single AppStoreVersionExperiment |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_store_version_experiments_v2_app_store_version_experiment_treatments_get_to_many_related**
> AppStoreVersionExperimentTreatmentsResponse app_store_version_experiments_v2_app_store_version_experiment_treatments_get_to_many_related(id, fields_app_store_version_experiment_treatments=fields_app_store_version_experiment_treatments, fields_app_store_version_experiments=fields_app_store_version_experiments, fields_app_store_version_experiment_treatment_localizations=fields_app_store_version_experiment_treatment_localizations, limit=limit, include=include, limit_app_store_version_experiment_treatment_localizations=limit_app_store_version_experiment_treatment_localizations)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_experiment_treatments_response import AppStoreVersionExperimentTreatmentsResponse
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
    api_instance = openapi_client.AppStoreVersionExperimentsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_store_version_experiment_treatments = ['fields_app_store_version_experiment_treatments_example'] # List[str] | the fields to include for returned resources of type appStoreVersionExperimentTreatments (optional)
    fields_app_store_version_experiments = ['fields_app_store_version_experiments_example'] # List[str] | the fields to include for returned resources of type appStoreVersionExperiments (optional)
    fields_app_store_version_experiment_treatment_localizations = ['fields_app_store_version_experiment_treatment_localizations_example'] # List[str] | the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_store_version_experiment_treatment_localizations = 56 # int | maximum number of related appStoreVersionExperimentTreatmentLocalizations returned (when they are included) (optional)

    try:
        api_response = api_instance.app_store_version_experiments_v2_app_store_version_experiment_treatments_get_to_many_related(id, fields_app_store_version_experiment_treatments=fields_app_store_version_experiment_treatments, fields_app_store_version_experiments=fields_app_store_version_experiments, fields_app_store_version_experiment_treatment_localizations=fields_app_store_version_experiment_treatment_localizations, limit=limit, include=include, limit_app_store_version_experiment_treatment_localizations=limit_app_store_version_experiment_treatment_localizations)
        print("The response of AppStoreVersionExperimentsApi->app_store_version_experiments_v2_app_store_version_experiment_treatments_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionExperimentsApi->app_store_version_experiments_v2_app_store_version_experiment_treatments_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_store_version_experiment_treatments** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionExperimentTreatments | [optional] 
 **fields_app_store_version_experiments** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionExperiments | [optional] 
 **fields_app_store_version_experiment_treatment_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionExperimentTreatmentLocalizations | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_store_version_experiment_treatment_localizations** | **int**| maximum number of related appStoreVersionExperimentTreatmentLocalizations returned (when they are included) | [optional] 

### Return type

[**AppStoreVersionExperimentTreatmentsResponse**](AppStoreVersionExperimentTreatmentsResponse.md)

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
**200** | List of AppStoreVersionExperimentTreatments |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_store_version_experiments_v2_app_store_version_experiment_treatments_get_to_many_relationship**
> AppStoreVersionExperimentV2AppStoreVersionExperimentTreatmentsLinkagesResponse app_store_version_experiments_v2_app_store_version_experiment_treatments_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_experiment_v2_app_store_version_experiment_treatments_linkages_response import AppStoreVersionExperimentV2AppStoreVersionExperimentTreatmentsLinkagesResponse
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
    api_instance = openapi_client.AppStoreVersionExperimentsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.app_store_version_experiments_v2_app_store_version_experiment_treatments_get_to_many_relationship(id, limit=limit)
        print("The response of AppStoreVersionExperimentsApi->app_store_version_experiments_v2_app_store_version_experiment_treatments_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionExperimentsApi->app_store_version_experiments_v2_app_store_version_experiment_treatments_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AppStoreVersionExperimentV2AppStoreVersionExperimentTreatmentsLinkagesResponse**](AppStoreVersionExperimentV2AppStoreVersionExperimentTreatmentsLinkagesResponse.md)

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

# **app_store_version_experiments_v2_create_instance**
> AppStoreVersionExperimentV2Response app_store_version_experiments_v2_create_instance(app_store_version_experiment_v2_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_experiment_v2_create_request import AppStoreVersionExperimentV2CreateRequest
from openapi_client.models.app_store_version_experiment_v2_response import AppStoreVersionExperimentV2Response
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
    api_instance = openapi_client.AppStoreVersionExperimentsApi(api_client)
    app_store_version_experiment_v2_create_request = openapi_client.AppStoreVersionExperimentV2CreateRequest() # AppStoreVersionExperimentV2CreateRequest | AppStoreVersionExperiment representation

    try:
        api_response = api_instance.app_store_version_experiments_v2_create_instance(app_store_version_experiment_v2_create_request)
        print("The response of AppStoreVersionExperimentsApi->app_store_version_experiments_v2_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionExperimentsApi->app_store_version_experiments_v2_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **app_store_version_experiment_v2_create_request** | [**AppStoreVersionExperimentV2CreateRequest**](AppStoreVersionExperimentV2CreateRequest.md)| AppStoreVersionExperiment representation | 

### Return type

[**AppStoreVersionExperimentV2Response**](AppStoreVersionExperimentV2Response.md)

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
**201** | Single AppStoreVersionExperiment |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_store_version_experiments_v2_delete_instance**
> app_store_version_experiments_v2_delete_instance(id)

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
    api_instance = openapi_client.AppStoreVersionExperimentsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.app_store_version_experiments_v2_delete_instance(id)
    except Exception as e:
        print("Exception when calling AppStoreVersionExperimentsApi->app_store_version_experiments_v2_delete_instance: %s\n" % e)
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

# **app_store_version_experiments_v2_get_instance**
> AppStoreVersionExperimentV2Response app_store_version_experiments_v2_get_instance(id, fields_app_store_version_experiments=fields_app_store_version_experiments, fields_app_store_version_experiment_treatments=fields_app_store_version_experiment_treatments, include=include, limit_app_store_version_experiment_treatments=limit_app_store_version_experiment_treatments, limit_control_versions=limit_control_versions)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_experiment_v2_response import AppStoreVersionExperimentV2Response
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
    api_instance = openapi_client.AppStoreVersionExperimentsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_store_version_experiments = ['fields_app_store_version_experiments_example'] # List[str] | the fields to include for returned resources of type appStoreVersionExperiments (optional)
    fields_app_store_version_experiment_treatments = ['fields_app_store_version_experiment_treatments_example'] # List[str] | the fields to include for returned resources of type appStoreVersionExperimentTreatments (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_store_version_experiment_treatments = 56 # int | maximum number of related appStoreVersionExperimentTreatments returned (when they are included) (optional)
    limit_control_versions = 56 # int | maximum number of related controlVersions returned (when they are included) (optional)

    try:
        api_response = api_instance.app_store_version_experiments_v2_get_instance(id, fields_app_store_version_experiments=fields_app_store_version_experiments, fields_app_store_version_experiment_treatments=fields_app_store_version_experiment_treatments, include=include, limit_app_store_version_experiment_treatments=limit_app_store_version_experiment_treatments, limit_control_versions=limit_control_versions)
        print("The response of AppStoreVersionExperimentsApi->app_store_version_experiments_v2_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionExperimentsApi->app_store_version_experiments_v2_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_store_version_experiments** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionExperiments | [optional] 
 **fields_app_store_version_experiment_treatments** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionExperimentTreatments | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_store_version_experiment_treatments** | **int**| maximum number of related appStoreVersionExperimentTreatments returned (when they are included) | [optional] 
 **limit_control_versions** | **int**| maximum number of related controlVersions returned (when they are included) | [optional] 

### Return type

[**AppStoreVersionExperimentV2Response**](AppStoreVersionExperimentV2Response.md)

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
**200** | Single AppStoreVersionExperiment |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_store_version_experiments_v2_update_instance**
> AppStoreVersionExperimentV2Response app_store_version_experiments_v2_update_instance(id, app_store_version_experiment_v2_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_experiment_v2_response import AppStoreVersionExperimentV2Response
from openapi_client.models.app_store_version_experiment_v2_update_request import AppStoreVersionExperimentV2UpdateRequest
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
    api_instance = openapi_client.AppStoreVersionExperimentsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    app_store_version_experiment_v2_update_request = openapi_client.AppStoreVersionExperimentV2UpdateRequest() # AppStoreVersionExperimentV2UpdateRequest | AppStoreVersionExperiment representation

    try:
        api_response = api_instance.app_store_version_experiments_v2_update_instance(id, app_store_version_experiment_v2_update_request)
        print("The response of AppStoreVersionExperimentsApi->app_store_version_experiments_v2_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppStoreVersionExperimentsApi->app_store_version_experiments_v2_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **app_store_version_experiment_v2_update_request** | [**AppStoreVersionExperimentV2UpdateRequest**](AppStoreVersionExperimentV2UpdateRequest.md)| AppStoreVersionExperiment representation | 

### Return type

[**AppStoreVersionExperimentV2Response**](AppStoreVersionExperimentV2Response.md)

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
**200** | Single AppStoreVersionExperiment |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

