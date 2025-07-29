# openapi_client.WebhooksApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**webhooks_create_instance**](WebhooksApi.md#webhooks_create_instance) | **POST** /v1/webhooks | 
[**webhooks_delete_instance**](WebhooksApi.md#webhooks_delete_instance) | **DELETE** /v1/webhooks/{id} | 
[**webhooks_deliveries_get_to_many_related**](WebhooksApi.md#webhooks_deliveries_get_to_many_related) | **GET** /v1/webhooks/{id}/deliveries | 
[**webhooks_deliveries_get_to_many_relationship**](WebhooksApi.md#webhooks_deliveries_get_to_many_relationship) | **GET** /v1/webhooks/{id}/relationships/deliveries | 
[**webhooks_get_instance**](WebhooksApi.md#webhooks_get_instance) | **GET** /v1/webhooks/{id} | 
[**webhooks_update_instance**](WebhooksApi.md#webhooks_update_instance) | **PATCH** /v1/webhooks/{id} | 


# **webhooks_create_instance**
> WebhookResponse webhooks_create_instance(webhook_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.webhook_create_request import WebhookCreateRequest
from openapi_client.models.webhook_response import WebhookResponse
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
    api_instance = openapi_client.WebhooksApi(api_client)
    webhook_create_request = openapi_client.WebhookCreateRequest() # WebhookCreateRequest | Webhook representation

    try:
        api_response = api_instance.webhooks_create_instance(webhook_create_request)
        print("The response of WebhooksApi->webhooks_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->webhooks_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **webhook_create_request** | [**WebhookCreateRequest**](WebhookCreateRequest.md)| Webhook representation | 

### Return type

[**WebhookResponse**](WebhookResponse.md)

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
**201** | Single Webhook |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **webhooks_delete_instance**
> webhooks_delete_instance(id)

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
    api_instance = openapi_client.WebhooksApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.webhooks_delete_instance(id)
    except Exception as e:
        print("Exception when calling WebhooksApi->webhooks_delete_instance: %s\n" % e)
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

# **webhooks_deliveries_get_to_many_related**
> WebhookDeliveriesResponse webhooks_deliveries_get_to_many_related(id, filter_delivery_state=filter_delivery_state, filter_created_date_greater_than_or_equal_to=filter_created_date_greater_than_or_equal_to, filter_created_date_less_than=filter_created_date_less_than, fields_webhook_deliveries=fields_webhook_deliveries, fields_webhook_events=fields_webhook_events, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.webhook_deliveries_response import WebhookDeliveriesResponse
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
    api_instance = openapi_client.WebhooksApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_delivery_state = ['filter_delivery_state_example'] # List[str] | filter by attribute 'deliveryState' (optional)
    filter_created_date_greater_than_or_equal_to = ['filter_created_date_greater_than_or_equal_to_example'] # List[str] | filter by createdDateGreaterThanOrEqualTo (optional)
    filter_created_date_less_than = ['filter_created_date_less_than_example'] # List[str] | filter by createdDateLessThan (optional)
    fields_webhook_deliveries = ['fields_webhook_deliveries_example'] # List[str] | the fields to include for returned resources of type webhookDeliveries (optional)
    fields_webhook_events = ['fields_webhook_events_example'] # List[str] | the fields to include for returned resources of type webhookEvents (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.webhooks_deliveries_get_to_many_related(id, filter_delivery_state=filter_delivery_state, filter_created_date_greater_than_or_equal_to=filter_created_date_greater_than_or_equal_to, filter_created_date_less_than=filter_created_date_less_than, fields_webhook_deliveries=fields_webhook_deliveries, fields_webhook_events=fields_webhook_events, limit=limit, include=include)
        print("The response of WebhooksApi->webhooks_deliveries_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->webhooks_deliveries_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_delivery_state** | [**List[str]**](str.md)| filter by attribute &#39;deliveryState&#39; | [optional] 
 **filter_created_date_greater_than_or_equal_to** | [**List[str]**](str.md)| filter by createdDateGreaterThanOrEqualTo | [optional] 
 **filter_created_date_less_than** | [**List[str]**](str.md)| filter by createdDateLessThan | [optional] 
 **fields_webhook_deliveries** | [**List[str]**](str.md)| the fields to include for returned resources of type webhookDeliveries | [optional] 
 **fields_webhook_events** | [**List[str]**](str.md)| the fields to include for returned resources of type webhookEvents | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**WebhookDeliveriesResponse**](WebhookDeliveriesResponse.md)

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
**200** | List of WebhookDeliveries |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **webhooks_deliveries_get_to_many_relationship**
> WebhookDeliveriesLinkagesResponse webhooks_deliveries_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.webhook_deliveries_linkages_response import WebhookDeliveriesLinkagesResponse
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
    api_instance = openapi_client.WebhooksApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.webhooks_deliveries_get_to_many_relationship(id, limit=limit)
        print("The response of WebhooksApi->webhooks_deliveries_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->webhooks_deliveries_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**WebhookDeliveriesLinkagesResponse**](WebhookDeliveriesLinkagesResponse.md)

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

# **webhooks_get_instance**
> WebhookResponse webhooks_get_instance(id, fields_webhooks=fields_webhooks, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.webhook_response import WebhookResponse
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
    api_instance = openapi_client.WebhooksApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_webhooks = ['fields_webhooks_example'] # List[str] | the fields to include for returned resources of type webhooks (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.webhooks_get_instance(id, fields_webhooks=fields_webhooks, include=include)
        print("The response of WebhooksApi->webhooks_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->webhooks_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_webhooks** | [**List[str]**](str.md)| the fields to include for returned resources of type webhooks | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**WebhookResponse**](WebhookResponse.md)

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
**200** | Single Webhook |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **webhooks_update_instance**
> WebhookResponse webhooks_update_instance(id, webhook_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.webhook_response import WebhookResponse
from openapi_client.models.webhook_update_request import WebhookUpdateRequest
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
    api_instance = openapi_client.WebhooksApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    webhook_update_request = openapi_client.WebhookUpdateRequest() # WebhookUpdateRequest | Webhook representation

    try:
        api_response = api_instance.webhooks_update_instance(id, webhook_update_request)
        print("The response of WebhooksApi->webhooks_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->webhooks_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **webhook_update_request** | [**WebhookUpdateRequest**](WebhookUpdateRequest.md)| Webhook representation | 

### Return type

[**WebhookResponse**](WebhookResponse.md)

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
**200** | Single Webhook |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

