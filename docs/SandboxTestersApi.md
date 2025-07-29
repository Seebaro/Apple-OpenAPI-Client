# openapi_client.SandboxTestersApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**sandbox_testers_v2_get_collection**](SandboxTestersApi.md#sandbox_testers_v2_get_collection) | **GET** /v2/sandboxTesters | 
[**sandbox_testers_v2_update_instance**](SandboxTestersApi.md#sandbox_testers_v2_update_instance) | **PATCH** /v2/sandboxTesters/{id} | 


# **sandbox_testers_v2_get_collection**
> SandboxTestersV2Response sandbox_testers_v2_get_collection(fields_sandbox_testers=fields_sandbox_testers, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.sandbox_testers_v2_response import SandboxTestersV2Response
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
    api_instance = openapi_client.SandboxTestersApi(api_client)
    fields_sandbox_testers = ['fields_sandbox_testers_example'] # List[str] | the fields to include for returned resources of type sandboxTesters (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.sandbox_testers_v2_get_collection(fields_sandbox_testers=fields_sandbox_testers, limit=limit)
        print("The response of SandboxTestersApi->sandbox_testers_v2_get_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SandboxTestersApi->sandbox_testers_v2_get_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fields_sandbox_testers** | [**List[str]**](str.md)| the fields to include for returned resources of type sandboxTesters | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**SandboxTestersV2Response**](SandboxTestersV2Response.md)

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
**200** | List of SandboxTesters |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **sandbox_testers_v2_update_instance**
> SandboxTesterV2Response sandbox_testers_v2_update_instance(id, sandbox_tester_v2_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.sandbox_tester_v2_response import SandboxTesterV2Response
from openapi_client.models.sandbox_tester_v2_update_request import SandboxTesterV2UpdateRequest
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
    api_instance = openapi_client.SandboxTestersApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    sandbox_tester_v2_update_request = openapi_client.SandboxTesterV2UpdateRequest() # SandboxTesterV2UpdateRequest | SandboxTester representation

    try:
        api_response = api_instance.sandbox_testers_v2_update_instance(id, sandbox_tester_v2_update_request)
        print("The response of SandboxTestersApi->sandbox_testers_v2_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SandboxTestersApi->sandbox_testers_v2_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **sandbox_tester_v2_update_request** | [**SandboxTesterV2UpdateRequest**](SandboxTesterV2UpdateRequest.md)| SandboxTester representation | 

### Return type

[**SandboxTesterV2Response**](SandboxTesterV2Response.md)

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
**200** | Single SandboxTester |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

