# openapi_client.BetaAppClipInvocationLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**beta_app_clip_invocation_localizations_create_instance**](BetaAppClipInvocationLocalizationsApi.md#beta_app_clip_invocation_localizations_create_instance) | **POST** /v1/betaAppClipInvocationLocalizations | 
[**beta_app_clip_invocation_localizations_delete_instance**](BetaAppClipInvocationLocalizationsApi.md#beta_app_clip_invocation_localizations_delete_instance) | **DELETE** /v1/betaAppClipInvocationLocalizations/{id} | 
[**beta_app_clip_invocation_localizations_update_instance**](BetaAppClipInvocationLocalizationsApi.md#beta_app_clip_invocation_localizations_update_instance) | **PATCH** /v1/betaAppClipInvocationLocalizations/{id} | 


# **beta_app_clip_invocation_localizations_create_instance**
> BetaAppClipInvocationLocalizationResponse beta_app_clip_invocation_localizations_create_instance(beta_app_clip_invocation_localization_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.beta_app_clip_invocation_localization_create_request import BetaAppClipInvocationLocalizationCreateRequest
from openapi_client.models.beta_app_clip_invocation_localization_response import BetaAppClipInvocationLocalizationResponse
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
    api_instance = openapi_client.BetaAppClipInvocationLocalizationsApi(api_client)
    beta_app_clip_invocation_localization_create_request = openapi_client.BetaAppClipInvocationLocalizationCreateRequest() # BetaAppClipInvocationLocalizationCreateRequest | BetaAppClipInvocationLocalization representation

    try:
        api_response = api_instance.beta_app_clip_invocation_localizations_create_instance(beta_app_clip_invocation_localization_create_request)
        print("The response of BetaAppClipInvocationLocalizationsApi->beta_app_clip_invocation_localizations_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BetaAppClipInvocationLocalizationsApi->beta_app_clip_invocation_localizations_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **beta_app_clip_invocation_localization_create_request** | [**BetaAppClipInvocationLocalizationCreateRequest**](BetaAppClipInvocationLocalizationCreateRequest.md)| BetaAppClipInvocationLocalization representation | 

### Return type

[**BetaAppClipInvocationLocalizationResponse**](BetaAppClipInvocationLocalizationResponse.md)

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
**201** | Single BetaAppClipInvocationLocalization |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **beta_app_clip_invocation_localizations_delete_instance**
> beta_app_clip_invocation_localizations_delete_instance(id)

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
    api_instance = openapi_client.BetaAppClipInvocationLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.beta_app_clip_invocation_localizations_delete_instance(id)
    except Exception as e:
        print("Exception when calling BetaAppClipInvocationLocalizationsApi->beta_app_clip_invocation_localizations_delete_instance: %s\n" % e)
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

# **beta_app_clip_invocation_localizations_update_instance**
> BetaAppClipInvocationLocalizationResponse beta_app_clip_invocation_localizations_update_instance(id, beta_app_clip_invocation_localization_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.beta_app_clip_invocation_localization_response import BetaAppClipInvocationLocalizationResponse
from openapi_client.models.beta_app_clip_invocation_localization_update_request import BetaAppClipInvocationLocalizationUpdateRequest
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
    api_instance = openapi_client.BetaAppClipInvocationLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    beta_app_clip_invocation_localization_update_request = openapi_client.BetaAppClipInvocationLocalizationUpdateRequest() # BetaAppClipInvocationLocalizationUpdateRequest | BetaAppClipInvocationLocalization representation

    try:
        api_response = api_instance.beta_app_clip_invocation_localizations_update_instance(id, beta_app_clip_invocation_localization_update_request)
        print("The response of BetaAppClipInvocationLocalizationsApi->beta_app_clip_invocation_localizations_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BetaAppClipInvocationLocalizationsApi->beta_app_clip_invocation_localizations_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **beta_app_clip_invocation_localization_update_request** | [**BetaAppClipInvocationLocalizationUpdateRequest**](BetaAppClipInvocationLocalizationUpdateRequest.md)| BetaAppClipInvocationLocalization representation | 

### Return type

[**BetaAppClipInvocationLocalizationResponse**](BetaAppClipInvocationLocalizationResponse.md)

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
**200** | Single BetaAppClipInvocationLocalization |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

