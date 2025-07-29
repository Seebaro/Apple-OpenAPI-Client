# openapi_client.AppCategoriesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**app_categories_get_collection**](AppCategoriesApi.md#app_categories_get_collection) | **GET** /v1/appCategories | 
[**app_categories_get_instance**](AppCategoriesApi.md#app_categories_get_instance) | **GET** /v1/appCategories/{id} | 
[**app_categories_parent_get_to_one_related**](AppCategoriesApi.md#app_categories_parent_get_to_one_related) | **GET** /v1/appCategories/{id}/parent | 
[**app_categories_parent_get_to_one_relationship**](AppCategoriesApi.md#app_categories_parent_get_to_one_relationship) | **GET** /v1/appCategories/{id}/relationships/parent | 
[**app_categories_subcategories_get_to_many_related**](AppCategoriesApi.md#app_categories_subcategories_get_to_many_related) | **GET** /v1/appCategories/{id}/subcategories | 
[**app_categories_subcategories_get_to_many_relationship**](AppCategoriesApi.md#app_categories_subcategories_get_to_many_relationship) | **GET** /v1/appCategories/{id}/relationships/subcategories | 


# **app_categories_get_collection**
> AppCategoriesResponse app_categories_get_collection(filter_platforms=filter_platforms, exists_parent=exists_parent, fields_app_categories=fields_app_categories, limit=limit, include=include, limit_subcategories=limit_subcategories)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_categories_response import AppCategoriesResponse
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
    api_instance = openapi_client.AppCategoriesApi(api_client)
    filter_platforms = ['filter_platforms_example'] # List[str] | filter by attribute 'platforms' (optional)
    exists_parent = True # bool | filter by existence or non-existence of related 'parent' (optional)
    fields_app_categories = ['fields_app_categories_example'] # List[str] | the fields to include for returned resources of type appCategories (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_subcategories = 56 # int | maximum number of related subcategories returned (when they are included) (optional)

    try:
        api_response = api_instance.app_categories_get_collection(filter_platforms=filter_platforms, exists_parent=exists_parent, fields_app_categories=fields_app_categories, limit=limit, include=include, limit_subcategories=limit_subcategories)
        print("The response of AppCategoriesApi->app_categories_get_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppCategoriesApi->app_categories_get_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter_platforms** | [**List[str]**](str.md)| filter by attribute &#39;platforms&#39; | [optional] 
 **exists_parent** | **bool**| filter by existence or non-existence of related &#39;parent&#39; | [optional] 
 **fields_app_categories** | [**List[str]**](str.md)| the fields to include for returned resources of type appCategories | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_subcategories** | **int**| maximum number of related subcategories returned (when they are included) | [optional] 

### Return type

[**AppCategoriesResponse**](AppCategoriesResponse.md)

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
**200** | List of AppCategories |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_categories_get_instance**
> AppCategoryResponse app_categories_get_instance(id, fields_app_categories=fields_app_categories, include=include, limit_subcategories=limit_subcategories)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_category_response import AppCategoryResponse
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
    api_instance = openapi_client.AppCategoriesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_categories = ['fields_app_categories_example'] # List[str] | the fields to include for returned resources of type appCategories (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_subcategories = 56 # int | maximum number of related subcategories returned (when they are included) (optional)

    try:
        api_response = api_instance.app_categories_get_instance(id, fields_app_categories=fields_app_categories, include=include, limit_subcategories=limit_subcategories)
        print("The response of AppCategoriesApi->app_categories_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppCategoriesApi->app_categories_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_categories** | [**List[str]**](str.md)| the fields to include for returned resources of type appCategories | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_subcategories** | **int**| maximum number of related subcategories returned (when they are included) | [optional] 

### Return type

[**AppCategoryResponse**](AppCategoryResponse.md)

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
**200** | Single AppCategory |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_categories_parent_get_to_one_related**
> AppCategoryWithoutIncludesResponse app_categories_parent_get_to_one_related(id, fields_app_categories=fields_app_categories)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_category_without_includes_response import AppCategoryWithoutIncludesResponse
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
    api_instance = openapi_client.AppCategoriesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_categories = ['fields_app_categories_example'] # List[str] | the fields to include for returned resources of type appCategories (optional)

    try:
        api_response = api_instance.app_categories_parent_get_to_one_related(id, fields_app_categories=fields_app_categories)
        print("The response of AppCategoriesApi->app_categories_parent_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppCategoriesApi->app_categories_parent_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_categories** | [**List[str]**](str.md)| the fields to include for returned resources of type appCategories | [optional] 

### Return type

[**AppCategoryWithoutIncludesResponse**](AppCategoryWithoutIncludesResponse.md)

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
**200** | Single AppCategory with get |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_categories_parent_get_to_one_relationship**
> AppCategoryParentLinkageResponse app_categories_parent_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_category_parent_linkage_response import AppCategoryParentLinkageResponse
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
    api_instance = openapi_client.AppCategoriesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.app_categories_parent_get_to_one_relationship(id)
        print("The response of AppCategoriesApi->app_categories_parent_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppCategoriesApi->app_categories_parent_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**AppCategoryParentLinkageResponse**](AppCategoryParentLinkageResponse.md)

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

# **app_categories_subcategories_get_to_many_related**
> AppCategoriesWithoutIncludesResponse app_categories_subcategories_get_to_many_related(id, fields_app_categories=fields_app_categories, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_categories_without_includes_response import AppCategoriesWithoutIncludesResponse
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
    api_instance = openapi_client.AppCategoriesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_categories = ['fields_app_categories_example'] # List[str] | the fields to include for returned resources of type appCategories (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.app_categories_subcategories_get_to_many_related(id, fields_app_categories=fields_app_categories, limit=limit)
        print("The response of AppCategoriesApi->app_categories_subcategories_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppCategoriesApi->app_categories_subcategories_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_categories** | [**List[str]**](str.md)| the fields to include for returned resources of type appCategories | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AppCategoriesWithoutIncludesResponse**](AppCategoriesWithoutIncludesResponse.md)

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
**200** | List of AppCategories with get |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_categories_subcategories_get_to_many_relationship**
> AppCategorySubcategoriesLinkagesResponse app_categories_subcategories_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_category_subcategories_linkages_response import AppCategorySubcategoriesLinkagesResponse
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
    api_instance = openapi_client.AppCategoriesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.app_categories_subcategories_get_to_many_relationship(id, limit=limit)
        print("The response of AppCategoriesApi->app_categories_subcategories_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppCategoriesApi->app_categories_subcategories_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AppCategorySubcategoriesLinkagesResponse**](AppCategorySubcategoriesLinkagesResponse.md)

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

