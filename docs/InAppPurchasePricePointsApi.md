# openapi_client.InAppPurchasePricePointsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**in_app_purchase_price_points_equalizations_get_to_many_related**](InAppPurchasePricePointsApi.md#in_app_purchase_price_points_equalizations_get_to_many_related) | **GET** /v1/inAppPurchasePricePoints/{id}/equalizations | 
[**in_app_purchase_price_points_equalizations_get_to_many_relationship**](InAppPurchasePricePointsApi.md#in_app_purchase_price_points_equalizations_get_to_many_relationship) | **GET** /v1/inAppPurchasePricePoints/{id}/relationships/equalizations | 


# **in_app_purchase_price_points_equalizations_get_to_many_related**
> InAppPurchasePricePointsResponse in_app_purchase_price_points_equalizations_get_to_many_related(id, filter_territory=filter_territory, filter_in_app_purchase_v2=filter_in_app_purchase_v2, fields_in_app_purchase_price_points=fields_in_app_purchase_price_points, fields_territories=fields_territories, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_price_points_response import InAppPurchasePricePointsResponse
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
    api_instance = openapi_client.InAppPurchasePricePointsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_territory = ['filter_territory_example'] # List[str] | filter by id(s) of related 'territory' (optional)
    filter_in_app_purchase_v2 = ['filter_in_app_purchase_v2_example'] # List[str] | filter by id(s) of related 'inAppPurchaseV2' (optional)
    fields_in_app_purchase_price_points = ['fields_in_app_purchase_price_points_example'] # List[str] | the fields to include for returned resources of type inAppPurchasePricePoints (optional)
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.in_app_purchase_price_points_equalizations_get_to_many_related(id, filter_territory=filter_territory, filter_in_app_purchase_v2=filter_in_app_purchase_v2, fields_in_app_purchase_price_points=fields_in_app_purchase_price_points, fields_territories=fields_territories, limit=limit, include=include)
        print("The response of InAppPurchasePricePointsApi->in_app_purchase_price_points_equalizations_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasePricePointsApi->in_app_purchase_price_points_equalizations_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_territory** | [**List[str]**](str.md)| filter by id(s) of related &#39;territory&#39; | [optional] 
 **filter_in_app_purchase_v2** | [**List[str]**](str.md)| filter by id(s) of related &#39;inAppPurchaseV2&#39; | [optional] 
 **fields_in_app_purchase_price_points** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchasePricePoints | [optional] 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**InAppPurchasePricePointsResponse**](InAppPurchasePricePointsResponse.md)

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
**200** | List of InAppPurchasePricePoints |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchase_price_points_equalizations_get_to_many_relationship**
> InAppPurchasePricePointEqualizationsLinkagesResponse in_app_purchase_price_points_equalizations_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_price_point_equalizations_linkages_response import InAppPurchasePricePointEqualizationsLinkagesResponse
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
    api_instance = openapi_client.InAppPurchasePricePointsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.in_app_purchase_price_points_equalizations_get_to_many_relationship(id, limit=limit)
        print("The response of InAppPurchasePricePointsApi->in_app_purchase_price_points_equalizations_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasePricePointsApi->in_app_purchase_price_points_equalizations_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**InAppPurchasePricePointEqualizationsLinkagesResponse**](InAppPurchasePricePointEqualizationsLinkagesResponse.md)

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

