# openapi_client.AppCustomProductPagesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**app_custom_product_pages_app_custom_product_page_versions_get_to_many_related**](AppCustomProductPagesApi.md#app_custom_product_pages_app_custom_product_page_versions_get_to_many_related) | **GET** /v1/appCustomProductPages/{id}/appCustomProductPageVersions | 
[**app_custom_product_pages_app_custom_product_page_versions_get_to_many_relationship**](AppCustomProductPagesApi.md#app_custom_product_pages_app_custom_product_page_versions_get_to_many_relationship) | **GET** /v1/appCustomProductPages/{id}/relationships/appCustomProductPageVersions | 
[**app_custom_product_pages_create_instance**](AppCustomProductPagesApi.md#app_custom_product_pages_create_instance) | **POST** /v1/appCustomProductPages | 
[**app_custom_product_pages_delete_instance**](AppCustomProductPagesApi.md#app_custom_product_pages_delete_instance) | **DELETE** /v1/appCustomProductPages/{id} | 
[**app_custom_product_pages_get_instance**](AppCustomProductPagesApi.md#app_custom_product_pages_get_instance) | **GET** /v1/appCustomProductPages/{id} | 
[**app_custom_product_pages_update_instance**](AppCustomProductPagesApi.md#app_custom_product_pages_update_instance) | **PATCH** /v1/appCustomProductPages/{id} | 


# **app_custom_product_pages_app_custom_product_page_versions_get_to_many_related**
> AppCustomProductPageVersionsResponse app_custom_product_pages_app_custom_product_page_versions_get_to_many_related(id, filter_state=filter_state, fields_app_custom_product_page_versions=fields_app_custom_product_page_versions, fields_app_custom_product_pages=fields_app_custom_product_pages, fields_app_custom_product_page_localizations=fields_app_custom_product_page_localizations, limit=limit, include=include, limit_app_custom_product_page_localizations=limit_app_custom_product_page_localizations)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_custom_product_page_versions_response import AppCustomProductPageVersionsResponse
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
    api_instance = openapi_client.AppCustomProductPagesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_state = ['filter_state_example'] # List[str] | filter by attribute 'state' (optional)
    fields_app_custom_product_page_versions = ['fields_app_custom_product_page_versions_example'] # List[str] | the fields to include for returned resources of type appCustomProductPageVersions (optional)
    fields_app_custom_product_pages = ['fields_app_custom_product_pages_example'] # List[str] | the fields to include for returned resources of type appCustomProductPages (optional)
    fields_app_custom_product_page_localizations = ['fields_app_custom_product_page_localizations_example'] # List[str] | the fields to include for returned resources of type appCustomProductPageLocalizations (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_custom_product_page_localizations = 56 # int | maximum number of related appCustomProductPageLocalizations returned (when they are included) (optional)

    try:
        api_response = api_instance.app_custom_product_pages_app_custom_product_page_versions_get_to_many_related(id, filter_state=filter_state, fields_app_custom_product_page_versions=fields_app_custom_product_page_versions, fields_app_custom_product_pages=fields_app_custom_product_pages, fields_app_custom_product_page_localizations=fields_app_custom_product_page_localizations, limit=limit, include=include, limit_app_custom_product_page_localizations=limit_app_custom_product_page_localizations)
        print("The response of AppCustomProductPagesApi->app_custom_product_pages_app_custom_product_page_versions_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppCustomProductPagesApi->app_custom_product_pages_app_custom_product_page_versions_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_state** | [**List[str]**](str.md)| filter by attribute &#39;state&#39; | [optional] 
 **fields_app_custom_product_page_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type appCustomProductPageVersions | [optional] 
 **fields_app_custom_product_pages** | [**List[str]**](str.md)| the fields to include for returned resources of type appCustomProductPages | [optional] 
 **fields_app_custom_product_page_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appCustomProductPageLocalizations | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_custom_product_page_localizations** | **int**| maximum number of related appCustomProductPageLocalizations returned (when they are included) | [optional] 

### Return type

[**AppCustomProductPageVersionsResponse**](AppCustomProductPageVersionsResponse.md)

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
**200** | List of AppCustomProductPageVersions |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_custom_product_pages_app_custom_product_page_versions_get_to_many_relationship**
> AppCustomProductPageAppCustomProductPageVersionsLinkagesResponse app_custom_product_pages_app_custom_product_page_versions_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_custom_product_page_app_custom_product_page_versions_linkages_response import AppCustomProductPageAppCustomProductPageVersionsLinkagesResponse
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
    api_instance = openapi_client.AppCustomProductPagesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.app_custom_product_pages_app_custom_product_page_versions_get_to_many_relationship(id, limit=limit)
        print("The response of AppCustomProductPagesApi->app_custom_product_pages_app_custom_product_page_versions_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppCustomProductPagesApi->app_custom_product_pages_app_custom_product_page_versions_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AppCustomProductPageAppCustomProductPageVersionsLinkagesResponse**](AppCustomProductPageAppCustomProductPageVersionsLinkagesResponse.md)

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

# **app_custom_product_pages_create_instance**
> AppCustomProductPageResponse app_custom_product_pages_create_instance(app_custom_product_page_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_custom_product_page_create_request import AppCustomProductPageCreateRequest
from openapi_client.models.app_custom_product_page_response import AppCustomProductPageResponse
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
    api_instance = openapi_client.AppCustomProductPagesApi(api_client)
    app_custom_product_page_create_request = openapi_client.AppCustomProductPageCreateRequest() # AppCustomProductPageCreateRequest | AppCustomProductPage representation

    try:
        api_response = api_instance.app_custom_product_pages_create_instance(app_custom_product_page_create_request)
        print("The response of AppCustomProductPagesApi->app_custom_product_pages_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppCustomProductPagesApi->app_custom_product_pages_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **app_custom_product_page_create_request** | [**AppCustomProductPageCreateRequest**](AppCustomProductPageCreateRequest.md)| AppCustomProductPage representation | 

### Return type

[**AppCustomProductPageResponse**](AppCustomProductPageResponse.md)

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
**201** | Single AppCustomProductPage |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_custom_product_pages_delete_instance**
> app_custom_product_pages_delete_instance(id)

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
    api_instance = openapi_client.AppCustomProductPagesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.app_custom_product_pages_delete_instance(id)
    except Exception as e:
        print("Exception when calling AppCustomProductPagesApi->app_custom_product_pages_delete_instance: %s\n" % e)
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

# **app_custom_product_pages_get_instance**
> AppCustomProductPageResponse app_custom_product_pages_get_instance(id, fields_app_custom_product_pages=fields_app_custom_product_pages, fields_app_custom_product_page_versions=fields_app_custom_product_page_versions, include=include, limit_app_custom_product_page_versions=limit_app_custom_product_page_versions)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_custom_product_page_response import AppCustomProductPageResponse
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
    api_instance = openapi_client.AppCustomProductPagesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_custom_product_pages = ['fields_app_custom_product_pages_example'] # List[str] | the fields to include for returned resources of type appCustomProductPages (optional)
    fields_app_custom_product_page_versions = ['fields_app_custom_product_page_versions_example'] # List[str] | the fields to include for returned resources of type appCustomProductPageVersions (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_custom_product_page_versions = 56 # int | maximum number of related appCustomProductPageVersions returned (when they are included) (optional)

    try:
        api_response = api_instance.app_custom_product_pages_get_instance(id, fields_app_custom_product_pages=fields_app_custom_product_pages, fields_app_custom_product_page_versions=fields_app_custom_product_page_versions, include=include, limit_app_custom_product_page_versions=limit_app_custom_product_page_versions)
        print("The response of AppCustomProductPagesApi->app_custom_product_pages_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppCustomProductPagesApi->app_custom_product_pages_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_custom_product_pages** | [**List[str]**](str.md)| the fields to include for returned resources of type appCustomProductPages | [optional] 
 **fields_app_custom_product_page_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type appCustomProductPageVersions | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_custom_product_page_versions** | **int**| maximum number of related appCustomProductPageVersions returned (when they are included) | [optional] 

### Return type

[**AppCustomProductPageResponse**](AppCustomProductPageResponse.md)

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
**200** | Single AppCustomProductPage |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_custom_product_pages_update_instance**
> AppCustomProductPageResponse app_custom_product_pages_update_instance(id, app_custom_product_page_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_custom_product_page_response import AppCustomProductPageResponse
from openapi_client.models.app_custom_product_page_update_request import AppCustomProductPageUpdateRequest
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
    api_instance = openapi_client.AppCustomProductPagesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    app_custom_product_page_update_request = openapi_client.AppCustomProductPageUpdateRequest() # AppCustomProductPageUpdateRequest | AppCustomProductPage representation

    try:
        api_response = api_instance.app_custom_product_pages_update_instance(id, app_custom_product_page_update_request)
        print("The response of AppCustomProductPagesApi->app_custom_product_pages_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppCustomProductPagesApi->app_custom_product_pages_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **app_custom_product_page_update_request** | [**AppCustomProductPageUpdateRequest**](AppCustomProductPageUpdateRequest.md)| AppCustomProductPage representation | 

### Return type

[**AppCustomProductPageResponse**](AppCustomProductPageResponse.md)

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
**200** | Single AppCustomProductPage |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

