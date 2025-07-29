# openapi_client.SubscriptionPricePointsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**subscription_price_points_equalizations_get_to_many_related**](SubscriptionPricePointsApi.md#subscription_price_points_equalizations_get_to_many_related) | **GET** /v1/subscriptionPricePoints/{id}/equalizations | 
[**subscription_price_points_equalizations_get_to_many_relationship**](SubscriptionPricePointsApi.md#subscription_price_points_equalizations_get_to_many_relationship) | **GET** /v1/subscriptionPricePoints/{id}/relationships/equalizations | 
[**subscription_price_points_get_instance**](SubscriptionPricePointsApi.md#subscription_price_points_get_instance) | **GET** /v1/subscriptionPricePoints/{id} | 


# **subscription_price_points_equalizations_get_to_many_related**
> SubscriptionPricePointsResponse subscription_price_points_equalizations_get_to_many_related(id, filter_territory=filter_territory, filter_subscription=filter_subscription, fields_subscription_price_points=fields_subscription_price_points, fields_territories=fields_territories, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_price_points_response import SubscriptionPricePointsResponse
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
    api_instance = openapi_client.SubscriptionPricePointsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_territory = ['filter_territory_example'] # List[str] | filter by id(s) of related 'territory' (optional)
    filter_subscription = ['filter_subscription_example'] # List[str] | filter by id(s) of related 'subscription' (optional)
    fields_subscription_price_points = ['fields_subscription_price_points_example'] # List[str] | the fields to include for returned resources of type subscriptionPricePoints (optional)
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.subscription_price_points_equalizations_get_to_many_related(id, filter_territory=filter_territory, filter_subscription=filter_subscription, fields_subscription_price_points=fields_subscription_price_points, fields_territories=fields_territories, limit=limit, include=include)
        print("The response of SubscriptionPricePointsApi->subscription_price_points_equalizations_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionPricePointsApi->subscription_price_points_equalizations_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_territory** | [**List[str]**](str.md)| filter by id(s) of related &#39;territory&#39; | [optional] 
 **filter_subscription** | [**List[str]**](str.md)| filter by id(s) of related &#39;subscription&#39; | [optional] 
 **fields_subscription_price_points** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionPricePoints | [optional] 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**SubscriptionPricePointsResponse**](SubscriptionPricePointsResponse.md)

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
**200** | List of SubscriptionPricePoints |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_price_points_equalizations_get_to_many_relationship**
> SubscriptionPricePointEqualizationsLinkagesResponse subscription_price_points_equalizations_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_price_point_equalizations_linkages_response import SubscriptionPricePointEqualizationsLinkagesResponse
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
    api_instance = openapi_client.SubscriptionPricePointsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.subscription_price_points_equalizations_get_to_many_relationship(id, limit=limit)
        print("The response of SubscriptionPricePointsApi->subscription_price_points_equalizations_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionPricePointsApi->subscription_price_points_equalizations_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**SubscriptionPricePointEqualizationsLinkagesResponse**](SubscriptionPricePointEqualizationsLinkagesResponse.md)

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

# **subscription_price_points_get_instance**
> SubscriptionPricePointResponse subscription_price_points_get_instance(id, fields_subscription_price_points=fields_subscription_price_points, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_price_point_response import SubscriptionPricePointResponse
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
    api_instance = openapi_client.SubscriptionPricePointsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_subscription_price_points = ['fields_subscription_price_points_example'] # List[str] | the fields to include for returned resources of type subscriptionPricePoints (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.subscription_price_points_get_instance(id, fields_subscription_price_points=fields_subscription_price_points, include=include)
        print("The response of SubscriptionPricePointsApi->subscription_price_points_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionPricePointsApi->subscription_price_points_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_subscription_price_points** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionPricePoints | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**SubscriptionPricePointResponse**](SubscriptionPricePointResponse.md)

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
**200** | Single SubscriptionPricePoint |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

