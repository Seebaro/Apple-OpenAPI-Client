# openapi_client.WebhookPingsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**webhook_pings_create_instance**](WebhookPingsApi.md#webhook_pings_create_instance) | **POST** /v1/webhookPings | 


# **webhook_pings_create_instance**
> WebhookPingResponse webhook_pings_create_instance(webhook_ping_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.webhook_ping_create_request import WebhookPingCreateRequest
from openapi_client.models.webhook_ping_response import WebhookPingResponse
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
    api_instance = openapi_client.WebhookPingsApi(api_client)
    webhook_ping_create_request = openapi_client.WebhookPingCreateRequest() # WebhookPingCreateRequest | WebhookPing representation

    try:
        api_response = api_instance.webhook_pings_create_instance(webhook_ping_create_request)
        print("The response of WebhookPingsApi->webhook_pings_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhookPingsApi->webhook_pings_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **webhook_ping_create_request** | [**WebhookPingCreateRequest**](WebhookPingCreateRequest.md)| WebhookPing representation | 

### Return type

[**WebhookPingResponse**](WebhookPingResponse.md)

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
**201** | Single WebhookPing |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

