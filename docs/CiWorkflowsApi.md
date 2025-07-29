# openapi_client.CiWorkflowsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ci_workflows_build_runs_get_to_many_related**](CiWorkflowsApi.md#ci_workflows_build_runs_get_to_many_related) | **GET** /v1/ciWorkflows/{id}/buildRuns | 
[**ci_workflows_build_runs_get_to_many_relationship**](CiWorkflowsApi.md#ci_workflows_build_runs_get_to_many_relationship) | **GET** /v1/ciWorkflows/{id}/relationships/buildRuns | 
[**ci_workflows_create_instance**](CiWorkflowsApi.md#ci_workflows_create_instance) | **POST** /v1/ciWorkflows | 
[**ci_workflows_delete_instance**](CiWorkflowsApi.md#ci_workflows_delete_instance) | **DELETE** /v1/ciWorkflows/{id} | 
[**ci_workflows_get_instance**](CiWorkflowsApi.md#ci_workflows_get_instance) | **GET** /v1/ciWorkflows/{id} | 
[**ci_workflows_repository_get_to_one_related**](CiWorkflowsApi.md#ci_workflows_repository_get_to_one_related) | **GET** /v1/ciWorkflows/{id}/repository | 
[**ci_workflows_repository_get_to_one_relationship**](CiWorkflowsApi.md#ci_workflows_repository_get_to_one_relationship) | **GET** /v1/ciWorkflows/{id}/relationships/repository | 
[**ci_workflows_update_instance**](CiWorkflowsApi.md#ci_workflows_update_instance) | **PATCH** /v1/ciWorkflows/{id} | 


# **ci_workflows_build_runs_get_to_many_related**
> CiBuildRunsResponse ci_workflows_build_runs_get_to_many_related(id, filter_builds=filter_builds, sort=sort, fields_ci_build_runs=fields_ci_build_runs, fields_builds=fields_builds, fields_ci_workflows=fields_ci_workflows, fields_ci_products=fields_ci_products, fields_scm_git_references=fields_scm_git_references, fields_scm_pull_requests=fields_scm_pull_requests, limit=limit, include=include, limit_builds=limit_builds)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_build_runs_response import CiBuildRunsResponse
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
    api_instance = openapi_client.CiWorkflowsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_builds = ['filter_builds_example'] # List[str] | filter by id(s) of related 'builds' (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; resources will be sorted as specified (optional)
    fields_ci_build_runs = ['fields_ci_build_runs_example'] # List[str] | the fields to include for returned resources of type ciBuildRuns (optional)
    fields_builds = ['fields_builds_example'] # List[str] | the fields to include for returned resources of type builds (optional)
    fields_ci_workflows = ['fields_ci_workflows_example'] # List[str] | the fields to include for returned resources of type ciWorkflows (optional)
    fields_ci_products = ['fields_ci_products_example'] # List[str] | the fields to include for returned resources of type ciProducts (optional)
    fields_scm_git_references = ['fields_scm_git_references_example'] # List[str] | the fields to include for returned resources of type scmGitReferences (optional)
    fields_scm_pull_requests = ['fields_scm_pull_requests_example'] # List[str] | the fields to include for returned resources of type scmPullRequests (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_builds = 56 # int | maximum number of related builds returned (when they are included) (optional)

    try:
        api_response = api_instance.ci_workflows_build_runs_get_to_many_related(id, filter_builds=filter_builds, sort=sort, fields_ci_build_runs=fields_ci_build_runs, fields_builds=fields_builds, fields_ci_workflows=fields_ci_workflows, fields_ci_products=fields_ci_products, fields_scm_git_references=fields_scm_git_references, fields_scm_pull_requests=fields_scm_pull_requests, limit=limit, include=include, limit_builds=limit_builds)
        print("The response of CiWorkflowsApi->ci_workflows_build_runs_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiWorkflowsApi->ci_workflows_build_runs_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_builds** | [**List[str]**](str.md)| filter by id(s) of related &#39;builds&#39; | [optional] 
 **sort** | [**List[str]**](str.md)| comma-separated list of sort expressions; resources will be sorted as specified | [optional] 
 **fields_ci_build_runs** | [**List[str]**](str.md)| the fields to include for returned resources of type ciBuildRuns | [optional] 
 **fields_builds** | [**List[str]**](str.md)| the fields to include for returned resources of type builds | [optional] 
 **fields_ci_workflows** | [**List[str]**](str.md)| the fields to include for returned resources of type ciWorkflows | [optional] 
 **fields_ci_products** | [**List[str]**](str.md)| the fields to include for returned resources of type ciProducts | [optional] 
 **fields_scm_git_references** | [**List[str]**](str.md)| the fields to include for returned resources of type scmGitReferences | [optional] 
 **fields_scm_pull_requests** | [**List[str]**](str.md)| the fields to include for returned resources of type scmPullRequests | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_builds** | **int**| maximum number of related builds returned (when they are included) | [optional] 

### Return type

[**CiBuildRunsResponse**](CiBuildRunsResponse.md)

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
**200** | List of CiBuildRuns |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_workflows_build_runs_get_to_many_relationship**
> CiWorkflowBuildRunsLinkagesResponse ci_workflows_build_runs_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_workflow_build_runs_linkages_response import CiWorkflowBuildRunsLinkagesResponse
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
    api_instance = openapi_client.CiWorkflowsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.ci_workflows_build_runs_get_to_many_relationship(id, limit=limit)
        print("The response of CiWorkflowsApi->ci_workflows_build_runs_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiWorkflowsApi->ci_workflows_build_runs_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**CiWorkflowBuildRunsLinkagesResponse**](CiWorkflowBuildRunsLinkagesResponse.md)

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

# **ci_workflows_create_instance**
> CiWorkflowResponse ci_workflows_create_instance(ci_workflow_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_workflow_create_request import CiWorkflowCreateRequest
from openapi_client.models.ci_workflow_response import CiWorkflowResponse
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
    api_instance = openapi_client.CiWorkflowsApi(api_client)
    ci_workflow_create_request = openapi_client.CiWorkflowCreateRequest() # CiWorkflowCreateRequest | CiWorkflow representation

    try:
        api_response = api_instance.ci_workflows_create_instance(ci_workflow_create_request)
        print("The response of CiWorkflowsApi->ci_workflows_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiWorkflowsApi->ci_workflows_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ci_workflow_create_request** | [**CiWorkflowCreateRequest**](CiWorkflowCreateRequest.md)| CiWorkflow representation | 

### Return type

[**CiWorkflowResponse**](CiWorkflowResponse.md)

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
**201** | Single CiWorkflow |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_workflows_delete_instance**
> ci_workflows_delete_instance(id)

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
    api_instance = openapi_client.CiWorkflowsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.ci_workflows_delete_instance(id)
    except Exception as e:
        print("Exception when calling CiWorkflowsApi->ci_workflows_delete_instance: %s\n" % e)
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

# **ci_workflows_get_instance**
> CiWorkflowResponse ci_workflows_get_instance(id, fields_ci_workflows=fields_ci_workflows, fields_scm_repositories=fields_scm_repositories, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_workflow_response import CiWorkflowResponse
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
    api_instance = openapi_client.CiWorkflowsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_ci_workflows = ['fields_ci_workflows_example'] # List[str] | the fields to include for returned resources of type ciWorkflows (optional)
    fields_scm_repositories = ['fields_scm_repositories_example'] # List[str] | the fields to include for returned resources of type scmRepositories (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.ci_workflows_get_instance(id, fields_ci_workflows=fields_ci_workflows, fields_scm_repositories=fields_scm_repositories, include=include)
        print("The response of CiWorkflowsApi->ci_workflows_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiWorkflowsApi->ci_workflows_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_ci_workflows** | [**List[str]**](str.md)| the fields to include for returned resources of type ciWorkflows | [optional] 
 **fields_scm_repositories** | [**List[str]**](str.md)| the fields to include for returned resources of type scmRepositories | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**CiWorkflowResponse**](CiWorkflowResponse.md)

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
**200** | Single CiWorkflow |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_workflows_repository_get_to_one_related**
> ScmRepositoryResponse ci_workflows_repository_get_to_one_related(id, fields_scm_repositories=fields_scm_repositories, fields_scm_providers=fields_scm_providers, fields_scm_git_references=fields_scm_git_references, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.scm_repository_response import ScmRepositoryResponse
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
    api_instance = openapi_client.CiWorkflowsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_scm_repositories = ['fields_scm_repositories_example'] # List[str] | the fields to include for returned resources of type scmRepositories (optional)
    fields_scm_providers = ['fields_scm_providers_example'] # List[str] | the fields to include for returned resources of type scmProviders (optional)
    fields_scm_git_references = ['fields_scm_git_references_example'] # List[str] | the fields to include for returned resources of type scmGitReferences (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.ci_workflows_repository_get_to_one_related(id, fields_scm_repositories=fields_scm_repositories, fields_scm_providers=fields_scm_providers, fields_scm_git_references=fields_scm_git_references, include=include)
        print("The response of CiWorkflowsApi->ci_workflows_repository_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiWorkflowsApi->ci_workflows_repository_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_scm_repositories** | [**List[str]**](str.md)| the fields to include for returned resources of type scmRepositories | [optional] 
 **fields_scm_providers** | [**List[str]**](str.md)| the fields to include for returned resources of type scmProviders | [optional] 
 **fields_scm_git_references** | [**List[str]**](str.md)| the fields to include for returned resources of type scmGitReferences | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**ScmRepositoryResponse**](ScmRepositoryResponse.md)

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
**200** | Single ScmRepository |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_workflows_repository_get_to_one_relationship**
> CiWorkflowRepositoryLinkageResponse ci_workflows_repository_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_workflow_repository_linkage_response import CiWorkflowRepositoryLinkageResponse
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
    api_instance = openapi_client.CiWorkflowsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.ci_workflows_repository_get_to_one_relationship(id)
        print("The response of CiWorkflowsApi->ci_workflows_repository_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiWorkflowsApi->ci_workflows_repository_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**CiWorkflowRepositoryLinkageResponse**](CiWorkflowRepositoryLinkageResponse.md)

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
**200** | Related linkage |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_workflows_update_instance**
> CiWorkflowResponse ci_workflows_update_instance(id, ci_workflow_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_workflow_response import CiWorkflowResponse
from openapi_client.models.ci_workflow_update_request import CiWorkflowUpdateRequest
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
    api_instance = openapi_client.CiWorkflowsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    ci_workflow_update_request = openapi_client.CiWorkflowUpdateRequest() # CiWorkflowUpdateRequest | CiWorkflow representation

    try:
        api_response = api_instance.ci_workflows_update_instance(id, ci_workflow_update_request)
        print("The response of CiWorkflowsApi->ci_workflows_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiWorkflowsApi->ci_workflows_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **ci_workflow_update_request** | [**CiWorkflowUpdateRequest**](CiWorkflowUpdateRequest.md)| CiWorkflow representation | 

### Return type

[**CiWorkflowResponse**](CiWorkflowResponse.md)

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
**200** | Single CiWorkflow |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

