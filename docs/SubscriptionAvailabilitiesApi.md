# openapi_client.SubscriptionAvailabilitiesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**subscription_availabilities_available_territories_get_to_many_related**](SubscriptionAvailabilitiesApi.md#subscription_availabilities_available_territories_get_to_many_related) | **GET** /v1/subscriptionAvailabilities/{id}/availableTerritories | 
[**subscription_availabilities_available_territories_get_to_many_relationship**](SubscriptionAvailabilitiesApi.md#subscription_availabilities_available_territories_get_to_many_relationship) | **GET** /v1/subscriptionAvailabilities/{id}/relationships/availableTerritories | 
[**subscription_availabilities_create_instance**](SubscriptionAvailabilitiesApi.md#subscription_availabilities_create_instance) | **POST** /v1/subscriptionAvailabilities | 
[**subscription_availabilities_get_instance**](SubscriptionAvailabilitiesApi.md#subscription_availabilities_get_instance) | **GET** /v1/subscriptionAvailabilities/{id} | 


# **subscription_availabilities_available_territories_get_to_many_related**
> TerritoriesResponse subscription_availabilities_available_territories_get_to_many_related(id, fields_territories=fields_territories, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.territories_response import TerritoriesResponse
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
    api_instance = openapi_client.SubscriptionAvailabilitiesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.subscription_availabilities_available_territories_get_to_many_related(id, fields_territories=fields_territories, limit=limit)
        print("The response of SubscriptionAvailabilitiesApi->subscription_availabilities_available_territories_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionAvailabilitiesApi->subscription_availabilities_available_territories_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**TerritoriesResponse**](TerritoriesResponse.md)

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
**200** | List of Territories |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_availabilities_available_territories_get_to_many_relationship**
> SubscriptionAvailabilityAvailableTerritoriesLinkagesResponse subscription_availabilities_available_territories_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_availability_available_territories_linkages_response import SubscriptionAvailabilityAvailableTerritoriesLinkagesResponse
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
    api_instance = openapi_client.SubscriptionAvailabilitiesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.subscription_availabilities_available_territories_get_to_many_relationship(id, limit=limit)
        print("The response of SubscriptionAvailabilitiesApi->subscription_availabilities_available_territories_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionAvailabilitiesApi->subscription_availabilities_available_territories_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**SubscriptionAvailabilityAvailableTerritoriesLinkagesResponse**](SubscriptionAvailabilityAvailableTerritoriesLinkagesResponse.md)

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

# **subscription_availabilities_create_instance**
> SubscriptionAvailabilityResponse subscription_availabilities_create_instance(subscription_availability_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_availability_create_request import SubscriptionAvailabilityCreateRequest
from openapi_client.models.subscription_availability_response import SubscriptionAvailabilityResponse
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
    api_instance = openapi_client.SubscriptionAvailabilitiesApi(api_client)
    subscription_availability_create_request = openapi_client.SubscriptionAvailabilityCreateRequest() # SubscriptionAvailabilityCreateRequest | SubscriptionAvailability representation

    try:
        api_response = api_instance.subscription_availabilities_create_instance(subscription_availability_create_request)
        print("The response of SubscriptionAvailabilitiesApi->subscription_availabilities_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionAvailabilitiesApi->subscription_availabilities_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subscription_availability_create_request** | [**SubscriptionAvailabilityCreateRequest**](SubscriptionAvailabilityCreateRequest.md)| SubscriptionAvailability representation | 

### Return type

[**SubscriptionAvailabilityResponse**](SubscriptionAvailabilityResponse.md)

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
**201** | Single SubscriptionAvailability |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscription_availabilities_get_instance**
> SubscriptionAvailabilityResponse subscription_availabilities_get_instance(id, fields_subscription_availabilities=fields_subscription_availabilities, fields_territories=fields_territories, include=include, limit_available_territories=limit_available_territories)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_availability_response import SubscriptionAvailabilityResponse
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
    api_instance = openapi_client.SubscriptionAvailabilitiesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_subscription_availabilities = ['fields_subscription_availabilities_example'] # List[str] | the fields to include for returned resources of type subscriptionAvailabilities (optional)
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_available_territories = 56 # int | maximum number of related availableTerritories returned (when they are included) (optional)

    try:
        api_response = api_instance.subscription_availabilities_get_instance(id, fields_subscription_availabilities=fields_subscription_availabilities, fields_territories=fields_territories, include=include, limit_available_territories=limit_available_territories)
        print("The response of SubscriptionAvailabilitiesApi->subscription_availabilities_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionAvailabilitiesApi->subscription_availabilities_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_subscription_availabilities** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionAvailabilities | [optional] 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_available_territories** | **int**| maximum number of related availableTerritories returned (when they are included) | [optional] 

### Return type

[**SubscriptionAvailabilityResponse**](SubscriptionAvailabilityResponse.md)

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
**200** | Single SubscriptionAvailability |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

