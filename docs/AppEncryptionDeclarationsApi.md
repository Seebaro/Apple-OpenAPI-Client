# openapi_client.AppEncryptionDeclarationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**app_encryption_declarations_app_encryption_declaration_document_get_to_one_related**](AppEncryptionDeclarationsApi.md#app_encryption_declarations_app_encryption_declaration_document_get_to_one_related) | **GET** /v1/appEncryptionDeclarations/{id}/appEncryptionDeclarationDocument | 
[**app_encryption_declarations_app_encryption_declaration_document_get_to_one_relationship**](AppEncryptionDeclarationsApi.md#app_encryption_declarations_app_encryption_declaration_document_get_to_one_relationship) | **GET** /v1/appEncryptionDeclarations/{id}/relationships/appEncryptionDeclarationDocument | 
[**app_encryption_declarations_app_get_to_one_related**](AppEncryptionDeclarationsApi.md#app_encryption_declarations_app_get_to_one_related) | **GET** /v1/appEncryptionDeclarations/{id}/app | 
[**app_encryption_declarations_app_get_to_one_relationship**](AppEncryptionDeclarationsApi.md#app_encryption_declarations_app_get_to_one_relationship) | **GET** /v1/appEncryptionDeclarations/{id}/relationships/app | 
[**app_encryption_declarations_builds_create_to_many_relationship**](AppEncryptionDeclarationsApi.md#app_encryption_declarations_builds_create_to_many_relationship) | **POST** /v1/appEncryptionDeclarations/{id}/relationships/builds | 
[**app_encryption_declarations_create_instance**](AppEncryptionDeclarationsApi.md#app_encryption_declarations_create_instance) | **POST** /v1/appEncryptionDeclarations | 
[**app_encryption_declarations_get_collection**](AppEncryptionDeclarationsApi.md#app_encryption_declarations_get_collection) | **GET** /v1/appEncryptionDeclarations | 
[**app_encryption_declarations_get_instance**](AppEncryptionDeclarationsApi.md#app_encryption_declarations_get_instance) | **GET** /v1/appEncryptionDeclarations/{id} | 


# **app_encryption_declarations_app_encryption_declaration_document_get_to_one_related**
> AppEncryptionDeclarationDocumentResponse app_encryption_declarations_app_encryption_declaration_document_get_to_one_related(id, fields_app_encryption_declaration_documents=fields_app_encryption_declaration_documents)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_encryption_declaration_document_response import AppEncryptionDeclarationDocumentResponse
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
    api_instance = openapi_client.AppEncryptionDeclarationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_encryption_declaration_documents = ['fields_app_encryption_declaration_documents_example'] # List[str] | the fields to include for returned resources of type appEncryptionDeclarationDocuments (optional)

    try:
        api_response = api_instance.app_encryption_declarations_app_encryption_declaration_document_get_to_one_related(id, fields_app_encryption_declaration_documents=fields_app_encryption_declaration_documents)
        print("The response of AppEncryptionDeclarationsApi->app_encryption_declarations_app_encryption_declaration_document_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEncryptionDeclarationsApi->app_encryption_declarations_app_encryption_declaration_document_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_encryption_declaration_documents** | [**List[str]**](str.md)| the fields to include for returned resources of type appEncryptionDeclarationDocuments | [optional] 

### Return type

[**AppEncryptionDeclarationDocumentResponse**](AppEncryptionDeclarationDocumentResponse.md)

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
**200** | Single AppEncryptionDeclarationDocument |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_encryption_declarations_app_encryption_declaration_document_get_to_one_relationship**
> AppEncryptionDeclarationAppEncryptionDeclarationDocumentLinkageResponse app_encryption_declarations_app_encryption_declaration_document_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_encryption_declaration_app_encryption_declaration_document_linkage_response import AppEncryptionDeclarationAppEncryptionDeclarationDocumentLinkageResponse
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
    api_instance = openapi_client.AppEncryptionDeclarationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.app_encryption_declarations_app_encryption_declaration_document_get_to_one_relationship(id)
        print("The response of AppEncryptionDeclarationsApi->app_encryption_declarations_app_encryption_declaration_document_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEncryptionDeclarationsApi->app_encryption_declarations_app_encryption_declaration_document_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**AppEncryptionDeclarationAppEncryptionDeclarationDocumentLinkageResponse**](AppEncryptionDeclarationAppEncryptionDeclarationDocumentLinkageResponse.md)

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

# **app_encryption_declarations_app_get_to_one_related**
> AppWithoutIncludesResponse app_encryption_declarations_app_get_to_one_related(id, fields_apps=fields_apps)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_without_includes_response import AppWithoutIncludesResponse
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
    api_instance = openapi_client.AppEncryptionDeclarationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_apps = ['fields_apps_example'] # List[str] | the fields to include for returned resources of type apps (optional)

    try:
        api_response = api_instance.app_encryption_declarations_app_get_to_one_related(id, fields_apps=fields_apps)
        print("The response of AppEncryptionDeclarationsApi->app_encryption_declarations_app_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEncryptionDeclarationsApi->app_encryption_declarations_app_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_apps** | [**List[str]**](str.md)| the fields to include for returned resources of type apps | [optional] 

### Return type

[**AppWithoutIncludesResponse**](AppWithoutIncludesResponse.md)

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
**200** | Single App with get |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_encryption_declarations_app_get_to_one_relationship**
> AppEncryptionDeclarationAppLinkageResponse app_encryption_declarations_app_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_encryption_declaration_app_linkage_response import AppEncryptionDeclarationAppLinkageResponse
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
    api_instance = openapi_client.AppEncryptionDeclarationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.app_encryption_declarations_app_get_to_one_relationship(id)
        print("The response of AppEncryptionDeclarationsApi->app_encryption_declarations_app_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEncryptionDeclarationsApi->app_encryption_declarations_app_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**AppEncryptionDeclarationAppLinkageResponse**](AppEncryptionDeclarationAppLinkageResponse.md)

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

# **app_encryption_declarations_builds_create_to_many_relationship**
> app_encryption_declarations_builds_create_to_many_relationship(id, app_encryption_declaration_builds_linkages_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_encryption_declaration_builds_linkages_request import AppEncryptionDeclarationBuildsLinkagesRequest
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
    api_instance = openapi_client.AppEncryptionDeclarationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    app_encryption_declaration_builds_linkages_request = openapi_client.AppEncryptionDeclarationBuildsLinkagesRequest() # AppEncryptionDeclarationBuildsLinkagesRequest | List of related linkages

    try:
        api_instance.app_encryption_declarations_builds_create_to_many_relationship(id, app_encryption_declaration_builds_linkages_request)
    except Exception as e:
        print("Exception when calling AppEncryptionDeclarationsApi->app_encryption_declarations_builds_create_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **app_encryption_declaration_builds_linkages_request** | [**AppEncryptionDeclarationBuildsLinkagesRequest**](AppEncryptionDeclarationBuildsLinkagesRequest.md)| List of related linkages | 

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

# **app_encryption_declarations_create_instance**
> AppEncryptionDeclarationResponse app_encryption_declarations_create_instance(app_encryption_declaration_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_encryption_declaration_create_request import AppEncryptionDeclarationCreateRequest
from openapi_client.models.app_encryption_declaration_response import AppEncryptionDeclarationResponse
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
    api_instance = openapi_client.AppEncryptionDeclarationsApi(api_client)
    app_encryption_declaration_create_request = openapi_client.AppEncryptionDeclarationCreateRequest() # AppEncryptionDeclarationCreateRequest | AppEncryptionDeclaration representation

    try:
        api_response = api_instance.app_encryption_declarations_create_instance(app_encryption_declaration_create_request)
        print("The response of AppEncryptionDeclarationsApi->app_encryption_declarations_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEncryptionDeclarationsApi->app_encryption_declarations_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **app_encryption_declaration_create_request** | [**AppEncryptionDeclarationCreateRequest**](AppEncryptionDeclarationCreateRequest.md)| AppEncryptionDeclaration representation | 

### Return type

[**AppEncryptionDeclarationResponse**](AppEncryptionDeclarationResponse.md)

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
**201** | Single AppEncryptionDeclaration |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_encryption_declarations_get_collection**
> AppEncryptionDeclarationsResponse app_encryption_declarations_get_collection(filter_platform=filter_platform, filter_app=filter_app, filter_builds=filter_builds, fields_app_encryption_declarations=fields_app_encryption_declarations, fields_apps=fields_apps, fields_app_encryption_declaration_documents=fields_app_encryption_declaration_documents, limit=limit, include=include, limit_builds=limit_builds)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_encryption_declarations_response import AppEncryptionDeclarationsResponse
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
    api_instance = openapi_client.AppEncryptionDeclarationsApi(api_client)
    filter_platform = ['filter_platform_example'] # List[str] | filter by attribute 'platform' (optional)
    filter_app = ['filter_app_example'] # List[str] | filter by id(s) of related 'app' (optional)
    filter_builds = ['filter_builds_example'] # List[str] | filter by id(s) of related 'builds' (optional)
    fields_app_encryption_declarations = ['fields_app_encryption_declarations_example'] # List[str] | the fields to include for returned resources of type appEncryptionDeclarations (optional)
    fields_apps = ['fields_apps_example'] # List[str] | the fields to include for returned resources of type apps (optional)
    fields_app_encryption_declaration_documents = ['fields_app_encryption_declaration_documents_example'] # List[str] | the fields to include for returned resources of type appEncryptionDeclarationDocuments (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_builds = 56 # int | maximum number of related builds returned (when they are included) (optional)

    try:
        api_response = api_instance.app_encryption_declarations_get_collection(filter_platform=filter_platform, filter_app=filter_app, filter_builds=filter_builds, fields_app_encryption_declarations=fields_app_encryption_declarations, fields_apps=fields_apps, fields_app_encryption_declaration_documents=fields_app_encryption_declaration_documents, limit=limit, include=include, limit_builds=limit_builds)
        print("The response of AppEncryptionDeclarationsApi->app_encryption_declarations_get_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEncryptionDeclarationsApi->app_encryption_declarations_get_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter_platform** | [**List[str]**](str.md)| filter by attribute &#39;platform&#39; | [optional] 
 **filter_app** | [**List[str]**](str.md)| filter by id(s) of related &#39;app&#39; | [optional] 
 **filter_builds** | [**List[str]**](str.md)| filter by id(s) of related &#39;builds&#39; | [optional] 
 **fields_app_encryption_declarations** | [**List[str]**](str.md)| the fields to include for returned resources of type appEncryptionDeclarations | [optional] 
 **fields_apps** | [**List[str]**](str.md)| the fields to include for returned resources of type apps | [optional] 
 **fields_app_encryption_declaration_documents** | [**List[str]**](str.md)| the fields to include for returned resources of type appEncryptionDeclarationDocuments | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_builds** | **int**| maximum number of related builds returned (when they are included) | [optional] 

### Return type

[**AppEncryptionDeclarationsResponse**](AppEncryptionDeclarationsResponse.md)

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
**200** | List of AppEncryptionDeclarations |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_encryption_declarations_get_instance**
> AppEncryptionDeclarationResponse app_encryption_declarations_get_instance(id, fields_app_encryption_declarations=fields_app_encryption_declarations, fields_apps=fields_apps, fields_app_encryption_declaration_documents=fields_app_encryption_declaration_documents, include=include, limit_builds=limit_builds)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_encryption_declaration_response import AppEncryptionDeclarationResponse
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
    api_instance = openapi_client.AppEncryptionDeclarationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_encryption_declarations = ['fields_app_encryption_declarations_example'] # List[str] | the fields to include for returned resources of type appEncryptionDeclarations (optional)
    fields_apps = ['fields_apps_example'] # List[str] | the fields to include for returned resources of type apps (optional)
    fields_app_encryption_declaration_documents = ['fields_app_encryption_declaration_documents_example'] # List[str] | the fields to include for returned resources of type appEncryptionDeclarationDocuments (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_builds = 56 # int | maximum number of related builds returned (when they are included) (optional)

    try:
        api_response = api_instance.app_encryption_declarations_get_instance(id, fields_app_encryption_declarations=fields_app_encryption_declarations, fields_apps=fields_apps, fields_app_encryption_declaration_documents=fields_app_encryption_declaration_documents, include=include, limit_builds=limit_builds)
        print("The response of AppEncryptionDeclarationsApi->app_encryption_declarations_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppEncryptionDeclarationsApi->app_encryption_declarations_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_encryption_declarations** | [**List[str]**](str.md)| the fields to include for returned resources of type appEncryptionDeclarations | [optional] 
 **fields_apps** | [**List[str]**](str.md)| the fields to include for returned resources of type apps | [optional] 
 **fields_app_encryption_declaration_documents** | [**List[str]**](str.md)| the fields to include for returned resources of type appEncryptionDeclarationDocuments | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_builds** | **int**| maximum number of related builds returned (when they are included) | [optional] 

### Return type

[**AppEncryptionDeclarationResponse**](AppEncryptionDeclarationResponse.md)

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
**200** | Single AppEncryptionDeclaration |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

