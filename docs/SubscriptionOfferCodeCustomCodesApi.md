# openapi_client.SubscriptionOfferCodeCustomCodesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**subscription_offer_code_custom_codes_create_instance**](SubscriptionOfferCodeCustomCodesApi.md#subscription_offer_code_custom_codes_create_instance) | **POST** /v1/subscriptionOfferCodeCustomCodes | 
[**subscription_offer_code_custom_codes_get_instance**](SubscriptionOfferCodeCustomCodesApi.md#subscription_offer_code_custom_codes_get_instance) | **GET** /v1/subscriptionOfferCodeCustomCodes/{id} | 
[**subscription_offer_code_custom_codes_update_instance**](SubscriptionOfferCodeCustomCodesApi.md#subscription_offer_code_custom_codes_update_instance) | **PATCH** /v1/subscriptionOfferCodeCustomCodes/{id} | 


# **subscription_offer_code_custom_codes_create_instance**
> SubscriptionOfferCodeCustomCodeResponse subscription_offer_code_custom_codes_create_instance(subscription_offer_code_custom_code_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_offer_code_custom_code_create_request import SubscriptionOfferCodeCustomCodeCreateRequest
from openapi_client.models.subscription_offer_code_custom_code_response import SubscriptionOfferCodeCustomCodeResponse
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
    api_instance = openapi_client.SubscriptionOfferCodeCustomCodesApi(api_client)
    subscription_offer_code_custom_code_create_request = openapi_client.SubscriptionOfferCodeCustomCodeCreateRequest() # SubscriptionOfferCodeCustomCodeCreateRequest | SubscriptionOfferCodeCustomCode representation

    try:
        api_response = api_instance.subscription_offer_code_custom_codes_create_instance(subscription_offer_code_custom_code_create_request)
        print("The response of SubscriptionOfferCodeCustomCodesApi->subscription_offer_code_custom_codes_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionOfferCodeCustomCodesApi->subscription_offer_code_custom_codes_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subscription_offer_code_custom_code_create_request** | [**SubscriptionOfferCodeCustomCodeCreateRequest**](SubscriptionOfferCodeCustomCodeCreateRequest.md)| SubscriptionOfferCodeCustomCode representation | 

### Return type

[**SubscriptionOfferCodeCustomCodeResponse**](SubscriptionOfferCodeCustomCodeResponse.md)

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
**201** | Single SubscriptionOfferCodeCustomCode |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_offer_code_custom_codes_get_instance**
> SubscriptionOfferCodeCustomCodeResponse subscription_offer_code_custom_codes_get_instance(id, fields_subscription_offer_code_custom_codes=fields_subscription_offer_code_custom_codes, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_offer_code_custom_code_response import SubscriptionOfferCodeCustomCodeResponse
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
    api_instance = openapi_client.SubscriptionOfferCodeCustomCodesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_subscription_offer_code_custom_codes = ['fields_subscription_offer_code_custom_codes_example'] # List[str] | the fields to include for returned resources of type subscriptionOfferCodeCustomCodes (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.subscription_offer_code_custom_codes_get_instance(id, fields_subscription_offer_code_custom_codes=fields_subscription_offer_code_custom_codes, include=include)
        print("The response of SubscriptionOfferCodeCustomCodesApi->subscription_offer_code_custom_codes_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionOfferCodeCustomCodesApi->subscription_offer_code_custom_codes_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_subscription_offer_code_custom_codes** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionOfferCodeCustomCodes | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**SubscriptionOfferCodeCustomCodeResponse**](SubscriptionOfferCodeCustomCodeResponse.md)

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
**200** | Single SubscriptionOfferCodeCustomCode |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_offer_code_custom_codes_update_instance**
> SubscriptionOfferCodeCustomCodeResponse subscription_offer_code_custom_codes_update_instance(id, subscription_offer_code_custom_code_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_offer_code_custom_code_response import SubscriptionOfferCodeCustomCodeResponse
from openapi_client.models.subscription_offer_code_custom_code_update_request import SubscriptionOfferCodeCustomCodeUpdateRequest
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
    api_instance = openapi_client.SubscriptionOfferCodeCustomCodesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    subscription_offer_code_custom_code_update_request = openapi_client.SubscriptionOfferCodeCustomCodeUpdateRequest() # SubscriptionOfferCodeCustomCodeUpdateRequest | SubscriptionOfferCodeCustomCode representation

    try:
        api_response = api_instance.subscription_offer_code_custom_codes_update_instance(id, subscription_offer_code_custom_code_update_request)
        print("The response of SubscriptionOfferCodeCustomCodesApi->subscription_offer_code_custom_codes_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionOfferCodeCustomCodesApi->subscription_offer_code_custom_codes_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **subscription_offer_code_custom_code_update_request** | [**SubscriptionOfferCodeCustomCodeUpdateRequest**](SubscriptionOfferCodeCustomCodeUpdateRequest.md)| SubscriptionOfferCodeCustomCode representation | 

### Return type

[**SubscriptionOfferCodeCustomCodeResponse**](SubscriptionOfferCodeCustomCodeResponse.md)

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
**200** | Single SubscriptionOfferCodeCustomCode |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

