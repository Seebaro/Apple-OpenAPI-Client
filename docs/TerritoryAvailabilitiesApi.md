# openapi_client.TerritoryAvailabilitiesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**territory_availabilities_update_instance**](TerritoryAvailabilitiesApi.md#territory_availabilities_update_instance) | **PATCH** /v1/territoryAvailabilities/{id} | 


# **territory_availabilities_update_instance**
> TerritoryAvailabilityResponse territory_availabilities_update_instance(id, territory_availability_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.territory_availability_response import TerritoryAvailabilityResponse
from openapi_client.models.territory_availability_update_request import TerritoryAvailabilityUpdateRequest
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
    api_instance = openapi_client.TerritoryAvailabilitiesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    territory_availability_update_request = openapi_client.TerritoryAvailabilityUpdateRequest() # TerritoryAvailabilityUpdateRequest | TerritoryAvailability representation

    try:
        api_response = api_instance.territory_availabilities_update_instance(id, territory_availability_update_request)
        print("The response of TerritoryAvailabilitiesApi->territory_availabilities_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TerritoryAvailabilitiesApi->territory_availabilities_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **territory_availability_update_request** | [**TerritoryAvailabilityUpdateRequest**](TerritoryAvailabilityUpdateRequest.md)| TerritoryAvailability representation | 

### Return type

[**TerritoryAvailabilityResponse**](TerritoryAvailabilityResponse.md)

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
**200** | Single TerritoryAvailability |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

