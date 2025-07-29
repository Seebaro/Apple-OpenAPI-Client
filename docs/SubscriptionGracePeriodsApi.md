# openapi_client.SubscriptionGracePeriodsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**subscription_grace_periods_get_instance**](SubscriptionGracePeriodsApi.md#subscription_grace_periods_get_instance) | **GET** /v1/subscriptionGracePeriods/{id} | 
[**subscription_grace_periods_update_instance**](SubscriptionGracePeriodsApi.md#subscription_grace_periods_update_instance) | **PATCH** /v1/subscriptionGracePeriods/{id} | 


# **subscription_grace_periods_get_instance**
> SubscriptionGracePeriodResponse subscription_grace_periods_get_instance(id, fields_subscription_grace_periods=fields_subscription_grace_periods)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_grace_period_response import SubscriptionGracePeriodResponse
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
    api_instance = openapi_client.SubscriptionGracePeriodsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_subscription_grace_periods = ['fields_subscription_grace_periods_example'] # List[str] | the fields to include for returned resources of type subscriptionGracePeriods (optional)

    try:
        api_response = api_instance.subscription_grace_periods_get_instance(id, fields_subscription_grace_periods=fields_subscription_grace_periods)
        print("The response of SubscriptionGracePeriodsApi->subscription_grace_periods_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionGracePeriodsApi->subscription_grace_periods_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_subscription_grace_periods** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionGracePeriods | [optional] 

### Return type

[**SubscriptionGracePeriodResponse**](SubscriptionGracePeriodResponse.md)

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
**200** | Single SubscriptionGracePeriod |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_grace_periods_update_instance**
> SubscriptionGracePeriodResponse subscription_grace_periods_update_instance(id, subscription_grace_period_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_grace_period_response import SubscriptionGracePeriodResponse
from openapi_client.models.subscription_grace_period_update_request import SubscriptionGracePeriodUpdateRequest
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
    api_instance = openapi_client.SubscriptionGracePeriodsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    subscription_grace_period_update_request = openapi_client.SubscriptionGracePeriodUpdateRequest() # SubscriptionGracePeriodUpdateRequest | SubscriptionGracePeriod representation

    try:
        api_response = api_instance.subscription_grace_periods_update_instance(id, subscription_grace_period_update_request)
        print("The response of SubscriptionGracePeriodsApi->subscription_grace_periods_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionGracePeriodsApi->subscription_grace_periods_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **subscription_grace_period_update_request** | [**SubscriptionGracePeriodUpdateRequest**](SubscriptionGracePeriodUpdateRequest.md)| SubscriptionGracePeriod representation | 

### Return type

[**SubscriptionGracePeriodResponse**](SubscriptionGracePeriodResponse.md)

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
**200** | Single SubscriptionGracePeriod |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

