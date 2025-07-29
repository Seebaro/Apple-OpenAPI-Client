# openapi_client.SubscriptionOfferCodeOneTimeUseCodesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**subscription_offer_code_one_time_use_codes_create_instance**](SubscriptionOfferCodeOneTimeUseCodesApi.md#subscription_offer_code_one_time_use_codes_create_instance) | **POST** /v1/subscriptionOfferCodeOneTimeUseCodes | 
[**subscription_offer_code_one_time_use_codes_get_instance**](SubscriptionOfferCodeOneTimeUseCodesApi.md#subscription_offer_code_one_time_use_codes_get_instance) | **GET** /v1/subscriptionOfferCodeOneTimeUseCodes/{id} | 
[**subscription_offer_code_one_time_use_codes_update_instance**](SubscriptionOfferCodeOneTimeUseCodesApi.md#subscription_offer_code_one_time_use_codes_update_instance) | **PATCH** /v1/subscriptionOfferCodeOneTimeUseCodes/{id} | 
[**subscription_offer_code_one_time_use_codes_values_get_to_one_related**](SubscriptionOfferCodeOneTimeUseCodesApi.md#subscription_offer_code_one_time_use_codes_values_get_to_one_related) | **GET** /v1/subscriptionOfferCodeOneTimeUseCodes/{id}/values | 


# **subscription_offer_code_one_time_use_codes_create_instance**
> SubscriptionOfferCodeOneTimeUseCodeResponse subscription_offer_code_one_time_use_codes_create_instance(subscription_offer_code_one_time_use_code_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_offer_code_one_time_use_code_create_request import SubscriptionOfferCodeOneTimeUseCodeCreateRequest
from openapi_client.models.subscription_offer_code_one_time_use_code_response import SubscriptionOfferCodeOneTimeUseCodeResponse
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
    api_instance = openapi_client.SubscriptionOfferCodeOneTimeUseCodesApi(api_client)
    subscription_offer_code_one_time_use_code_create_request = openapi_client.SubscriptionOfferCodeOneTimeUseCodeCreateRequest() # SubscriptionOfferCodeOneTimeUseCodeCreateRequest | SubscriptionOfferCodeOneTimeUseCode representation

    try:
        api_response = api_instance.subscription_offer_code_one_time_use_codes_create_instance(subscription_offer_code_one_time_use_code_create_request)
        print("The response of SubscriptionOfferCodeOneTimeUseCodesApi->subscription_offer_code_one_time_use_codes_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionOfferCodeOneTimeUseCodesApi->subscription_offer_code_one_time_use_codes_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subscription_offer_code_one_time_use_code_create_request** | [**SubscriptionOfferCodeOneTimeUseCodeCreateRequest**](SubscriptionOfferCodeOneTimeUseCodeCreateRequest.md)| SubscriptionOfferCodeOneTimeUseCode representation | 

### Return type

[**SubscriptionOfferCodeOneTimeUseCodeResponse**](SubscriptionOfferCodeOneTimeUseCodeResponse.md)

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
**201** | Single SubscriptionOfferCodeOneTimeUseCode |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_offer_code_one_time_use_codes_get_instance**
> SubscriptionOfferCodeOneTimeUseCodeResponse subscription_offer_code_one_time_use_codes_get_instance(id, fields_subscription_offer_code_one_time_use_codes=fields_subscription_offer_code_one_time_use_codes, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_offer_code_one_time_use_code_response import SubscriptionOfferCodeOneTimeUseCodeResponse
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
    api_instance = openapi_client.SubscriptionOfferCodeOneTimeUseCodesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_subscription_offer_code_one_time_use_codes = ['fields_subscription_offer_code_one_time_use_codes_example'] # List[str] | the fields to include for returned resources of type subscriptionOfferCodeOneTimeUseCodes (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.subscription_offer_code_one_time_use_codes_get_instance(id, fields_subscription_offer_code_one_time_use_codes=fields_subscription_offer_code_one_time_use_codes, include=include)
        print("The response of SubscriptionOfferCodeOneTimeUseCodesApi->subscription_offer_code_one_time_use_codes_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionOfferCodeOneTimeUseCodesApi->subscription_offer_code_one_time_use_codes_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_subscription_offer_code_one_time_use_codes** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionOfferCodeOneTimeUseCodes | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**SubscriptionOfferCodeOneTimeUseCodeResponse**](SubscriptionOfferCodeOneTimeUseCodeResponse.md)

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
**200** | Single SubscriptionOfferCodeOneTimeUseCode |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_offer_code_one_time_use_codes_update_instance**
> SubscriptionOfferCodeOneTimeUseCodeResponse subscription_offer_code_one_time_use_codes_update_instance(id, subscription_offer_code_one_time_use_code_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_offer_code_one_time_use_code_response import SubscriptionOfferCodeOneTimeUseCodeResponse
from openapi_client.models.subscription_offer_code_one_time_use_code_update_request import SubscriptionOfferCodeOneTimeUseCodeUpdateRequest
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
    api_instance = openapi_client.SubscriptionOfferCodeOneTimeUseCodesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    subscription_offer_code_one_time_use_code_update_request = openapi_client.SubscriptionOfferCodeOneTimeUseCodeUpdateRequest() # SubscriptionOfferCodeOneTimeUseCodeUpdateRequest | SubscriptionOfferCodeOneTimeUseCode representation

    try:
        api_response = api_instance.subscription_offer_code_one_time_use_codes_update_instance(id, subscription_offer_code_one_time_use_code_update_request)
        print("The response of SubscriptionOfferCodeOneTimeUseCodesApi->subscription_offer_code_one_time_use_codes_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionOfferCodeOneTimeUseCodesApi->subscription_offer_code_one_time_use_codes_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **subscription_offer_code_one_time_use_code_update_request** | [**SubscriptionOfferCodeOneTimeUseCodeUpdateRequest**](SubscriptionOfferCodeOneTimeUseCodeUpdateRequest.md)| SubscriptionOfferCodeOneTimeUseCode representation | 

### Return type

[**SubscriptionOfferCodeOneTimeUseCodeResponse**](SubscriptionOfferCodeOneTimeUseCodeResponse.md)

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
**200** | Single SubscriptionOfferCodeOneTimeUseCode |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_offer_code_one_time_use_codes_values_get_to_one_related**
> str subscription_offer_code_one_time_use_codes_values_get_to_one_related(id)

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
    api_instance = openapi_client.SubscriptionOfferCodeOneTimeUseCodesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.subscription_offer_code_one_time_use_codes_values_get_to_one_related(id)
        print("The response of SubscriptionOfferCodeOneTimeUseCodesApi->subscription_offer_code_one_time_use_codes_values_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionOfferCodeOneTimeUseCodesApi->subscription_offer_code_one_time_use_codes_values_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

**str**

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
**404** | Not found error |  -  |
**200** | Single SubscriptionOfferCodeOneTimeUseCodeValue |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

