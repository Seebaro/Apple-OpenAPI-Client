# openapi_client.SandboxTestersClearPurchaseHistoryRequestApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**sandbox_testers_clear_purchase_history_request_v2_create_instance**](SandboxTestersClearPurchaseHistoryRequestApi.md#sandbox_testers_clear_purchase_history_request_v2_create_instance) | **POST** /v2/sandboxTestersClearPurchaseHistoryRequest | 


# **sandbox_testers_clear_purchase_history_request_v2_create_instance**
> SandboxTestersClearPurchaseHistoryRequestV2Response sandbox_testers_clear_purchase_history_request_v2_create_instance(sandbox_testers_clear_purchase_history_request_v2_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.sandbox_testers_clear_purchase_history_request_v2_create_request import SandboxTestersClearPurchaseHistoryRequestV2CreateRequest
from openapi_client.models.sandbox_testers_clear_purchase_history_request_v2_response import SandboxTestersClearPurchaseHistoryRequestV2Response
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
    api_instance = openapi_client.SandboxTestersClearPurchaseHistoryRequestApi(api_client)
    sandbox_testers_clear_purchase_history_request_v2_create_request = openapi_client.SandboxTestersClearPurchaseHistoryRequestV2CreateRequest() # SandboxTestersClearPurchaseHistoryRequestV2CreateRequest | SandboxTestersClearPurchaseHistoryRequest representation

    try:
        api_response = api_instance.sandbox_testers_clear_purchase_history_request_v2_create_instance(sandbox_testers_clear_purchase_history_request_v2_create_request)
        print("The response of SandboxTestersClearPurchaseHistoryRequestApi->sandbox_testers_clear_purchase_history_request_v2_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SandboxTestersClearPurchaseHistoryRequestApi->sandbox_testers_clear_purchase_history_request_v2_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sandbox_testers_clear_purchase_history_request_v2_create_request** | [**SandboxTestersClearPurchaseHistoryRequestV2CreateRequest**](SandboxTestersClearPurchaseHistoryRequestV2CreateRequest.md)| SandboxTestersClearPurchaseHistoryRequest representation | 

### Return type

[**SandboxTestersClearPurchaseHistoryRequestV2Response**](SandboxTestersClearPurchaseHistoryRequestV2Response.md)

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
**201** | Single SandboxTestersClearPurchaseHistoryRequest |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

