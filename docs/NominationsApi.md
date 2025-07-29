# openapi_client.NominationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**nominations_create_instance**](NominationsApi.md#nominations_create_instance) | **POST** /v1/nominations | 
[**nominations_delete_instance**](NominationsApi.md#nominations_delete_instance) | **DELETE** /v1/nominations/{id} | 
[**nominations_get_collection**](NominationsApi.md#nominations_get_collection) | **GET** /v1/nominations | 
[**nominations_get_instance**](NominationsApi.md#nominations_get_instance) | **GET** /v1/nominations/{id} | 
[**nominations_update_instance**](NominationsApi.md#nominations_update_instance) | **PATCH** /v1/nominations/{id} | 


# **nominations_create_instance**
> NominationResponse nominations_create_instance(nomination_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.nomination_create_request import NominationCreateRequest
from openapi_client.models.nomination_response import NominationResponse
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
    api_instance = openapi_client.NominationsApi(api_client)
    nomination_create_request = openapi_client.NominationCreateRequest() # NominationCreateRequest | Nomination representation

    try:
        api_response = api_instance.nominations_create_instance(nomination_create_request)
        print("The response of NominationsApi->nominations_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NominationsApi->nominations_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **nomination_create_request** | [**NominationCreateRequest**](NominationCreateRequest.md)| Nomination representation | 

### Return type

[**NominationResponse**](NominationResponse.md)

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
**201** | Single Nomination |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **nominations_delete_instance**
> nominations_delete_instance(id)

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
    api_instance = openapi_client.NominationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.nominations_delete_instance(id)
    except Exception as e:
        print("Exception when calling NominationsApi->nominations_delete_instance: %s\n" % e)
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

# **nominations_get_collection**
> NominationsResponse nominations_get_collection(filter_state, filter_type=filter_type, filter_related_apps=filter_related_apps, sort=sort, fields_nominations=fields_nominations, limit=limit, include=include, limit_in_app_events=limit_in_app_events, limit_related_apps=limit_related_apps, limit_supported_territories=limit_supported_territories)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.nominations_response import NominationsResponse
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
    api_instance = openapi_client.NominationsApi(api_client)
    filter_state = ['filter_state_example'] # List[str] | filter by attribute 'state'
    filter_type = ['filter_type_example'] # List[str] | filter by attribute 'type' (optional)
    filter_related_apps = ['filter_related_apps_example'] # List[str] | filter by id(s) of related 'relatedApps' (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; resources will be sorted as specified (optional)
    fields_nominations = ['fields_nominations_example'] # List[str] | the fields to include for returned resources of type nominations (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_in_app_events = 56 # int | maximum number of related inAppEvents returned (when they are included) (optional)
    limit_related_apps = 56 # int | maximum number of related relatedApps returned (when they are included) (optional)
    limit_supported_territories = 56 # int | maximum number of related supportedTerritories returned (when they are included) (optional)

    try:
        api_response = api_instance.nominations_get_collection(filter_state, filter_type=filter_type, filter_related_apps=filter_related_apps, sort=sort, fields_nominations=fields_nominations, limit=limit, include=include, limit_in_app_events=limit_in_app_events, limit_related_apps=limit_related_apps, limit_supported_territories=limit_supported_territories)
        print("The response of NominationsApi->nominations_get_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NominationsApi->nominations_get_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter_state** | [**List[str]**](str.md)| filter by attribute &#39;state&#39; | 
 **filter_type** | [**List[str]**](str.md)| filter by attribute &#39;type&#39; | [optional] 
 **filter_related_apps** | [**List[str]**](str.md)| filter by id(s) of related &#39;relatedApps&#39; | [optional] 
 **sort** | [**List[str]**](str.md)| comma-separated list of sort expressions; resources will be sorted as specified | [optional] 
 **fields_nominations** | [**List[str]**](str.md)| the fields to include for returned resources of type nominations | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_in_app_events** | **int**| maximum number of related inAppEvents returned (when they are included) | [optional] 
 **limit_related_apps** | **int**| maximum number of related relatedApps returned (when they are included) | [optional] 
 **limit_supported_territories** | **int**| maximum number of related supportedTerritories returned (when they are included) | [optional] 

### Return type

[**NominationsResponse**](NominationsResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/csv

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**200** | List of Nominations |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **nominations_get_instance**
> NominationResponse nominations_get_instance(id, fields_nominations=fields_nominations, include=include, limit_in_app_events=limit_in_app_events, limit_related_apps=limit_related_apps, limit_supported_territories=limit_supported_territories)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.nomination_response import NominationResponse
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
    api_instance = openapi_client.NominationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_nominations = ['fields_nominations_example'] # List[str] | the fields to include for returned resources of type nominations (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_in_app_events = 56 # int | maximum number of related inAppEvents returned (when they are included) (optional)
    limit_related_apps = 56 # int | maximum number of related relatedApps returned (when they are included) (optional)
    limit_supported_territories = 56 # int | maximum number of related supportedTerritories returned (when they are included) (optional)

    try:
        api_response = api_instance.nominations_get_instance(id, fields_nominations=fields_nominations, include=include, limit_in_app_events=limit_in_app_events, limit_related_apps=limit_related_apps, limit_supported_territories=limit_supported_territories)
        print("The response of NominationsApi->nominations_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NominationsApi->nominations_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_nominations** | [**List[str]**](str.md)| the fields to include for returned resources of type nominations | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_in_app_events** | **int**| maximum number of related inAppEvents returned (when they are included) | [optional] 
 **limit_related_apps** | **int**| maximum number of related relatedApps returned (when they are included) | [optional] 
 **limit_supported_territories** | **int**| maximum number of related supportedTerritories returned (when they are included) | [optional] 

### Return type

[**NominationResponse**](NominationResponse.md)

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
**200** | Single Nomination |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **nominations_update_instance**
> NominationResponse nominations_update_instance(id, nomination_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.nomination_response import NominationResponse
from openapi_client.models.nomination_update_request import NominationUpdateRequest
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
    api_instance = openapi_client.NominationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    nomination_update_request = openapi_client.NominationUpdateRequest() # NominationUpdateRequest | Nomination representation

    try:
        api_response = api_instance.nominations_update_instance(id, nomination_update_request)
        print("The response of NominationsApi->nominations_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NominationsApi->nominations_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **nomination_update_request** | [**NominationUpdateRequest**](NominationUpdateRequest.md)| Nomination representation | 

### Return type

[**NominationResponse**](NominationResponse.md)

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
**200** | Single Nomination |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

