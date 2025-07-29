# openapi_client.AppInfosApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**app_infos_age_rating_declaration_get_to_one_related**](AppInfosApi.md#app_infos_age_rating_declaration_get_to_one_related) | **GET** /v1/appInfos/{id}/ageRatingDeclaration | 
[**app_infos_age_rating_declaration_get_to_one_relationship**](AppInfosApi.md#app_infos_age_rating_declaration_get_to_one_relationship) | **GET** /v1/appInfos/{id}/relationships/ageRatingDeclaration | 
[**app_infos_app_info_localizations_get_to_many_related**](AppInfosApi.md#app_infos_app_info_localizations_get_to_many_related) | **GET** /v1/appInfos/{id}/appInfoLocalizations | 
[**app_infos_app_info_localizations_get_to_many_relationship**](AppInfosApi.md#app_infos_app_info_localizations_get_to_many_relationship) | **GET** /v1/appInfos/{id}/relationships/appInfoLocalizations | 
[**app_infos_get_instance**](AppInfosApi.md#app_infos_get_instance) | **GET** /v1/appInfos/{id} | 
[**app_infos_primary_category_get_to_one_related**](AppInfosApi.md#app_infos_primary_category_get_to_one_related) | **GET** /v1/appInfos/{id}/primaryCategory | 
[**app_infos_primary_category_get_to_one_relationship**](AppInfosApi.md#app_infos_primary_category_get_to_one_relationship) | **GET** /v1/appInfos/{id}/relationships/primaryCategory | 
[**app_infos_primary_subcategory_one_get_to_one_related**](AppInfosApi.md#app_infos_primary_subcategory_one_get_to_one_related) | **GET** /v1/appInfos/{id}/primarySubcategoryOne | 
[**app_infos_primary_subcategory_one_get_to_one_relationship**](AppInfosApi.md#app_infos_primary_subcategory_one_get_to_one_relationship) | **GET** /v1/appInfos/{id}/relationships/primarySubcategoryOne | 
[**app_infos_primary_subcategory_two_get_to_one_related**](AppInfosApi.md#app_infos_primary_subcategory_two_get_to_one_related) | **GET** /v1/appInfos/{id}/primarySubcategoryTwo | 
[**app_infos_primary_subcategory_two_get_to_one_relationship**](AppInfosApi.md#app_infos_primary_subcategory_two_get_to_one_relationship) | **GET** /v1/appInfos/{id}/relationships/primarySubcategoryTwo | 
[**app_infos_secondary_category_get_to_one_related**](AppInfosApi.md#app_infos_secondary_category_get_to_one_related) | **GET** /v1/appInfos/{id}/secondaryCategory | 
[**app_infos_secondary_category_get_to_one_relationship**](AppInfosApi.md#app_infos_secondary_category_get_to_one_relationship) | **GET** /v1/appInfos/{id}/relationships/secondaryCategory | 
[**app_infos_secondary_subcategory_one_get_to_one_related**](AppInfosApi.md#app_infos_secondary_subcategory_one_get_to_one_related) | **GET** /v1/appInfos/{id}/secondarySubcategoryOne | 
[**app_infos_secondary_subcategory_one_get_to_one_relationship**](AppInfosApi.md#app_infos_secondary_subcategory_one_get_to_one_relationship) | **GET** /v1/appInfos/{id}/relationships/secondarySubcategoryOne | 
[**app_infos_secondary_subcategory_two_get_to_one_related**](AppInfosApi.md#app_infos_secondary_subcategory_two_get_to_one_related) | **GET** /v1/appInfos/{id}/secondarySubcategoryTwo | 
[**app_infos_secondary_subcategory_two_get_to_one_relationship**](AppInfosApi.md#app_infos_secondary_subcategory_two_get_to_one_relationship) | **GET** /v1/appInfos/{id}/relationships/secondarySubcategoryTwo | 
[**app_infos_update_instance**](AppInfosApi.md#app_infos_update_instance) | **PATCH** /v1/appInfos/{id} | 


# **app_infos_age_rating_declaration_get_to_one_related**
> AgeRatingDeclarationResponse app_infos_age_rating_declaration_get_to_one_related(id, fields_age_rating_declarations=fields_age_rating_declarations)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.age_rating_declaration_response import AgeRatingDeclarationResponse
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
    api_instance = openapi_client.AppInfosApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_age_rating_declarations = ['fields_age_rating_declarations_example'] # List[str] | the fields to include for returned resources of type ageRatingDeclarations (optional)

    try:
        api_response = api_instance.app_infos_age_rating_declaration_get_to_one_related(id, fields_age_rating_declarations=fields_age_rating_declarations)
        print("The response of AppInfosApi->app_infos_age_rating_declaration_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppInfosApi->app_infos_age_rating_declaration_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_age_rating_declarations** | [**List[str]**](str.md)| the fields to include for returned resources of type ageRatingDeclarations | [optional] 

### Return type

[**AgeRatingDeclarationResponse**](AgeRatingDeclarationResponse.md)

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
**200** | Single AgeRatingDeclaration |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_infos_age_rating_declaration_get_to_one_relationship**
> AppInfoAgeRatingDeclarationLinkageResponse app_infos_age_rating_declaration_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_info_age_rating_declaration_linkage_response import AppInfoAgeRatingDeclarationLinkageResponse
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
    api_instance = openapi_client.AppInfosApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.app_infos_age_rating_declaration_get_to_one_relationship(id)
        print("The response of AppInfosApi->app_infos_age_rating_declaration_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppInfosApi->app_infos_age_rating_declaration_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**AppInfoAgeRatingDeclarationLinkageResponse**](AppInfoAgeRatingDeclarationLinkageResponse.md)

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

# **app_infos_app_info_localizations_get_to_many_related**
> AppInfoLocalizationsResponse app_infos_app_info_localizations_get_to_many_related(id, filter_locale=filter_locale, fields_app_info_localizations=fields_app_info_localizations, fields_app_infos=fields_app_infos, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_info_localizations_response import AppInfoLocalizationsResponse
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
    api_instance = openapi_client.AppInfosApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_locale = ['filter_locale_example'] # List[str] | filter by attribute 'locale' (optional)
    fields_app_info_localizations = ['fields_app_info_localizations_example'] # List[str] | the fields to include for returned resources of type appInfoLocalizations (optional)
    fields_app_infos = ['fields_app_infos_example'] # List[str] | the fields to include for returned resources of type appInfos (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.app_infos_app_info_localizations_get_to_many_related(id, filter_locale=filter_locale, fields_app_info_localizations=fields_app_info_localizations, fields_app_infos=fields_app_infos, limit=limit, include=include)
        print("The response of AppInfosApi->app_infos_app_info_localizations_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppInfosApi->app_infos_app_info_localizations_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_locale** | [**List[str]**](str.md)| filter by attribute &#39;locale&#39; | [optional] 
 **fields_app_info_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appInfoLocalizations | [optional] 
 **fields_app_infos** | [**List[str]**](str.md)| the fields to include for returned resources of type appInfos | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**AppInfoLocalizationsResponse**](AppInfoLocalizationsResponse.md)

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
**200** | List of AppInfoLocalizations |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_infos_app_info_localizations_get_to_many_relationship**
> AppInfoAppInfoLocalizationsLinkagesResponse app_infos_app_info_localizations_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_info_app_info_localizations_linkages_response import AppInfoAppInfoLocalizationsLinkagesResponse
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
    api_instance = openapi_client.AppInfosApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.app_infos_app_info_localizations_get_to_many_relationship(id, limit=limit)
        print("The response of AppInfosApi->app_infos_app_info_localizations_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppInfosApi->app_infos_app_info_localizations_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AppInfoAppInfoLocalizationsLinkagesResponse**](AppInfoAppInfoLocalizationsLinkagesResponse.md)

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

# **app_infos_get_instance**
> AppInfoResponse app_infos_get_instance(id, fields_app_infos=fields_app_infos, fields_age_rating_declarations=fields_age_rating_declarations, fields_app_info_localizations=fields_app_info_localizations, fields_app_categories=fields_app_categories, include=include, limit_app_info_localizations=limit_app_info_localizations)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_info_response import AppInfoResponse
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
    api_instance = openapi_client.AppInfosApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_infos = ['fields_app_infos_example'] # List[str] | the fields to include for returned resources of type appInfos (optional)
    fields_age_rating_declarations = ['fields_age_rating_declarations_example'] # List[str] | the fields to include for returned resources of type ageRatingDeclarations (optional)
    fields_app_info_localizations = ['fields_app_info_localizations_example'] # List[str] | the fields to include for returned resources of type appInfoLocalizations (optional)
    fields_app_categories = ['fields_app_categories_example'] # List[str] | the fields to include for returned resources of type appCategories (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_info_localizations = 56 # int | maximum number of related appInfoLocalizations returned (when they are included) (optional)

    try:
        api_response = api_instance.app_infos_get_instance(id, fields_app_infos=fields_app_infos, fields_age_rating_declarations=fields_age_rating_declarations, fields_app_info_localizations=fields_app_info_localizations, fields_app_categories=fields_app_categories, include=include, limit_app_info_localizations=limit_app_info_localizations)
        print("The response of AppInfosApi->app_infos_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppInfosApi->app_infos_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_infos** | [**List[str]**](str.md)| the fields to include for returned resources of type appInfos | [optional] 
 **fields_age_rating_declarations** | [**List[str]**](str.md)| the fields to include for returned resources of type ageRatingDeclarations | [optional] 
 **fields_app_info_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appInfoLocalizations | [optional] 
 **fields_app_categories** | [**List[str]**](str.md)| the fields to include for returned resources of type appCategories | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_info_localizations** | **int**| maximum number of related appInfoLocalizations returned (when they are included) | [optional] 

### Return type

[**AppInfoResponse**](AppInfoResponse.md)

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
**200** | Single AppInfo |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_infos_primary_category_get_to_one_related**
> AppCategoryResponse app_infos_primary_category_get_to_one_related(id, fields_app_categories=fields_app_categories, include=include, limit_subcategories=limit_subcategories)

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
    api_instance = openapi_client.AppInfosApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_categories = ['fields_app_categories_example'] # List[str] | the fields to include for returned resources of type appCategories (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_subcategories = 56 # int | maximum number of related subcategories returned (when they are included) (optional)

    try:
        api_response = api_instance.app_infos_primary_category_get_to_one_related(id, fields_app_categories=fields_app_categories, include=include, limit_subcategories=limit_subcategories)
        print("The response of AppInfosApi->app_infos_primary_category_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppInfosApi->app_infos_primary_category_get_to_one_related: %s\n" % e)
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

# **app_infos_primary_category_get_to_one_relationship**
> AppInfoPrimaryCategoryLinkageResponse app_infos_primary_category_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_info_primary_category_linkage_response import AppInfoPrimaryCategoryLinkageResponse
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
    api_instance = openapi_client.AppInfosApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.app_infos_primary_category_get_to_one_relationship(id)
        print("The response of AppInfosApi->app_infos_primary_category_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppInfosApi->app_infos_primary_category_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**AppInfoPrimaryCategoryLinkageResponse**](AppInfoPrimaryCategoryLinkageResponse.md)

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

# **app_infos_primary_subcategory_one_get_to_one_related**
> AppCategoryResponse app_infos_primary_subcategory_one_get_to_one_related(id, fields_app_categories=fields_app_categories, include=include, limit_subcategories=limit_subcategories)

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
    api_instance = openapi_client.AppInfosApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_categories = ['fields_app_categories_example'] # List[str] | the fields to include for returned resources of type appCategories (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_subcategories = 56 # int | maximum number of related subcategories returned (when they are included) (optional)

    try:
        api_response = api_instance.app_infos_primary_subcategory_one_get_to_one_related(id, fields_app_categories=fields_app_categories, include=include, limit_subcategories=limit_subcategories)
        print("The response of AppInfosApi->app_infos_primary_subcategory_one_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppInfosApi->app_infos_primary_subcategory_one_get_to_one_related: %s\n" % e)
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

# **app_infos_primary_subcategory_one_get_to_one_relationship**
> AppInfoPrimarySubcategoryOneLinkageResponse app_infos_primary_subcategory_one_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_info_primary_subcategory_one_linkage_response import AppInfoPrimarySubcategoryOneLinkageResponse
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
    api_instance = openapi_client.AppInfosApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.app_infos_primary_subcategory_one_get_to_one_relationship(id)
        print("The response of AppInfosApi->app_infos_primary_subcategory_one_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppInfosApi->app_infos_primary_subcategory_one_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**AppInfoPrimarySubcategoryOneLinkageResponse**](AppInfoPrimarySubcategoryOneLinkageResponse.md)

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

# **app_infos_primary_subcategory_two_get_to_one_related**
> AppCategoryResponse app_infos_primary_subcategory_two_get_to_one_related(id, fields_app_categories=fields_app_categories, include=include, limit_subcategories=limit_subcategories)

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
    api_instance = openapi_client.AppInfosApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_categories = ['fields_app_categories_example'] # List[str] | the fields to include for returned resources of type appCategories (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_subcategories = 56 # int | maximum number of related subcategories returned (when they are included) (optional)

    try:
        api_response = api_instance.app_infos_primary_subcategory_two_get_to_one_related(id, fields_app_categories=fields_app_categories, include=include, limit_subcategories=limit_subcategories)
        print("The response of AppInfosApi->app_infos_primary_subcategory_two_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppInfosApi->app_infos_primary_subcategory_two_get_to_one_related: %s\n" % e)
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

# **app_infos_primary_subcategory_two_get_to_one_relationship**
> AppInfoPrimarySubcategoryTwoLinkageResponse app_infos_primary_subcategory_two_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_info_primary_subcategory_two_linkage_response import AppInfoPrimarySubcategoryTwoLinkageResponse
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
    api_instance = openapi_client.AppInfosApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.app_infos_primary_subcategory_two_get_to_one_relationship(id)
        print("The response of AppInfosApi->app_infos_primary_subcategory_two_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppInfosApi->app_infos_primary_subcategory_two_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**AppInfoPrimarySubcategoryTwoLinkageResponse**](AppInfoPrimarySubcategoryTwoLinkageResponse.md)

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

# **app_infos_secondary_category_get_to_one_related**
> AppCategoryResponse app_infos_secondary_category_get_to_one_related(id, fields_app_categories=fields_app_categories, include=include, limit_subcategories=limit_subcategories)

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
    api_instance = openapi_client.AppInfosApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_categories = ['fields_app_categories_example'] # List[str] | the fields to include for returned resources of type appCategories (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_subcategories = 56 # int | maximum number of related subcategories returned (when they are included) (optional)

    try:
        api_response = api_instance.app_infos_secondary_category_get_to_one_related(id, fields_app_categories=fields_app_categories, include=include, limit_subcategories=limit_subcategories)
        print("The response of AppInfosApi->app_infos_secondary_category_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppInfosApi->app_infos_secondary_category_get_to_one_related: %s\n" % e)
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

# **app_infos_secondary_category_get_to_one_relationship**
> AppInfoSecondaryCategoryLinkageResponse app_infos_secondary_category_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_info_secondary_category_linkage_response import AppInfoSecondaryCategoryLinkageResponse
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
    api_instance = openapi_client.AppInfosApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.app_infos_secondary_category_get_to_one_relationship(id)
        print("The response of AppInfosApi->app_infos_secondary_category_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppInfosApi->app_infos_secondary_category_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**AppInfoSecondaryCategoryLinkageResponse**](AppInfoSecondaryCategoryLinkageResponse.md)

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

# **app_infos_secondary_subcategory_one_get_to_one_related**
> AppCategoryResponse app_infos_secondary_subcategory_one_get_to_one_related(id, fields_app_categories=fields_app_categories, include=include, limit_subcategories=limit_subcategories)

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
    api_instance = openapi_client.AppInfosApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_categories = ['fields_app_categories_example'] # List[str] | the fields to include for returned resources of type appCategories (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_subcategories = 56 # int | maximum number of related subcategories returned (when they are included) (optional)

    try:
        api_response = api_instance.app_infos_secondary_subcategory_one_get_to_one_related(id, fields_app_categories=fields_app_categories, include=include, limit_subcategories=limit_subcategories)
        print("The response of AppInfosApi->app_infos_secondary_subcategory_one_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppInfosApi->app_infos_secondary_subcategory_one_get_to_one_related: %s\n" % e)
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

# **app_infos_secondary_subcategory_one_get_to_one_relationship**
> AppInfoSecondarySubcategoryOneLinkageResponse app_infos_secondary_subcategory_one_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_info_secondary_subcategory_one_linkage_response import AppInfoSecondarySubcategoryOneLinkageResponse
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
    api_instance = openapi_client.AppInfosApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.app_infos_secondary_subcategory_one_get_to_one_relationship(id)
        print("The response of AppInfosApi->app_infos_secondary_subcategory_one_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppInfosApi->app_infos_secondary_subcategory_one_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**AppInfoSecondarySubcategoryOneLinkageResponse**](AppInfoSecondarySubcategoryOneLinkageResponse.md)

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

# **app_infos_secondary_subcategory_two_get_to_one_related**
> AppCategoryResponse app_infos_secondary_subcategory_two_get_to_one_related(id, fields_app_categories=fields_app_categories, include=include, limit_subcategories=limit_subcategories)

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
    api_instance = openapi_client.AppInfosApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_categories = ['fields_app_categories_example'] # List[str] | the fields to include for returned resources of type appCategories (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_subcategories = 56 # int | maximum number of related subcategories returned (when they are included) (optional)

    try:
        api_response = api_instance.app_infos_secondary_subcategory_two_get_to_one_related(id, fields_app_categories=fields_app_categories, include=include, limit_subcategories=limit_subcategories)
        print("The response of AppInfosApi->app_infos_secondary_subcategory_two_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppInfosApi->app_infos_secondary_subcategory_two_get_to_one_related: %s\n" % e)
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

# **app_infos_secondary_subcategory_two_get_to_one_relationship**
> AppInfoSecondarySubcategoryTwoLinkageResponse app_infos_secondary_subcategory_two_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_info_secondary_subcategory_two_linkage_response import AppInfoSecondarySubcategoryTwoLinkageResponse
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
    api_instance = openapi_client.AppInfosApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.app_infos_secondary_subcategory_two_get_to_one_relationship(id)
        print("The response of AppInfosApi->app_infos_secondary_subcategory_two_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppInfosApi->app_infos_secondary_subcategory_two_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**AppInfoSecondarySubcategoryTwoLinkageResponse**](AppInfoSecondarySubcategoryTwoLinkageResponse.md)

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

# **app_infos_update_instance**
> AppInfoResponse app_infos_update_instance(id, app_info_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_info_response import AppInfoResponse
from openapi_client.models.app_info_update_request import AppInfoUpdateRequest
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
    api_instance = openapi_client.AppInfosApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    app_info_update_request = openapi_client.AppInfoUpdateRequest() # AppInfoUpdateRequest | AppInfo representation

    try:
        api_response = api_instance.app_infos_update_instance(id, app_info_update_request)
        print("The response of AppInfosApi->app_infos_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppInfosApi->app_infos_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **app_info_update_request** | [**AppInfoUpdateRequest**](AppInfoUpdateRequest.md)| AppInfo representation | 

### Return type

[**AppInfoResponse**](AppInfoResponse.md)

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
**200** | Single AppInfo |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

