# openapi_client.CiArtifactsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ci_artifacts_get_instance**](CiArtifactsApi.md#ci_artifacts_get_instance) | **GET** /v1/ciArtifacts/{id} | 


# **ci_artifacts_get_instance**
> CiArtifactResponse ci_artifacts_get_instance(id, fields_ci_artifacts=fields_ci_artifacts)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_artifact_response import CiArtifactResponse
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
    api_instance = openapi_client.CiArtifactsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_ci_artifacts = ['fields_ci_artifacts_example'] # List[str] | the fields to include for returned resources of type ciArtifacts (optional)

    try:
        api_response = api_instance.ci_artifacts_get_instance(id, fields_ci_artifacts=fields_ci_artifacts)
        print("The response of CiArtifactsApi->ci_artifacts_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiArtifactsApi->ci_artifacts_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_ci_artifacts** | [**List[str]**](str.md)| the fields to include for returned resources of type ciArtifacts | [optional] 

### Return type

[**CiArtifactResponse**](CiArtifactResponse.md)

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
**200** | Single CiArtifact |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

