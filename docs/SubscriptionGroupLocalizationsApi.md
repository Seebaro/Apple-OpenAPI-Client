# openapi_client.SubscriptionGroupLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**subscription_group_localizations_create_instance**](SubscriptionGroupLocalizationsApi.md#subscription_group_localizations_create_instance) | **POST** /v1/subscriptionGroupLocalizations | 
[**subscription_group_localizations_delete_instance**](SubscriptionGroupLocalizationsApi.md#subscription_group_localizations_delete_instance) | **DELETE** /v1/subscriptionGroupLocalizations/{id} | 
[**subscription_group_localizations_get_instance**](SubscriptionGroupLocalizationsApi.md#subscription_group_localizations_get_instance) | **GET** /v1/subscriptionGroupLocalizations/{id} | 
[**subscription_group_localizations_update_instance**](SubscriptionGroupLocalizationsApi.md#subscription_group_localizations_update_instance) | **PATCH** /v1/subscriptionGroupLocalizations/{id} | 


# **subscription_group_localizations_create_instance**
> SubscriptionGroupLocalizationResponse subscription_group_localizations_create_instance(subscription_group_localization_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_group_localization_create_request import SubscriptionGroupLocalizationCreateRequest
from openapi_client.models.subscription_group_localization_response import SubscriptionGroupLocalizationResponse
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
    api_instance = openapi_client.SubscriptionGroupLocalizationsApi(api_client)
    subscription_group_localization_create_request = openapi_client.SubscriptionGroupLocalizationCreateRequest() # SubscriptionGroupLocalizationCreateRequest | SubscriptionGroupLocalization representation

    try:
        api_response = api_instance.subscription_group_localizations_create_instance(subscription_group_localization_create_request)
        print("The response of SubscriptionGroupLocalizationsApi->subscription_group_localizations_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionGroupLocalizationsApi->subscription_group_localizations_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subscription_group_localization_create_request** | [**SubscriptionGroupLocalizationCreateRequest**](SubscriptionGroupLocalizationCreateRequest.md)| SubscriptionGroupLocalization representation | 

### Return type

[**SubscriptionGroupLocalizationResponse**](SubscriptionGroupLocalizationResponse.md)

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
**201** | Single SubscriptionGroupLocalization |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_group_localizations_delete_instance**
> subscription_group_localizations_delete_instance(id)

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
    api_instance = openapi_client.SubscriptionGroupLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.subscription_group_localizations_delete_instance(id)
    except Exception as e:
        print("Exception when calling SubscriptionGroupLocalizationsApi->subscription_group_localizations_delete_instance: %s\n" % e)
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

# **subscription_group_localizations_get_instance**
> SubscriptionGroupLocalizationResponse subscription_group_localizations_get_instance(id, fields_subscription_group_localizations=fields_subscription_group_localizations, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_group_localization_response import SubscriptionGroupLocalizationResponse
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
    api_instance = openapi_client.SubscriptionGroupLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_subscription_group_localizations = ['fields_subscription_group_localizations_example'] # List[str] | the fields to include for returned resources of type subscriptionGroupLocalizations (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.subscription_group_localizations_get_instance(id, fields_subscription_group_localizations=fields_subscription_group_localizations, include=include)
        print("The response of SubscriptionGroupLocalizationsApi->subscription_group_localizations_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionGroupLocalizationsApi->subscription_group_localizations_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_subscription_group_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionGroupLocalizations | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**SubscriptionGroupLocalizationResponse**](SubscriptionGroupLocalizationResponse.md)

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
**200** | Single SubscriptionGroupLocalization |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_group_localizations_update_instance**
> SubscriptionGroupLocalizationResponse subscription_group_localizations_update_instance(id, subscription_group_localization_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_group_localization_response import SubscriptionGroupLocalizationResponse
from openapi_client.models.subscription_group_localization_update_request import SubscriptionGroupLocalizationUpdateRequest
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
    api_instance = openapi_client.SubscriptionGroupLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    subscription_group_localization_update_request = openapi_client.SubscriptionGroupLocalizationUpdateRequest() # SubscriptionGroupLocalizationUpdateRequest | SubscriptionGroupLocalization representation

    try:
        api_response = api_instance.subscription_group_localizations_update_instance(id, subscription_group_localization_update_request)
        print("The response of SubscriptionGroupLocalizationsApi->subscription_group_localizations_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionGroupLocalizationsApi->subscription_group_localizations_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **subscription_group_localization_update_request** | [**SubscriptionGroupLocalizationUpdateRequest**](SubscriptionGroupLocalizationUpdateRequest.md)| SubscriptionGroupLocalization representation | 

### Return type

[**SubscriptionGroupLocalizationResponse**](SubscriptionGroupLocalizationResponse.md)

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
**200** | Single SubscriptionGroupLocalization |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

