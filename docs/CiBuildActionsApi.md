# openapi_client.CiBuildActionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ci_build_actions_artifacts_get_to_many_related**](CiBuildActionsApi.md#ci_build_actions_artifacts_get_to_many_related) | **GET** /v1/ciBuildActions/{id}/artifacts | 
[**ci_build_actions_artifacts_get_to_many_relationship**](CiBuildActionsApi.md#ci_build_actions_artifacts_get_to_many_relationship) | **GET** /v1/ciBuildActions/{id}/relationships/artifacts | 
[**ci_build_actions_build_run_get_to_one_related**](CiBuildActionsApi.md#ci_build_actions_build_run_get_to_one_related) | **GET** /v1/ciBuildActions/{id}/buildRun | 
[**ci_build_actions_build_run_get_to_one_relationship**](CiBuildActionsApi.md#ci_build_actions_build_run_get_to_one_relationship) | **GET** /v1/ciBuildActions/{id}/relationships/buildRun | 
[**ci_build_actions_get_instance**](CiBuildActionsApi.md#ci_build_actions_get_instance) | **GET** /v1/ciBuildActions/{id} | 
[**ci_build_actions_issues_get_to_many_related**](CiBuildActionsApi.md#ci_build_actions_issues_get_to_many_related) | **GET** /v1/ciBuildActions/{id}/issues | 
[**ci_build_actions_issues_get_to_many_relationship**](CiBuildActionsApi.md#ci_build_actions_issues_get_to_many_relationship) | **GET** /v1/ciBuildActions/{id}/relationships/issues | 
[**ci_build_actions_test_results_get_to_many_related**](CiBuildActionsApi.md#ci_build_actions_test_results_get_to_many_related) | **GET** /v1/ciBuildActions/{id}/testResults | 
[**ci_build_actions_test_results_get_to_many_relationship**](CiBuildActionsApi.md#ci_build_actions_test_results_get_to_many_relationship) | **GET** /v1/ciBuildActions/{id}/relationships/testResults | 


# **ci_build_actions_artifacts_get_to_many_related**
> CiArtifactsResponse ci_build_actions_artifacts_get_to_many_related(id, fields_ci_artifacts=fields_ci_artifacts, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_artifacts_response import CiArtifactsResponse
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
    api_instance = openapi_client.CiBuildActionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_ci_artifacts = ['fields_ci_artifacts_example'] # List[str] | the fields to include for returned resources of type ciArtifacts (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.ci_build_actions_artifacts_get_to_many_related(id, fields_ci_artifacts=fields_ci_artifacts, limit=limit)
        print("The response of CiBuildActionsApi->ci_build_actions_artifacts_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiBuildActionsApi->ci_build_actions_artifacts_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_ci_artifacts** | [**List[str]**](str.md)| the fields to include for returned resources of type ciArtifacts | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**CiArtifactsResponse**](CiArtifactsResponse.md)

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
**200** | List of CiArtifacts |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_build_actions_artifacts_get_to_many_relationship**
> CiBuildActionArtifactsLinkagesResponse ci_build_actions_artifacts_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_build_action_artifacts_linkages_response import CiBuildActionArtifactsLinkagesResponse
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
    api_instance = openapi_client.CiBuildActionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.ci_build_actions_artifacts_get_to_many_relationship(id, limit=limit)
        print("The response of CiBuildActionsApi->ci_build_actions_artifacts_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiBuildActionsApi->ci_build_actions_artifacts_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**CiBuildActionArtifactsLinkagesResponse**](CiBuildActionArtifactsLinkagesResponse.md)

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

# **ci_build_actions_build_run_get_to_one_related**
> CiBuildRunResponse ci_build_actions_build_run_get_to_one_related(id, fields_ci_build_runs=fields_ci_build_runs, fields_builds=fields_builds, fields_ci_workflows=fields_ci_workflows, fields_ci_products=fields_ci_products, fields_scm_git_references=fields_scm_git_references, fields_scm_pull_requests=fields_scm_pull_requests, include=include, limit_builds=limit_builds)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_build_run_response import CiBuildRunResponse
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
    api_instance = openapi_client.CiBuildActionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_ci_build_runs = ['fields_ci_build_runs_example'] # List[str] | the fields to include for returned resources of type ciBuildRuns (optional)
    fields_builds = ['fields_builds_example'] # List[str] | the fields to include for returned resources of type builds (optional)
    fields_ci_workflows = ['fields_ci_workflows_example'] # List[str] | the fields to include for returned resources of type ciWorkflows (optional)
    fields_ci_products = ['fields_ci_products_example'] # List[str] | the fields to include for returned resources of type ciProducts (optional)
    fields_scm_git_references = ['fields_scm_git_references_example'] # List[str] | the fields to include for returned resources of type scmGitReferences (optional)
    fields_scm_pull_requests = ['fields_scm_pull_requests_example'] # List[str] | the fields to include for returned resources of type scmPullRequests (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_builds = 56 # int | maximum number of related builds returned (when they are included) (optional)

    try:
        api_response = api_instance.ci_build_actions_build_run_get_to_one_related(id, fields_ci_build_runs=fields_ci_build_runs, fields_builds=fields_builds, fields_ci_workflows=fields_ci_workflows, fields_ci_products=fields_ci_products, fields_scm_git_references=fields_scm_git_references, fields_scm_pull_requests=fields_scm_pull_requests, include=include, limit_builds=limit_builds)
        print("The response of CiBuildActionsApi->ci_build_actions_build_run_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiBuildActionsApi->ci_build_actions_build_run_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_ci_build_runs** | [**List[str]**](str.md)| the fields to include for returned resources of type ciBuildRuns | [optional] 
 **fields_builds** | [**List[str]**](str.md)| the fields to include for returned resources of type builds | [optional] 
 **fields_ci_workflows** | [**List[str]**](str.md)| the fields to include for returned resources of type ciWorkflows | [optional] 
 **fields_ci_products** | [**List[str]**](str.md)| the fields to include for returned resources of type ciProducts | [optional] 
 **fields_scm_git_references** | [**List[str]**](str.md)| the fields to include for returned resources of type scmGitReferences | [optional] 
 **fields_scm_pull_requests** | [**List[str]**](str.md)| the fields to include for returned resources of type scmPullRequests | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_builds** | **int**| maximum number of related builds returned (when they are included) | [optional] 

### Return type

[**CiBuildRunResponse**](CiBuildRunResponse.md)

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
**200** | Single CiBuildRun |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_build_actions_build_run_get_to_one_relationship**
> CiBuildActionBuildRunLinkageResponse ci_build_actions_build_run_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_build_action_build_run_linkage_response import CiBuildActionBuildRunLinkageResponse
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
    api_instance = openapi_client.CiBuildActionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.ci_build_actions_build_run_get_to_one_relationship(id)
        print("The response of CiBuildActionsApi->ci_build_actions_build_run_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiBuildActionsApi->ci_build_actions_build_run_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**CiBuildActionBuildRunLinkageResponse**](CiBuildActionBuildRunLinkageResponse.md)

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

# **ci_build_actions_get_instance**
> CiBuildActionResponse ci_build_actions_get_instance(id, fields_ci_build_actions=fields_ci_build_actions, fields_ci_build_runs=fields_ci_build_runs, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_build_action_response import CiBuildActionResponse
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
    api_instance = openapi_client.CiBuildActionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_ci_build_actions = ['fields_ci_build_actions_example'] # List[str] | the fields to include for returned resources of type ciBuildActions (optional)
    fields_ci_build_runs = ['fields_ci_build_runs_example'] # List[str] | the fields to include for returned resources of type ciBuildRuns (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.ci_build_actions_get_instance(id, fields_ci_build_actions=fields_ci_build_actions, fields_ci_build_runs=fields_ci_build_runs, include=include)
        print("The response of CiBuildActionsApi->ci_build_actions_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiBuildActionsApi->ci_build_actions_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_ci_build_actions** | [**List[str]**](str.md)| the fields to include for returned resources of type ciBuildActions | [optional] 
 **fields_ci_build_runs** | [**List[str]**](str.md)| the fields to include for returned resources of type ciBuildRuns | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**CiBuildActionResponse**](CiBuildActionResponse.md)

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
**200** | Single CiBuildAction |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_build_actions_issues_get_to_many_related**
> CiIssuesResponse ci_build_actions_issues_get_to_many_related(id, fields_ci_issues=fields_ci_issues, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_issues_response import CiIssuesResponse
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
    api_instance = openapi_client.CiBuildActionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_ci_issues = ['fields_ci_issues_example'] # List[str] | the fields to include for returned resources of type ciIssues (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.ci_build_actions_issues_get_to_many_related(id, fields_ci_issues=fields_ci_issues, limit=limit)
        print("The response of CiBuildActionsApi->ci_build_actions_issues_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiBuildActionsApi->ci_build_actions_issues_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_ci_issues** | [**List[str]**](str.md)| the fields to include for returned resources of type ciIssues | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**CiIssuesResponse**](CiIssuesResponse.md)

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
**200** | List of CiIssues |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_build_actions_issues_get_to_many_relationship**
> CiBuildActionIssuesLinkagesResponse ci_build_actions_issues_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_build_action_issues_linkages_response import CiBuildActionIssuesLinkagesResponse
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
    api_instance = openapi_client.CiBuildActionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.ci_build_actions_issues_get_to_many_relationship(id, limit=limit)
        print("The response of CiBuildActionsApi->ci_build_actions_issues_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiBuildActionsApi->ci_build_actions_issues_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**CiBuildActionIssuesLinkagesResponse**](CiBuildActionIssuesLinkagesResponse.md)

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

# **ci_build_actions_test_results_get_to_many_related**
> CiTestResultsResponse ci_build_actions_test_results_get_to_many_related(id, fields_ci_test_results=fields_ci_test_results, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_test_results_response import CiTestResultsResponse
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
    api_instance = openapi_client.CiBuildActionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_ci_test_results = ['fields_ci_test_results_example'] # List[str] | the fields to include for returned resources of type ciTestResults (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.ci_build_actions_test_results_get_to_many_related(id, fields_ci_test_results=fields_ci_test_results, limit=limit)
        print("The response of CiBuildActionsApi->ci_build_actions_test_results_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiBuildActionsApi->ci_build_actions_test_results_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_ci_test_results** | [**List[str]**](str.md)| the fields to include for returned resources of type ciTestResults | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**CiTestResultsResponse**](CiTestResultsResponse.md)

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
**200** | List of CiTestResults |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_build_actions_test_results_get_to_many_relationship**
> CiBuildActionTestResultsLinkagesResponse ci_build_actions_test_results_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_build_action_test_results_linkages_response import CiBuildActionTestResultsLinkagesResponse
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
    api_instance = openapi_client.CiBuildActionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.ci_build_actions_test_results_get_to_many_relationship(id, limit=limit)
        print("The response of CiBuildActionsApi->ci_build_actions_test_results_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiBuildActionsApi->ci_build_actions_test_results_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**CiBuildActionTestResultsLinkagesResponse**](CiBuildActionTestResultsLinkagesResponse.md)

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

