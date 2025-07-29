# openapi_client.CiIssuesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ci_issues_get_instance**](CiIssuesApi.md#ci_issues_get_instance) | **GET** /v1/ciIssues/{id} | 


# **ci_issues_get_instance**
> CiIssueResponse ci_issues_get_instance(id, fields_ci_issues=fields_ci_issues)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_issue_response import CiIssueResponse
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
    api_instance = openapi_client.CiIssuesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_ci_issues = ['fields_ci_issues_example'] # List[str] | the fields to include for returned resources of type ciIssues (optional)

    try:
        api_response = api_instance.ci_issues_get_instance(id, fields_ci_issues=fields_ci_issues)
        print("The response of CiIssuesApi->ci_issues_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiIssuesApi->ci_issues_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_ci_issues** | [**List[str]**](str.md)| the fields to include for returned resources of type ciIssues | [optional] 

### Return type

[**CiIssueResponse**](CiIssueResponse.md)

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
**200** | Single CiIssue |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

