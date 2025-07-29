# openapi_client.ScmGitReferencesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**scm_git_references_get_instance**](ScmGitReferencesApi.md#scm_git_references_get_instance) | **GET** /v1/scmGitReferences/{id} | 


# **scm_git_references_get_instance**
> ScmGitReferenceResponse scm_git_references_get_instance(id, fields_scm_git_references=fields_scm_git_references, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.scm_git_reference_response import ScmGitReferenceResponse
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
    api_instance = openapi_client.ScmGitReferencesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_scm_git_references = ['fields_scm_git_references_example'] # List[str] | the fields to include for returned resources of type scmGitReferences (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.scm_git_references_get_instance(id, fields_scm_git_references=fields_scm_git_references, include=include)
        print("The response of ScmGitReferencesApi->scm_git_references_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ScmGitReferencesApi->scm_git_references_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_scm_git_references** | [**List[str]**](str.md)| the fields to include for returned resources of type scmGitReferences | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**ScmGitReferenceResponse**](ScmGitReferenceResponse.md)

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
**200** | Single ScmGitReference |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

