# openapi_client.MarketplaceWebhooksApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**marketplace_webhooks_create_instance**](MarketplaceWebhooksApi.md#marketplace_webhooks_create_instance) | **POST** /v1/marketplaceWebhooks | 
[**marketplace_webhooks_delete_instance**](MarketplaceWebhooksApi.md#marketplace_webhooks_delete_instance) | **DELETE** /v1/marketplaceWebhooks/{id} | 
[**marketplace_webhooks_get_collection**](MarketplaceWebhooksApi.md#marketplace_webhooks_get_collection) | **GET** /v1/marketplaceWebhooks | 
[**marketplace_webhooks_update_instance**](MarketplaceWebhooksApi.md#marketplace_webhooks_update_instance) | **PATCH** /v1/marketplaceWebhooks/{id} | 


# **marketplace_webhooks_create_instance**
> MarketplaceWebhookResponse marketplace_webhooks_create_instance(marketplace_webhook_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.marketplace_webhook_create_request import MarketplaceWebhookCreateRequest
from openapi_client.models.marketplace_webhook_response import MarketplaceWebhookResponse
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
    api_instance = openapi_client.MarketplaceWebhooksApi(api_client)
    marketplace_webhook_create_request = openapi_client.MarketplaceWebhookCreateRequest() # MarketplaceWebhookCreateRequest | MarketplaceWebhook representation

    try:
        api_response = api_instance.marketplace_webhooks_create_instance(marketplace_webhook_create_request)
        print("The response of MarketplaceWebhooksApi->marketplace_webhooks_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MarketplaceWebhooksApi->marketplace_webhooks_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **marketplace_webhook_create_request** | [**MarketplaceWebhookCreateRequest**](MarketplaceWebhookCreateRequest.md)| MarketplaceWebhook representation | 

### Return type

[**MarketplaceWebhookResponse**](MarketplaceWebhookResponse.md)

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
**201** | Single MarketplaceWebhook |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **marketplace_webhooks_delete_instance**
> marketplace_webhooks_delete_instance(id)

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
    api_instance = openapi_client.MarketplaceWebhooksApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.marketplace_webhooks_delete_instance(id)
    except Exception as e:
        print("Exception when calling MarketplaceWebhooksApi->marketplace_webhooks_delete_instance: %s\n" % e)
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

# **marketplace_webhooks_get_collection**
> MarketplaceWebhooksResponse marketplace_webhooks_get_collection(fields_marketplace_webhooks=fields_marketplace_webhooks, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.marketplace_webhooks_response import MarketplaceWebhooksResponse
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
    api_instance = openapi_client.MarketplaceWebhooksApi(api_client)
    fields_marketplace_webhooks = ['fields_marketplace_webhooks_example'] # List[str] | the fields to include for returned resources of type marketplaceWebhooks (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.marketplace_webhooks_get_collection(fields_marketplace_webhooks=fields_marketplace_webhooks, limit=limit)
        print("The response of MarketplaceWebhooksApi->marketplace_webhooks_get_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MarketplaceWebhooksApi->marketplace_webhooks_get_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fields_marketplace_webhooks** | [**List[str]**](str.md)| the fields to include for returned resources of type marketplaceWebhooks | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**MarketplaceWebhooksResponse**](MarketplaceWebhooksResponse.md)

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
**200** | List of MarketplaceWebhooks |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **marketplace_webhooks_update_instance**
> MarketplaceWebhookResponse marketplace_webhooks_update_instance(id, marketplace_webhook_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.marketplace_webhook_response import MarketplaceWebhookResponse
from openapi_client.models.marketplace_webhook_update_request import MarketplaceWebhookUpdateRequest
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
    api_instance = openapi_client.MarketplaceWebhooksApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    marketplace_webhook_update_request = openapi_client.MarketplaceWebhookUpdateRequest() # MarketplaceWebhookUpdateRequest | MarketplaceWebhook representation

    try:
        api_response = api_instance.marketplace_webhooks_update_instance(id, marketplace_webhook_update_request)
        print("The response of MarketplaceWebhooksApi->marketplace_webhooks_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MarketplaceWebhooksApi->marketplace_webhooks_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **marketplace_webhook_update_request** | [**MarketplaceWebhookUpdateRequest**](MarketplaceWebhookUpdateRequest.md)| MarketplaceWebhook representation | 

### Return type

[**MarketplaceWebhookResponse**](MarketplaceWebhookResponse.md)

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
**200** | Single MarketplaceWebhook |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

