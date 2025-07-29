# openapi_client.AppPriceSchedulesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**app_price_schedules_automatic_prices_get_to_many_related**](AppPriceSchedulesApi.md#app_price_schedules_automatic_prices_get_to_many_related) | **GET** /v1/appPriceSchedules/{id}/automaticPrices | 
[**app_price_schedules_automatic_prices_get_to_many_relationship**](AppPriceSchedulesApi.md#app_price_schedules_automatic_prices_get_to_many_relationship) | **GET** /v1/appPriceSchedules/{id}/relationships/automaticPrices | 
[**app_price_schedules_base_territory_get_to_one_related**](AppPriceSchedulesApi.md#app_price_schedules_base_territory_get_to_one_related) | **GET** /v1/appPriceSchedules/{id}/baseTerritory | 
[**app_price_schedules_base_territory_get_to_one_relationship**](AppPriceSchedulesApi.md#app_price_schedules_base_territory_get_to_one_relationship) | **GET** /v1/appPriceSchedules/{id}/relationships/baseTerritory | 
[**app_price_schedules_create_instance**](AppPriceSchedulesApi.md#app_price_schedules_create_instance) | **POST** /v1/appPriceSchedules | 
[**app_price_schedules_get_instance**](AppPriceSchedulesApi.md#app_price_schedules_get_instance) | **GET** /v1/appPriceSchedules/{id} | 
[**app_price_schedules_manual_prices_get_to_many_related**](AppPriceSchedulesApi.md#app_price_schedules_manual_prices_get_to_many_related) | **GET** /v1/appPriceSchedules/{id}/manualPrices | 
[**app_price_schedules_manual_prices_get_to_many_relationship**](AppPriceSchedulesApi.md#app_price_schedules_manual_prices_get_to_many_relationship) | **GET** /v1/appPriceSchedules/{id}/relationships/manualPrices | 


# **app_price_schedules_automatic_prices_get_to_many_related**
> AppPricesV2Response app_price_schedules_automatic_prices_get_to_many_related(id, filter_start_date=filter_start_date, filter_end_date=filter_end_date, filter_territory=filter_territory, fields_app_prices=fields_app_prices, fields_app_price_points=fields_app_price_points, fields_territories=fields_territories, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_prices_v2_response import AppPricesV2Response
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
    api_instance = openapi_client.AppPriceSchedulesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_start_date = ['filter_start_date_example'] # List[str] | filter by attribute 'startDate' (optional)
    filter_end_date = ['filter_end_date_example'] # List[str] | filter by attribute 'endDate' (optional)
    filter_territory = ['filter_territory_example'] # List[str] | filter by id(s) of related 'territory' (optional)
    fields_app_prices = ['fields_app_prices_example'] # List[str] | the fields to include for returned resources of type appPrices (optional)
    fields_app_price_points = ['fields_app_price_points_example'] # List[str] | the fields to include for returned resources of type appPricePoints (optional)
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.app_price_schedules_automatic_prices_get_to_many_related(id, filter_start_date=filter_start_date, filter_end_date=filter_end_date, filter_territory=filter_territory, fields_app_prices=fields_app_prices, fields_app_price_points=fields_app_price_points, fields_territories=fields_territories, limit=limit, include=include)
        print("The response of AppPriceSchedulesApi->app_price_schedules_automatic_prices_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppPriceSchedulesApi->app_price_schedules_automatic_prices_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_start_date** | [**List[str]**](str.md)| filter by attribute &#39;startDate&#39; | [optional] 
 **filter_end_date** | [**List[str]**](str.md)| filter by attribute &#39;endDate&#39; | [optional] 
 **filter_territory** | [**List[str]**](str.md)| filter by id(s) of related &#39;territory&#39; | [optional] 
 **fields_app_prices** | [**List[str]**](str.md)| the fields to include for returned resources of type appPrices | [optional] 
 **fields_app_price_points** | [**List[str]**](str.md)| the fields to include for returned resources of type appPricePoints | [optional] 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**AppPricesV2Response**](AppPricesV2Response.md)

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
**200** | List of AppPrices |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_price_schedules_automatic_prices_get_to_many_relationship**
> AppPriceScheduleAutomaticPricesLinkagesResponse app_price_schedules_automatic_prices_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_price_schedule_automatic_prices_linkages_response import AppPriceScheduleAutomaticPricesLinkagesResponse
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
    api_instance = openapi_client.AppPriceSchedulesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.app_price_schedules_automatic_prices_get_to_many_relationship(id, limit=limit)
        print("The response of AppPriceSchedulesApi->app_price_schedules_automatic_prices_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppPriceSchedulesApi->app_price_schedules_automatic_prices_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AppPriceScheduleAutomaticPricesLinkagesResponse**](AppPriceScheduleAutomaticPricesLinkagesResponse.md)

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

# **app_price_schedules_base_territory_get_to_one_related**
> TerritoryResponse app_price_schedules_base_territory_get_to_one_related(id, fields_territories=fields_territories)

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
    api_instance = openapi_client.AppPriceSchedulesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)

    try:
        api_response = api_instance.app_price_schedules_base_territory_get_to_one_related(id, fields_territories=fields_territories)
        print("The response of AppPriceSchedulesApi->app_price_schedules_base_territory_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppPriceSchedulesApi->app_price_schedules_base_territory_get_to_one_related: %s\n" % e)
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

# **app_price_schedules_base_territory_get_to_one_relationship**
> AppPriceScheduleBaseTerritoryLinkageResponse app_price_schedules_base_territory_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_price_schedule_base_territory_linkage_response import AppPriceScheduleBaseTerritoryLinkageResponse
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
    api_instance = openapi_client.AppPriceSchedulesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.app_price_schedules_base_territory_get_to_one_relationship(id)
        print("The response of AppPriceSchedulesApi->app_price_schedules_base_territory_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppPriceSchedulesApi->app_price_schedules_base_territory_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**AppPriceScheduleBaseTerritoryLinkageResponse**](AppPriceScheduleBaseTerritoryLinkageResponse.md)

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

# **app_price_schedules_create_instance**
> AppPriceScheduleResponse app_price_schedules_create_instance(app_price_schedule_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_price_schedule_create_request import AppPriceScheduleCreateRequest
from openapi_client.models.app_price_schedule_response import AppPriceScheduleResponse
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
    api_instance = openapi_client.AppPriceSchedulesApi(api_client)
    app_price_schedule_create_request = openapi_client.AppPriceScheduleCreateRequest() # AppPriceScheduleCreateRequest | AppPriceSchedule representation

    try:
        api_response = api_instance.app_price_schedules_create_instance(app_price_schedule_create_request)
        print("The response of AppPriceSchedulesApi->app_price_schedules_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppPriceSchedulesApi->app_price_schedules_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **app_price_schedule_create_request** | [**AppPriceScheduleCreateRequest**](AppPriceScheduleCreateRequest.md)| AppPriceSchedule representation | 

### Return type

[**AppPriceScheduleResponse**](AppPriceScheduleResponse.md)

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
**201** | Single AppPriceSchedule |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_price_schedules_get_instance**
> AppPriceScheduleResponse app_price_schedules_get_instance(id, fields_app_price_schedules=fields_app_price_schedules, fields_territories=fields_territories, fields_app_prices=fields_app_prices, include=include, limit_automatic_prices=limit_automatic_prices, limit_manual_prices=limit_manual_prices)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_price_schedule_response import AppPriceScheduleResponse
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
    api_instance = openapi_client.AppPriceSchedulesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_price_schedules = ['fields_app_price_schedules_example'] # List[str] | the fields to include for returned resources of type appPriceSchedules (optional)
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)
    fields_app_prices = ['fields_app_prices_example'] # List[str] | the fields to include for returned resources of type appPrices (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_automatic_prices = 56 # int | maximum number of related automaticPrices returned (when they are included) (optional)
    limit_manual_prices = 56 # int | maximum number of related manualPrices returned (when they are included) (optional)

    try:
        api_response = api_instance.app_price_schedules_get_instance(id, fields_app_price_schedules=fields_app_price_schedules, fields_territories=fields_territories, fields_app_prices=fields_app_prices, include=include, limit_automatic_prices=limit_automatic_prices, limit_manual_prices=limit_manual_prices)
        print("The response of AppPriceSchedulesApi->app_price_schedules_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppPriceSchedulesApi->app_price_schedules_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_price_schedules** | [**List[str]**](str.md)| the fields to include for returned resources of type appPriceSchedules | [optional] 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 
 **fields_app_prices** | [**List[str]**](str.md)| the fields to include for returned resources of type appPrices | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_automatic_prices** | **int**| maximum number of related automaticPrices returned (when they are included) | [optional] 
 **limit_manual_prices** | **int**| maximum number of related manualPrices returned (when they are included) | [optional] 

### Return type

[**AppPriceScheduleResponse**](AppPriceScheduleResponse.md)

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
**200** | Single AppPriceSchedule |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_price_schedules_manual_prices_get_to_many_related**
> AppPricesV2Response app_price_schedules_manual_prices_get_to_many_related(id, filter_start_date=filter_start_date, filter_end_date=filter_end_date, filter_territory=filter_territory, fields_app_prices=fields_app_prices, fields_app_price_points=fields_app_price_points, fields_territories=fields_territories, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_prices_v2_response import AppPricesV2Response
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
    api_instance = openapi_client.AppPriceSchedulesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_start_date = ['filter_start_date_example'] # List[str] | filter by attribute 'startDate' (optional)
    filter_end_date = ['filter_end_date_example'] # List[str] | filter by attribute 'endDate' (optional)
    filter_territory = ['filter_territory_example'] # List[str] | filter by id(s) of related 'territory' (optional)
    fields_app_prices = ['fields_app_prices_example'] # List[str] | the fields to include for returned resources of type appPrices (optional)
    fields_app_price_points = ['fields_app_price_points_example'] # List[str] | the fields to include for returned resources of type appPricePoints (optional)
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.app_price_schedules_manual_prices_get_to_many_related(id, filter_start_date=filter_start_date, filter_end_date=filter_end_date, filter_territory=filter_territory, fields_app_prices=fields_app_prices, fields_app_price_points=fields_app_price_points, fields_territories=fields_territories, limit=limit, include=include)
        print("The response of AppPriceSchedulesApi->app_price_schedules_manual_prices_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppPriceSchedulesApi->app_price_schedules_manual_prices_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_start_date** | [**List[str]**](str.md)| filter by attribute &#39;startDate&#39; | [optional] 
 **filter_end_date** | [**List[str]**](str.md)| filter by attribute &#39;endDate&#39; | [optional] 
 **filter_territory** | [**List[str]**](str.md)| filter by id(s) of related &#39;territory&#39; | [optional] 
 **fields_app_prices** | [**List[str]**](str.md)| the fields to include for returned resources of type appPrices | [optional] 
 **fields_app_price_points** | [**List[str]**](str.md)| the fields to include for returned resources of type appPricePoints | [optional] 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**AppPricesV2Response**](AppPricesV2Response.md)

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
**200** | List of AppPrices |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_price_schedules_manual_prices_get_to_many_relationship**
> AppPriceScheduleManualPricesLinkagesResponse app_price_schedules_manual_prices_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_price_schedule_manual_prices_linkages_response import AppPriceScheduleManualPricesLinkagesResponse
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
    api_instance = openapi_client.AppPriceSchedulesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.app_price_schedules_manual_prices_get_to_many_relationship(id, limit=limit)
        print("The response of AppPriceSchedulesApi->app_price_schedules_manual_prices_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppPriceSchedulesApi->app_price_schedules_manual_prices_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AppPriceScheduleManualPricesLinkagesResponse**](AppPriceScheduleManualPricesLinkagesResponse.md)

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

