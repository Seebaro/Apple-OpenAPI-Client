# openapi_client.BetaAppClipInvocationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**beta_app_clip_invocations_create_instance**](BetaAppClipInvocationsApi.md#beta_app_clip_invocations_create_instance) | **POST** /v1/betaAppClipInvocations | 
[**beta_app_clip_invocations_delete_instance**](BetaAppClipInvocationsApi.md#beta_app_clip_invocations_delete_instance) | **DELETE** /v1/betaAppClipInvocations/{id} | 
[**beta_app_clip_invocations_get_instance**](BetaAppClipInvocationsApi.md#beta_app_clip_invocations_get_instance) | **GET** /v1/betaAppClipInvocations/{id} | 
[**beta_app_clip_invocations_update_instance**](BetaAppClipInvocationsApi.md#beta_app_clip_invocations_update_instance) | **PATCH** /v1/betaAppClipInvocations/{id} | 


# **beta_app_clip_invocations_create_instance**
> BetaAppClipInvocationResponse beta_app_clip_invocations_create_instance(beta_app_clip_invocation_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.beta_app_clip_invocation_create_request import BetaAppClipInvocationCreateRequest
from openapi_client.models.beta_app_clip_invocation_response import BetaAppClipInvocationResponse
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
    api_instance = openapi_client.BetaAppClipInvocationsApi(api_client)
    beta_app_clip_invocation_create_request = openapi_client.BetaAppClipInvocationCreateRequest() # BetaAppClipInvocationCreateRequest | BetaAppClipInvocation representation

    try:
        api_response = api_instance.beta_app_clip_invocations_create_instance(beta_app_clip_invocation_create_request)
        print("The response of BetaAppClipInvocationsApi->beta_app_clip_invocations_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BetaAppClipInvocationsApi->beta_app_clip_invocations_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **beta_app_clip_invocation_create_request** | [**BetaAppClipInvocationCreateRequest**](BetaAppClipInvocationCreateRequest.md)| BetaAppClipInvocation representation | 

### Return type

[**BetaAppClipInvocationResponse**](BetaAppClipInvocationResponse.md)

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
**201** | Single BetaAppClipInvocation |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **beta_app_clip_invocations_delete_instance**
> beta_app_clip_invocations_delete_instance(id)

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
    api_instance = openapi_client.BetaAppClipInvocationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.beta_app_clip_invocations_delete_instance(id)
    except Exception as e:
        print("Exception when calling BetaAppClipInvocationsApi->beta_app_clip_invocations_delete_instance: %s\n" % e)
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

# **beta_app_clip_invocations_get_instance**
> BetaAppClipInvocationResponse beta_app_clip_invocations_get_instance(id, fields_beta_app_clip_invocations=fields_beta_app_clip_invocations, include=include, limit_beta_app_clip_invocation_localizations=limit_beta_app_clip_invocation_localizations)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.beta_app_clip_invocation_response import BetaAppClipInvocationResponse
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
    api_instance = openapi_client.BetaAppClipInvocationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_beta_app_clip_invocations = ['fields_beta_app_clip_invocations_example'] # List[str] | the fields to include for returned resources of type betaAppClipInvocations (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_beta_app_clip_invocation_localizations = 56 # int | maximum number of related betaAppClipInvocationLocalizations returned (when they are included) (optional)

    try:
        api_response = api_instance.beta_app_clip_invocations_get_instance(id, fields_beta_app_clip_invocations=fields_beta_app_clip_invocations, include=include, limit_beta_app_clip_invocation_localizations=limit_beta_app_clip_invocation_localizations)
        print("The response of BetaAppClipInvocationsApi->beta_app_clip_invocations_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BetaAppClipInvocationsApi->beta_app_clip_invocations_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_beta_app_clip_invocations** | [**List[str]**](str.md)| the fields to include for returned resources of type betaAppClipInvocations | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_beta_app_clip_invocation_localizations** | **int**| maximum number of related betaAppClipInvocationLocalizations returned (when they are included) | [optional] 

### Return type

[**BetaAppClipInvocationResponse**](BetaAppClipInvocationResponse.md)

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
**200** | Single BetaAppClipInvocation |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **beta_app_clip_invocations_update_instance**
> BetaAppClipInvocationResponse beta_app_clip_invocations_update_instance(id, beta_app_clip_invocation_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.beta_app_clip_invocation_response import BetaAppClipInvocationResponse
from openapi_client.models.beta_app_clip_invocation_update_request import BetaAppClipInvocationUpdateRequest
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
    api_instance = openapi_client.BetaAppClipInvocationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    beta_app_clip_invocation_update_request = openapi_client.BetaAppClipInvocationUpdateRequest() # BetaAppClipInvocationUpdateRequest | BetaAppClipInvocation representation

    try:
        api_response = api_instance.beta_app_clip_invocations_update_instance(id, beta_app_clip_invocation_update_request)
        print("The response of BetaAppClipInvocationsApi->beta_app_clip_invocations_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BetaAppClipInvocationsApi->beta_app_clip_invocations_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **beta_app_clip_invocation_update_request** | [**BetaAppClipInvocationUpdateRequest**](BetaAppClipInvocationUpdateRequest.md)| BetaAppClipInvocation representation | 

### Return type

[**BetaAppClipInvocationResponse**](BetaAppClipInvocationResponse.md)

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
**200** | Single BetaAppClipInvocation |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

