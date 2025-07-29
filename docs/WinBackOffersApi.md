# openapi_client.WinBackOffersApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**win_back_offers_create_instance**](WinBackOffersApi.md#win_back_offers_create_instance) | **POST** /v1/winBackOffers | 
[**win_back_offers_delete_instance**](WinBackOffersApi.md#win_back_offers_delete_instance) | **DELETE** /v1/winBackOffers/{id} | 
[**win_back_offers_get_instance**](WinBackOffersApi.md#win_back_offers_get_instance) | **GET** /v1/winBackOffers/{id} | 
[**win_back_offers_prices_get_to_many_related**](WinBackOffersApi.md#win_back_offers_prices_get_to_many_related) | **GET** /v1/winBackOffers/{id}/prices | 
[**win_back_offers_prices_get_to_many_relationship**](WinBackOffersApi.md#win_back_offers_prices_get_to_many_relationship) | **GET** /v1/winBackOffers/{id}/relationships/prices | 
[**win_back_offers_update_instance**](WinBackOffersApi.md#win_back_offers_update_instance) | **PATCH** /v1/winBackOffers/{id} | 


# **win_back_offers_create_instance**
> WinBackOfferResponse win_back_offers_create_instance(win_back_offer_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.win_back_offer_create_request import WinBackOfferCreateRequest
from openapi_client.models.win_back_offer_response import WinBackOfferResponse
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
    api_instance = openapi_client.WinBackOffersApi(api_client)
    win_back_offer_create_request = openapi_client.WinBackOfferCreateRequest() # WinBackOfferCreateRequest | WinBackOffer representation

    try:
        api_response = api_instance.win_back_offers_create_instance(win_back_offer_create_request)
        print("The response of WinBackOffersApi->win_back_offers_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WinBackOffersApi->win_back_offers_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **win_back_offer_create_request** | [**WinBackOfferCreateRequest**](WinBackOfferCreateRequest.md)| WinBackOffer representation | 

### Return type

[**WinBackOfferResponse**](WinBackOfferResponse.md)

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
**201** | Single WinBackOffer |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **win_back_offers_delete_instance**
> win_back_offers_delete_instance(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
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
    api_instance = openapi_client.WinBackOffersApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.win_back_offers_delete_instance(id)
    except Exception as e:
        print("Exception when calling WinBackOffersApi->win_back_offers_delete_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

void (empty response body)

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
**409** | Request entity error(s) |  -  |
**204** | Success (no content) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **win_back_offers_get_instance**
> WinBackOfferResponse win_back_offers_get_instance(id, fields_win_back_offers=fields_win_back_offers, fields_win_back_offer_prices=fields_win_back_offer_prices, include=include, limit_prices=limit_prices)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.win_back_offer_response import WinBackOfferResponse
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
    api_instance = openapi_client.WinBackOffersApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_win_back_offers = ['fields_win_back_offers_example'] # List[str] | the fields to include for returned resources of type winBackOffers (optional)
    fields_win_back_offer_prices = ['fields_win_back_offer_prices_example'] # List[str] | the fields to include for returned resources of type winBackOfferPrices (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_prices = 56 # int | maximum number of related prices returned (when they are included) (optional)

    try:
        api_response = api_instance.win_back_offers_get_instance(id, fields_win_back_offers=fields_win_back_offers, fields_win_back_offer_prices=fields_win_back_offer_prices, include=include, limit_prices=limit_prices)
        print("The response of WinBackOffersApi->win_back_offers_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WinBackOffersApi->win_back_offers_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_win_back_offers** | [**List[str]**](str.md)| the fields to include for returned resources of type winBackOffers | [optional] 
 **fields_win_back_offer_prices** | [**List[str]**](str.md)| the fields to include for returned resources of type winBackOfferPrices | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_prices** | **int**| maximum number of related prices returned (when they are included) | [optional] 

### Return type

[**WinBackOfferResponse**](WinBackOfferResponse.md)

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
**200** | Single WinBackOffer |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **win_back_offers_prices_get_to_many_related**
> WinBackOfferPricesResponse win_back_offers_prices_get_to_many_related(id, filter_territory=filter_territory, fields_win_back_offer_prices=fields_win_back_offer_prices, fields_territories=fields_territories, fields_subscription_price_points=fields_subscription_price_points, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.win_back_offer_prices_response import WinBackOfferPricesResponse
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
    api_instance = openapi_client.WinBackOffersApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_territory = ['filter_territory_example'] # List[str] | filter by id(s) of related 'territory' (optional)
    fields_win_back_offer_prices = ['fields_win_back_offer_prices_example'] # List[str] | the fields to include for returned resources of type winBackOfferPrices (optional)
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)
    fields_subscription_price_points = ['fields_subscription_price_points_example'] # List[str] | the fields to include for returned resources of type subscriptionPricePoints (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.win_back_offers_prices_get_to_many_related(id, filter_territory=filter_territory, fields_win_back_offer_prices=fields_win_back_offer_prices, fields_territories=fields_territories, fields_subscription_price_points=fields_subscription_price_points, limit=limit, include=include)
        print("The response of WinBackOffersApi->win_back_offers_prices_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WinBackOffersApi->win_back_offers_prices_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_territory** | [**List[str]**](str.md)| filter by id(s) of related &#39;territory&#39; | [optional] 
 **fields_win_back_offer_prices** | [**List[str]**](str.md)| the fields to include for returned resources of type winBackOfferPrices | [optional] 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 
 **fields_subscription_price_points** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionPricePoints | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**WinBackOfferPricesResponse**](WinBackOfferPricesResponse.md)

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
**200** | List of WinBackOfferPrices |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **win_back_offers_prices_get_to_many_relationship**
> WinBackOfferPricesLinkagesResponse win_back_offers_prices_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.win_back_offer_prices_linkages_response import WinBackOfferPricesLinkagesResponse
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
    api_instance = openapi_client.WinBackOffersApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.win_back_offers_prices_get_to_many_relationship(id, limit=limit)
        print("The response of WinBackOffersApi->win_back_offers_prices_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WinBackOffersApi->win_back_offers_prices_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**WinBackOfferPricesLinkagesResponse**](WinBackOfferPricesLinkagesResponse.md)

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

# **win_back_offers_update_instance**
> WinBackOfferResponse win_back_offers_update_instance(id, win_back_offer_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.win_back_offer_response import WinBackOfferResponse
from openapi_client.models.win_back_offer_update_request import WinBackOfferUpdateRequest
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
    api_instance = openapi_client.WinBackOffersApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    win_back_offer_update_request = openapi_client.WinBackOfferUpdateRequest() # WinBackOfferUpdateRequest | WinBackOffer representation

    try:
        api_response = api_instance.win_back_offers_update_instance(id, win_back_offer_update_request)
        print("The response of WinBackOffersApi->win_back_offers_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WinBackOffersApi->win_back_offers_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **win_back_offer_update_request** | [**WinBackOfferUpdateRequest**](WinBackOfferUpdateRequest.md)| WinBackOffer representation | 

### Return type

[**WinBackOfferResponse**](WinBackOfferResponse.md)

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
**200** | Single WinBackOffer |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

