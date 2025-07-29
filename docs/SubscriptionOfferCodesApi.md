# openapi_client.SubscriptionOfferCodesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**subscription_offer_codes_create_instance**](SubscriptionOfferCodesApi.md#subscription_offer_codes_create_instance) | **POST** /v1/subscriptionOfferCodes | 
[**subscription_offer_codes_custom_codes_get_to_many_related**](SubscriptionOfferCodesApi.md#subscription_offer_codes_custom_codes_get_to_many_related) | **GET** /v1/subscriptionOfferCodes/{id}/customCodes | 
[**subscription_offer_codes_custom_codes_get_to_many_relationship**](SubscriptionOfferCodesApi.md#subscription_offer_codes_custom_codes_get_to_many_relationship) | **GET** /v1/subscriptionOfferCodes/{id}/relationships/customCodes | 
[**subscription_offer_codes_get_instance**](SubscriptionOfferCodesApi.md#subscription_offer_codes_get_instance) | **GET** /v1/subscriptionOfferCodes/{id} | 
[**subscription_offer_codes_one_time_use_codes_get_to_many_related**](SubscriptionOfferCodesApi.md#subscription_offer_codes_one_time_use_codes_get_to_many_related) | **GET** /v1/subscriptionOfferCodes/{id}/oneTimeUseCodes | 
[**subscription_offer_codes_one_time_use_codes_get_to_many_relationship**](SubscriptionOfferCodesApi.md#subscription_offer_codes_one_time_use_codes_get_to_many_relationship) | **GET** /v1/subscriptionOfferCodes/{id}/relationships/oneTimeUseCodes | 
[**subscription_offer_codes_prices_get_to_many_related**](SubscriptionOfferCodesApi.md#subscription_offer_codes_prices_get_to_many_related) | **GET** /v1/subscriptionOfferCodes/{id}/prices | 
[**subscription_offer_codes_prices_get_to_many_relationship**](SubscriptionOfferCodesApi.md#subscription_offer_codes_prices_get_to_many_relationship) | **GET** /v1/subscriptionOfferCodes/{id}/relationships/prices | 
[**subscription_offer_codes_update_instance**](SubscriptionOfferCodesApi.md#subscription_offer_codes_update_instance) | **PATCH** /v1/subscriptionOfferCodes/{id} | 


# **subscription_offer_codes_create_instance**
> SubscriptionOfferCodeResponse subscription_offer_codes_create_instance(subscription_offer_code_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_offer_code_create_request import SubscriptionOfferCodeCreateRequest
from openapi_client.models.subscription_offer_code_response import SubscriptionOfferCodeResponse
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
    api_instance = openapi_client.SubscriptionOfferCodesApi(api_client)
    subscription_offer_code_create_request = openapi_client.SubscriptionOfferCodeCreateRequest() # SubscriptionOfferCodeCreateRequest | SubscriptionOfferCode representation

    try:
        api_response = api_instance.subscription_offer_codes_create_instance(subscription_offer_code_create_request)
        print("The response of SubscriptionOfferCodesApi->subscription_offer_codes_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionOfferCodesApi->subscription_offer_codes_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subscription_offer_code_create_request** | [**SubscriptionOfferCodeCreateRequest**](SubscriptionOfferCodeCreateRequest.md)| SubscriptionOfferCode representation | 

### Return type

[**SubscriptionOfferCodeResponse**](SubscriptionOfferCodeResponse.md)

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
**201** | Single SubscriptionOfferCode |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_offer_codes_custom_codes_get_to_many_related**
> SubscriptionOfferCodeCustomCodesResponse subscription_offer_codes_custom_codes_get_to_many_related(id, fields_subscription_offer_code_custom_codes=fields_subscription_offer_code_custom_codes, fields_subscription_offer_codes=fields_subscription_offer_codes, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_offer_code_custom_codes_response import SubscriptionOfferCodeCustomCodesResponse
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
    api_instance = openapi_client.SubscriptionOfferCodesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_subscription_offer_code_custom_codes = ['fields_subscription_offer_code_custom_codes_example'] # List[str] | the fields to include for returned resources of type subscriptionOfferCodeCustomCodes (optional)
    fields_subscription_offer_codes = ['fields_subscription_offer_codes_example'] # List[str] | the fields to include for returned resources of type subscriptionOfferCodes (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.subscription_offer_codes_custom_codes_get_to_many_related(id, fields_subscription_offer_code_custom_codes=fields_subscription_offer_code_custom_codes, fields_subscription_offer_codes=fields_subscription_offer_codes, limit=limit, include=include)
        print("The response of SubscriptionOfferCodesApi->subscription_offer_codes_custom_codes_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionOfferCodesApi->subscription_offer_codes_custom_codes_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_subscription_offer_code_custom_codes** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionOfferCodeCustomCodes | [optional] 
 **fields_subscription_offer_codes** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionOfferCodes | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**SubscriptionOfferCodeCustomCodesResponse**](SubscriptionOfferCodeCustomCodesResponse.md)

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
**200** | List of SubscriptionOfferCodeCustomCodes |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_offer_codes_custom_codes_get_to_many_relationship**
> SubscriptionOfferCodeCustomCodesLinkagesResponse subscription_offer_codes_custom_codes_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_offer_code_custom_codes_linkages_response import SubscriptionOfferCodeCustomCodesLinkagesResponse
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
    api_instance = openapi_client.SubscriptionOfferCodesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.subscription_offer_codes_custom_codes_get_to_many_relationship(id, limit=limit)
        print("The response of SubscriptionOfferCodesApi->subscription_offer_codes_custom_codes_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionOfferCodesApi->subscription_offer_codes_custom_codes_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**SubscriptionOfferCodeCustomCodesLinkagesResponse**](SubscriptionOfferCodeCustomCodesLinkagesResponse.md)

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

# **subscription_offer_codes_get_instance**
> SubscriptionOfferCodeResponse subscription_offer_codes_get_instance(id, fields_subscription_offer_codes=fields_subscription_offer_codes, fields_subscription_offer_code_one_time_use_codes=fields_subscription_offer_code_one_time_use_codes, fields_subscription_offer_code_custom_codes=fields_subscription_offer_code_custom_codes, fields_subscription_offer_code_prices=fields_subscription_offer_code_prices, include=include, limit_custom_codes=limit_custom_codes, limit_one_time_use_codes=limit_one_time_use_codes, limit_prices=limit_prices)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_offer_code_response import SubscriptionOfferCodeResponse
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
    api_instance = openapi_client.SubscriptionOfferCodesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_subscription_offer_codes = ['fields_subscription_offer_codes_example'] # List[str] | the fields to include for returned resources of type subscriptionOfferCodes (optional)
    fields_subscription_offer_code_one_time_use_codes = ['fields_subscription_offer_code_one_time_use_codes_example'] # List[str] | the fields to include for returned resources of type subscriptionOfferCodeOneTimeUseCodes (optional)
    fields_subscription_offer_code_custom_codes = ['fields_subscription_offer_code_custom_codes_example'] # List[str] | the fields to include for returned resources of type subscriptionOfferCodeCustomCodes (optional)
    fields_subscription_offer_code_prices = ['fields_subscription_offer_code_prices_example'] # List[str] | the fields to include for returned resources of type subscriptionOfferCodePrices (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_custom_codes = 56 # int | maximum number of related customCodes returned (when they are included) (optional)
    limit_one_time_use_codes = 56 # int | maximum number of related oneTimeUseCodes returned (when they are included) (optional)
    limit_prices = 56 # int | maximum number of related prices returned (when they are included) (optional)

    try:
        api_response = api_instance.subscription_offer_codes_get_instance(id, fields_subscription_offer_codes=fields_subscription_offer_codes, fields_subscription_offer_code_one_time_use_codes=fields_subscription_offer_code_one_time_use_codes, fields_subscription_offer_code_custom_codes=fields_subscription_offer_code_custom_codes, fields_subscription_offer_code_prices=fields_subscription_offer_code_prices, include=include, limit_custom_codes=limit_custom_codes, limit_one_time_use_codes=limit_one_time_use_codes, limit_prices=limit_prices)
        print("The response of SubscriptionOfferCodesApi->subscription_offer_codes_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionOfferCodesApi->subscription_offer_codes_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_subscription_offer_codes** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionOfferCodes | [optional] 
 **fields_subscription_offer_code_one_time_use_codes** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionOfferCodeOneTimeUseCodes | [optional] 
 **fields_subscription_offer_code_custom_codes** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionOfferCodeCustomCodes | [optional] 
 **fields_subscription_offer_code_prices** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionOfferCodePrices | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_custom_codes** | **int**| maximum number of related customCodes returned (when they are included) | [optional] 
 **limit_one_time_use_codes** | **int**| maximum number of related oneTimeUseCodes returned (when they are included) | [optional] 
 **limit_prices** | **int**| maximum number of related prices returned (when they are included) | [optional] 

### Return type

[**SubscriptionOfferCodeResponse**](SubscriptionOfferCodeResponse.md)

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
**200** | Single SubscriptionOfferCode |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_offer_codes_one_time_use_codes_get_to_many_related**
> SubscriptionOfferCodeOneTimeUseCodesResponse subscription_offer_codes_one_time_use_codes_get_to_many_related(id, fields_subscription_offer_code_one_time_use_codes=fields_subscription_offer_code_one_time_use_codes, fields_subscription_offer_codes=fields_subscription_offer_codes, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_offer_code_one_time_use_codes_response import SubscriptionOfferCodeOneTimeUseCodesResponse
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
    api_instance = openapi_client.SubscriptionOfferCodesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_subscription_offer_code_one_time_use_codes = ['fields_subscription_offer_code_one_time_use_codes_example'] # List[str] | the fields to include for returned resources of type subscriptionOfferCodeOneTimeUseCodes (optional)
    fields_subscription_offer_codes = ['fields_subscription_offer_codes_example'] # List[str] | the fields to include for returned resources of type subscriptionOfferCodes (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.subscription_offer_codes_one_time_use_codes_get_to_many_related(id, fields_subscription_offer_code_one_time_use_codes=fields_subscription_offer_code_one_time_use_codes, fields_subscription_offer_codes=fields_subscription_offer_codes, limit=limit, include=include)
        print("The response of SubscriptionOfferCodesApi->subscription_offer_codes_one_time_use_codes_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionOfferCodesApi->subscription_offer_codes_one_time_use_codes_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_subscription_offer_code_one_time_use_codes** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionOfferCodeOneTimeUseCodes | [optional] 
 **fields_subscription_offer_codes** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionOfferCodes | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**SubscriptionOfferCodeOneTimeUseCodesResponse**](SubscriptionOfferCodeOneTimeUseCodesResponse.md)

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
**200** | List of SubscriptionOfferCodeOneTimeUseCodes |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_offer_codes_one_time_use_codes_get_to_many_relationship**
> SubscriptionOfferCodeOneTimeUseCodesLinkagesResponse subscription_offer_codes_one_time_use_codes_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_offer_code_one_time_use_codes_linkages_response import SubscriptionOfferCodeOneTimeUseCodesLinkagesResponse
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
    api_instance = openapi_client.SubscriptionOfferCodesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.subscription_offer_codes_one_time_use_codes_get_to_many_relationship(id, limit=limit)
        print("The response of SubscriptionOfferCodesApi->subscription_offer_codes_one_time_use_codes_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionOfferCodesApi->subscription_offer_codes_one_time_use_codes_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**SubscriptionOfferCodeOneTimeUseCodesLinkagesResponse**](SubscriptionOfferCodeOneTimeUseCodesLinkagesResponse.md)

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

# **subscription_offer_codes_prices_get_to_many_related**
> SubscriptionOfferCodePricesResponse subscription_offer_codes_prices_get_to_many_related(id, filter_territory=filter_territory, fields_subscription_offer_code_prices=fields_subscription_offer_code_prices, fields_territories=fields_territories, fields_subscription_price_points=fields_subscription_price_points, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_offer_code_prices_response import SubscriptionOfferCodePricesResponse
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
    api_instance = openapi_client.SubscriptionOfferCodesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_territory = ['filter_territory_example'] # List[str] | filter by id(s) of related 'territory' (optional)
    fields_subscription_offer_code_prices = ['fields_subscription_offer_code_prices_example'] # List[str] | the fields to include for returned resources of type subscriptionOfferCodePrices (optional)
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)
    fields_subscription_price_points = ['fields_subscription_price_points_example'] # List[str] | the fields to include for returned resources of type subscriptionPricePoints (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.subscription_offer_codes_prices_get_to_many_related(id, filter_territory=filter_territory, fields_subscription_offer_code_prices=fields_subscription_offer_code_prices, fields_territories=fields_territories, fields_subscription_price_points=fields_subscription_price_points, limit=limit, include=include)
        print("The response of SubscriptionOfferCodesApi->subscription_offer_codes_prices_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionOfferCodesApi->subscription_offer_codes_prices_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_territory** | [**List[str]**](str.md)| filter by id(s) of related &#39;territory&#39; | [optional] 
 **fields_subscription_offer_code_prices** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionOfferCodePrices | [optional] 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 
 **fields_subscription_price_points** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionPricePoints | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**SubscriptionOfferCodePricesResponse**](SubscriptionOfferCodePricesResponse.md)

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
**200** | List of SubscriptionOfferCodePrices |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_offer_codes_prices_get_to_many_relationship**
> SubscriptionOfferCodePricesLinkagesResponse subscription_offer_codes_prices_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_offer_code_prices_linkages_response import SubscriptionOfferCodePricesLinkagesResponse
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
    api_instance = openapi_client.SubscriptionOfferCodesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.subscription_offer_codes_prices_get_to_many_relationship(id, limit=limit)
        print("The response of SubscriptionOfferCodesApi->subscription_offer_codes_prices_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionOfferCodesApi->subscription_offer_codes_prices_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**SubscriptionOfferCodePricesLinkagesResponse**](SubscriptionOfferCodePricesLinkagesResponse.md)

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

# **subscription_offer_codes_update_instance**
> SubscriptionOfferCodeResponse subscription_offer_codes_update_instance(id, subscription_offer_code_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_offer_code_response import SubscriptionOfferCodeResponse
from openapi_client.models.subscription_offer_code_update_request import SubscriptionOfferCodeUpdateRequest
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
    api_instance = openapi_client.SubscriptionOfferCodesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    subscription_offer_code_update_request = openapi_client.SubscriptionOfferCodeUpdateRequest() # SubscriptionOfferCodeUpdateRequest | SubscriptionOfferCode representation

    try:
        api_response = api_instance.subscription_offer_codes_update_instance(id, subscription_offer_code_update_request)
        print("The response of SubscriptionOfferCodesApi->subscription_offer_codes_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionOfferCodesApi->subscription_offer_codes_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **subscription_offer_code_update_request** | [**SubscriptionOfferCodeUpdateRequest**](SubscriptionOfferCodeUpdateRequest.md)| SubscriptionOfferCode representation | 

### Return type

[**SubscriptionOfferCodeResponse**](SubscriptionOfferCodeResponse.md)

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
**200** | Single SubscriptionOfferCode |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

