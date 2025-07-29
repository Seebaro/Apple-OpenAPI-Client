# openapi_client.AppAvailabilitiesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**app_availabilities_v2_create_instance**](AppAvailabilitiesApi.md#app_availabilities_v2_create_instance) | **POST** /v2/appAvailabilities | 
[**app_availabilities_v2_get_instance**](AppAvailabilitiesApi.md#app_availabilities_v2_get_instance) | **GET** /v2/appAvailabilities/{id} | 
[**app_availabilities_v2_territory_availabilities_get_to_many_related**](AppAvailabilitiesApi.md#app_availabilities_v2_territory_availabilities_get_to_many_related) | **GET** /v2/appAvailabilities/{id}/territoryAvailabilities | 
[**app_availabilities_v2_territory_availabilities_get_to_many_relationship**](AppAvailabilitiesApi.md#app_availabilities_v2_territory_availabilities_get_to_many_relationship) | **GET** /v2/appAvailabilities/{id}/relationships/territoryAvailabilities | 


# **app_availabilities_v2_create_instance**
> AppAvailabilityV2Response app_availabilities_v2_create_instance(app_availability_v2_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_availability_v2_create_request import AppAvailabilityV2CreateRequest
from openapi_client.models.app_availability_v2_response import AppAvailabilityV2Response
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
    api_instance = openapi_client.AppAvailabilitiesApi(api_client)
    app_availability_v2_create_request = openapi_client.AppAvailabilityV2CreateRequest() # AppAvailabilityV2CreateRequest | AppAvailability representation

    try:
        api_response = api_instance.app_availabilities_v2_create_instance(app_availability_v2_create_request)
        print("The response of AppAvailabilitiesApi->app_availabilities_v2_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppAvailabilitiesApi->app_availabilities_v2_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **app_availability_v2_create_request** | [**AppAvailabilityV2CreateRequest**](AppAvailabilityV2CreateRequest.md)| AppAvailability representation | 

### Return type

[**AppAvailabilityV2Response**](AppAvailabilityV2Response.md)

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
**201** | Single AppAvailability |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_availabilities_v2_get_instance**
> AppAvailabilityV2Response app_availabilities_v2_get_instance(id, fields_app_availabilities=fields_app_availabilities, fields_territory_availabilities=fields_territory_availabilities, include=include, limit_territory_availabilities=limit_territory_availabilities)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_availability_v2_response import AppAvailabilityV2Response
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
    api_instance = openapi_client.AppAvailabilitiesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_availabilities = ['fields_app_availabilities_example'] # List[str] | the fields to include for returned resources of type appAvailabilities (optional)
    fields_territory_availabilities = ['fields_territory_availabilities_example'] # List[str] | the fields to include for returned resources of type territoryAvailabilities (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_territory_availabilities = 56 # int | maximum number of related territoryAvailabilities returned (when they are included) (optional)

    try:
        api_response = api_instance.app_availabilities_v2_get_instance(id, fields_app_availabilities=fields_app_availabilities, fields_territory_availabilities=fields_territory_availabilities, include=include, limit_territory_availabilities=limit_territory_availabilities)
        print("The response of AppAvailabilitiesApi->app_availabilities_v2_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppAvailabilitiesApi->app_availabilities_v2_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_availabilities** | [**List[str]**](str.md)| the fields to include for returned resources of type appAvailabilities | [optional] 
 **fields_territory_availabilities** | [**List[str]**](str.md)| the fields to include for returned resources of type territoryAvailabilities | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_territory_availabilities** | **int**| maximum number of related territoryAvailabilities returned (when they are included) | [optional] 

### Return type

[**AppAvailabilityV2Response**](AppAvailabilityV2Response.md)

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
**200** | Single AppAvailability |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_availabilities_v2_territory_availabilities_get_to_many_related**
> TerritoryAvailabilitiesResponse app_availabilities_v2_territory_availabilities_get_to_many_related(id, fields_territory_availabilities=fields_territory_availabilities, fields_territories=fields_territories, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.territory_availabilities_response import TerritoryAvailabilitiesResponse
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
    api_instance = openapi_client.AppAvailabilitiesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_territory_availabilities = ['fields_territory_availabilities_example'] # List[str] | the fields to include for returned resources of type territoryAvailabilities (optional)
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.app_availabilities_v2_territory_availabilities_get_to_many_related(id, fields_territory_availabilities=fields_territory_availabilities, fields_territories=fields_territories, limit=limit, include=include)
        print("The response of AppAvailabilitiesApi->app_availabilities_v2_territory_availabilities_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppAvailabilitiesApi->app_availabilities_v2_territory_availabilities_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_territory_availabilities** | [**List[str]**](str.md)| the fields to include for returned resources of type territoryAvailabilities | [optional] 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**TerritoryAvailabilitiesResponse**](TerritoryAvailabilitiesResponse.md)

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
**200** | List of TerritoryAvailabilities |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **app_availabilities_v2_territory_availabilities_get_to_many_relationship**
> AppAvailabilityV2TerritoryAvailabilitiesLinkagesResponse app_availabilities_v2_territory_availabilities_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_availability_v2_territory_availabilities_linkages_response import AppAvailabilityV2TerritoryAvailabilitiesLinkagesResponse
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
    api_instance = openapi_client.AppAvailabilitiesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.app_availabilities_v2_territory_availabilities_get_to_many_relationship(id, limit=limit)
        print("The response of AppAvailabilitiesApi->app_availabilities_v2_territory_availabilities_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AppAvailabilitiesApi->app_availabilities_v2_territory_availabilities_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AppAvailabilityV2TerritoryAvailabilitiesLinkagesResponse**](AppAvailabilityV2TerritoryAvailabilitiesLinkagesResponse.md)

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

