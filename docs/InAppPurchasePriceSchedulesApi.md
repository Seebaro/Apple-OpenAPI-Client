# openapi_client.InAppPurchasePriceSchedulesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**in_app_purchase_price_schedules_automatic_prices_get_to_many_related**](InAppPurchasePriceSchedulesApi.md#in_app_purchase_price_schedules_automatic_prices_get_to_many_related) | **GET** /v1/inAppPurchasePriceSchedules/{id}/automaticPrices | 
[**in_app_purchase_price_schedules_automatic_prices_get_to_many_relationship**](InAppPurchasePriceSchedulesApi.md#in_app_purchase_price_schedules_automatic_prices_get_to_many_relationship) | **GET** /v1/inAppPurchasePriceSchedules/{id}/relationships/automaticPrices | 
[**in_app_purchase_price_schedules_base_territory_get_to_one_related**](InAppPurchasePriceSchedulesApi.md#in_app_purchase_price_schedules_base_territory_get_to_one_related) | **GET** /v1/inAppPurchasePriceSchedules/{id}/baseTerritory | 
[**in_app_purchase_price_schedules_base_territory_get_to_one_relationship**](InAppPurchasePriceSchedulesApi.md#in_app_purchase_price_schedules_base_territory_get_to_one_relationship) | **GET** /v1/inAppPurchasePriceSchedules/{id}/relationships/baseTerritory | 
[**in_app_purchase_price_schedules_create_instance**](InAppPurchasePriceSchedulesApi.md#in_app_purchase_price_schedules_create_instance) | **POST** /v1/inAppPurchasePriceSchedules | 
[**in_app_purchase_price_schedules_get_instance**](InAppPurchasePriceSchedulesApi.md#in_app_purchase_price_schedules_get_instance) | **GET** /v1/inAppPurchasePriceSchedules/{id} | 
[**in_app_purchase_price_schedules_manual_prices_get_to_many_related**](InAppPurchasePriceSchedulesApi.md#in_app_purchase_price_schedules_manual_prices_get_to_many_related) | **GET** /v1/inAppPurchasePriceSchedules/{id}/manualPrices | 
[**in_app_purchase_price_schedules_manual_prices_get_to_many_relationship**](InAppPurchasePriceSchedulesApi.md#in_app_purchase_price_schedules_manual_prices_get_to_many_relationship) | **GET** /v1/inAppPurchasePriceSchedules/{id}/relationships/manualPrices | 


# **in_app_purchase_price_schedules_automatic_prices_get_to_many_related**
> InAppPurchasePricesResponse in_app_purchase_price_schedules_automatic_prices_get_to_many_related(id, filter_territory=filter_territory, fields_in_app_purchase_prices=fields_in_app_purchase_prices, fields_in_app_purchase_price_points=fields_in_app_purchase_price_points, fields_territories=fields_territories, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_prices_response import InAppPurchasePricesResponse
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
    api_instance = openapi_client.InAppPurchasePriceSchedulesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_territory = ['filter_territory_example'] # List[str] | filter by id(s) of related 'territory' (optional)
    fields_in_app_purchase_prices = ['fields_in_app_purchase_prices_example'] # List[str] | the fields to include for returned resources of type inAppPurchasePrices (optional)
    fields_in_app_purchase_price_points = ['fields_in_app_purchase_price_points_example'] # List[str] | the fields to include for returned resources of type inAppPurchasePricePoints (optional)
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.in_app_purchase_price_schedules_automatic_prices_get_to_many_related(id, filter_territory=filter_territory, fields_in_app_purchase_prices=fields_in_app_purchase_prices, fields_in_app_purchase_price_points=fields_in_app_purchase_price_points, fields_territories=fields_territories, limit=limit, include=include)
        print("The response of InAppPurchasePriceSchedulesApi->in_app_purchase_price_schedules_automatic_prices_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasePriceSchedulesApi->in_app_purchase_price_schedules_automatic_prices_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_territory** | [**List[str]**](str.md)| filter by id(s) of related &#39;territory&#39; | [optional] 
 **fields_in_app_purchase_prices** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchasePrices | [optional] 
 **fields_in_app_purchase_price_points** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchasePricePoints | [optional] 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**InAppPurchasePricesResponse**](InAppPurchasePricesResponse.md)

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
**200** | List of InAppPurchasePrices |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchase_price_schedules_automatic_prices_get_to_many_relationship**
> InAppPurchasePriceScheduleAutomaticPricesLinkagesResponse in_app_purchase_price_schedules_automatic_prices_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_price_schedule_automatic_prices_linkages_response import InAppPurchasePriceScheduleAutomaticPricesLinkagesResponse
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
    api_instance = openapi_client.InAppPurchasePriceSchedulesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.in_app_purchase_price_schedules_automatic_prices_get_to_many_relationship(id, limit=limit)
        print("The response of InAppPurchasePriceSchedulesApi->in_app_purchase_price_schedules_automatic_prices_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasePriceSchedulesApi->in_app_purchase_price_schedules_automatic_prices_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**InAppPurchasePriceScheduleAutomaticPricesLinkagesResponse**](InAppPurchasePriceScheduleAutomaticPricesLinkagesResponse.md)

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

# **in_app_purchase_price_schedules_base_territory_get_to_one_related**
> TerritoryResponse in_app_purchase_price_schedules_base_territory_get_to_one_related(id, fields_territories=fields_territories)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.territory_response import TerritoryResponse
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
    api_instance = openapi_client.InAppPurchasePriceSchedulesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)

    try:
        api_response = api_instance.in_app_purchase_price_schedules_base_territory_get_to_one_related(id, fields_territories=fields_territories)
        print("The response of InAppPurchasePriceSchedulesApi->in_app_purchase_price_schedules_base_territory_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasePriceSchedulesApi->in_app_purchase_price_schedules_base_territory_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 

### Return type

[**TerritoryResponse**](TerritoryResponse.md)

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
**200** | Single Territory |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchase_price_schedules_base_territory_get_to_one_relationship**
> InAppPurchasePriceScheduleBaseTerritoryLinkageResponse in_app_purchase_price_schedules_base_territory_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_price_schedule_base_territory_linkage_response import InAppPurchasePriceScheduleBaseTerritoryLinkageResponse
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
    api_instance = openapi_client.InAppPurchasePriceSchedulesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.in_app_purchase_price_schedules_base_territory_get_to_one_relationship(id)
        print("The response of InAppPurchasePriceSchedulesApi->in_app_purchase_price_schedules_base_territory_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasePriceSchedulesApi->in_app_purchase_price_schedules_base_territory_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**InAppPurchasePriceScheduleBaseTerritoryLinkageResponse**](InAppPurchasePriceScheduleBaseTerritoryLinkageResponse.md)

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

# **in_app_purchase_price_schedules_create_instance**
> InAppPurchasePriceScheduleResponse in_app_purchase_price_schedules_create_instance(in_app_purchase_price_schedule_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_price_schedule_create_request import InAppPurchasePriceScheduleCreateRequest
from openapi_client.models.in_app_purchase_price_schedule_response import InAppPurchasePriceScheduleResponse
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
    api_instance = openapi_client.InAppPurchasePriceSchedulesApi(api_client)
    in_app_purchase_price_schedule_create_request = openapi_client.InAppPurchasePriceScheduleCreateRequest() # InAppPurchasePriceScheduleCreateRequest | InAppPurchasePriceSchedule representation

    try:
        api_response = api_instance.in_app_purchase_price_schedules_create_instance(in_app_purchase_price_schedule_create_request)
        print("The response of InAppPurchasePriceSchedulesApi->in_app_purchase_price_schedules_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasePriceSchedulesApi->in_app_purchase_price_schedules_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **in_app_purchase_price_schedule_create_request** | [**InAppPurchasePriceScheduleCreateRequest**](InAppPurchasePriceScheduleCreateRequest.md)| InAppPurchasePriceSchedule representation | 

### Return type

[**InAppPurchasePriceScheduleResponse**](InAppPurchasePriceScheduleResponse.md)

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
**201** | Single InAppPurchasePriceSchedule |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchase_price_schedules_get_instance**
> InAppPurchasePriceScheduleResponse in_app_purchase_price_schedules_get_instance(id, fields_in_app_purchase_price_schedules=fields_in_app_purchase_price_schedules, fields_territories=fields_territories, fields_in_app_purchase_prices=fields_in_app_purchase_prices, include=include, limit_automatic_prices=limit_automatic_prices, limit_manual_prices=limit_manual_prices)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_price_schedule_response import InAppPurchasePriceScheduleResponse
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
    api_instance = openapi_client.InAppPurchasePriceSchedulesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_in_app_purchase_price_schedules = ['fields_in_app_purchase_price_schedules_example'] # List[str] | the fields to include for returned resources of type inAppPurchasePriceSchedules (optional)
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)
    fields_in_app_purchase_prices = ['fields_in_app_purchase_prices_example'] # List[str] | the fields to include for returned resources of type inAppPurchasePrices (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_automatic_prices = 56 # int | maximum number of related automaticPrices returned (when they are included) (optional)
    limit_manual_prices = 56 # int | maximum number of related manualPrices returned (when they are included) (optional)

    try:
        api_response = api_instance.in_app_purchase_price_schedules_get_instance(id, fields_in_app_purchase_price_schedules=fields_in_app_purchase_price_schedules, fields_territories=fields_territories, fields_in_app_purchase_prices=fields_in_app_purchase_prices, include=include, limit_automatic_prices=limit_automatic_prices, limit_manual_prices=limit_manual_prices)
        print("The response of InAppPurchasePriceSchedulesApi->in_app_purchase_price_schedules_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasePriceSchedulesApi->in_app_purchase_price_schedules_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_in_app_purchase_price_schedules** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchasePriceSchedules | [optional] 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 
 **fields_in_app_purchase_prices** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchasePrices | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_automatic_prices** | **int**| maximum number of related automaticPrices returned (when they are included) | [optional] 
 **limit_manual_prices** | **int**| maximum number of related manualPrices returned (when they are included) | [optional] 

### Return type

[**InAppPurchasePriceScheduleResponse**](InAppPurchasePriceScheduleResponse.md)

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
**200** | Single InAppPurchasePriceSchedule |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchase_price_schedules_manual_prices_get_to_many_related**
> InAppPurchasePricesResponse in_app_purchase_price_schedules_manual_prices_get_to_many_related(id, filter_territory=filter_territory, fields_in_app_purchase_prices=fields_in_app_purchase_prices, fields_in_app_purchase_price_points=fields_in_app_purchase_price_points, fields_territories=fields_territories, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_prices_response import InAppPurchasePricesResponse
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
    api_instance = openapi_client.InAppPurchasePriceSchedulesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_territory = ['filter_territory_example'] # List[str] | filter by id(s) of related 'territory' (optional)
    fields_in_app_purchase_prices = ['fields_in_app_purchase_prices_example'] # List[str] | the fields to include for returned resources of type inAppPurchasePrices (optional)
    fields_in_app_purchase_price_points = ['fields_in_app_purchase_price_points_example'] # List[str] | the fields to include for returned resources of type inAppPurchasePricePoints (optional)
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.in_app_purchase_price_schedules_manual_prices_get_to_many_related(id, filter_territory=filter_territory, fields_in_app_purchase_prices=fields_in_app_purchase_prices, fields_in_app_purchase_price_points=fields_in_app_purchase_price_points, fields_territories=fields_territories, limit=limit, include=include)
        print("The response of InAppPurchasePriceSchedulesApi->in_app_purchase_price_schedules_manual_prices_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasePriceSchedulesApi->in_app_purchase_price_schedules_manual_prices_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_territory** | [**List[str]**](str.md)| filter by id(s) of related &#39;territory&#39; | [optional] 
 **fields_in_app_purchase_prices** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchasePrices | [optional] 
 **fields_in_app_purchase_price_points** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchasePricePoints | [optional] 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**InAppPurchasePricesResponse**](InAppPurchasePricesResponse.md)

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
**200** | List of InAppPurchasePrices |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchase_price_schedules_manual_prices_get_to_many_relationship**
> InAppPurchasePriceScheduleManualPricesLinkagesResponse in_app_purchase_price_schedules_manual_prices_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_price_schedule_manual_prices_linkages_response import InAppPurchasePriceScheduleManualPricesLinkagesResponse
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
    api_instance = openapi_client.InAppPurchasePriceSchedulesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.in_app_purchase_price_schedules_manual_prices_get_to_many_relationship(id, limit=limit)
        print("The response of InAppPurchasePriceSchedulesApi->in_app_purchase_price_schedules_manual_prices_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasePriceSchedulesApi->in_app_purchase_price_schedules_manual_prices_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**InAppPurchasePriceScheduleManualPricesLinkagesResponse**](InAppPurchasePriceScheduleManualPricesLinkagesResponse.md)

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

