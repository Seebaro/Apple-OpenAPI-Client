# openapi_client.ScmRepositoriesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**scm_repositories_get_collection**](ScmRepositoriesApi.md#scm_repositories_get_collection) | **GET** /v1/scmRepositories | 
[**scm_repositories_get_instance**](ScmRepositoriesApi.md#scm_repositories_get_instance) | **GET** /v1/scmRepositories/{id} | 
[**scm_repositories_git_references_get_to_many_related**](ScmRepositoriesApi.md#scm_repositories_git_references_get_to_many_related) | **GET** /v1/scmRepositories/{id}/gitReferences | 
[**scm_repositories_git_references_get_to_many_relationship**](ScmRepositoriesApi.md#scm_repositories_git_references_get_to_many_relationship) | **GET** /v1/scmRepositories/{id}/relationships/gitReferences | 
[**scm_repositories_pull_requests_get_to_many_related**](ScmRepositoriesApi.md#scm_repositories_pull_requests_get_to_many_related) | **GET** /v1/scmRepositories/{id}/pullRequests | 
[**scm_repositories_pull_requests_get_to_many_relationship**](ScmRepositoriesApi.md#scm_repositories_pull_requests_get_to_many_relationship) | **GET** /v1/scmRepositories/{id}/relationships/pullRequests | 


# **scm_repositories_get_collection**
> ScmRepositoriesResponse scm_repositories_get_collection(filter_id=filter_id, fields_scm_repositories=fields_scm_repositories, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.scm_repositories_response import ScmRepositoriesResponse
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
    api_instance = openapi_client.ScmRepositoriesApi(api_client)
    filter_id = ['filter_id_example'] # List[str] | filter by id(s) (optional)
    fields_scm_repositories = ['fields_scm_repositories_example'] # List[str] | the fields to include for returned resources of type scmRepositories (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.scm_repositories_get_collection(filter_id=filter_id, fields_scm_repositories=fields_scm_repositories, limit=limit, include=include)
        print("The response of ScmRepositoriesApi->scm_repositories_get_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ScmRepositoriesApi->scm_repositories_get_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter_id** | [**List[str]**](str.md)| filter by id(s) | [optional] 
 **fields_scm_repositories** | [**List[str]**](str.md)| the fields to include for returned resources of type scmRepositories | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**ScmRepositoriesResponse**](ScmRepositoriesResponse.md)

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
**200** | List of ScmRepositories |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **scm_repositories_get_instance**
> ScmRepositoryResponse scm_repositories_get_instance(id, fields_scm_repositories=fields_scm_repositories, include=include)

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
    api_instance = openapi_client.ScmRepositoriesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_scm_repositories = ['fields_scm_repositories_example'] # List[str] | the fields to include for returned resources of type scmRepositories (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.scm_repositories_get_instance(id, fields_scm_repositories=fields_scm_repositories, include=include)
        print("The response of ScmRepositoriesApi->scm_repositories_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ScmRepositoriesApi->scm_repositories_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_scm_repositories** | [**List[str]**](str.md)| the fields to include for returned resources of type scmRepositories | [optional] 
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

# **scm_repositories_git_references_get_to_many_related**
> ScmGitReferencesResponse scm_repositories_git_references_get_to_many_related(id, fields_scm_git_references=fields_scm_git_references, fields_scm_repositories=fields_scm_repositories, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.scm_git_references_response import ScmGitReferencesResponse
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
    api_instance = openapi_client.ScmRepositoriesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_scm_git_references = ['fields_scm_git_references_example'] # List[str] | the fields to include for returned resources of type scmGitReferences (optional)
    fields_scm_repositories = ['fields_scm_repositories_example'] # List[str] | the fields to include for returned resources of type scmRepositories (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.scm_repositories_git_references_get_to_many_related(id, fields_scm_git_references=fields_scm_git_references, fields_scm_repositories=fields_scm_repositories, limit=limit, include=include)
        print("The response of ScmRepositoriesApi->scm_repositories_git_references_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ScmRepositoriesApi->scm_repositories_git_references_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_scm_git_references** | [**List[str]**](str.md)| the fields to include for returned resources of type scmGitReferences | [optional] 
 **fields_scm_repositories** | [**List[str]**](str.md)| the fields to include for returned resources of type scmRepositories | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**ScmGitReferencesResponse**](ScmGitReferencesResponse.md)

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
**200** | List of ScmGitReferences |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **scm_repositories_git_references_get_to_many_relationship**
> ScmRepositoryGitReferencesLinkagesResponse scm_repositories_git_references_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.scm_repository_git_references_linkages_response import ScmRepositoryGitReferencesLinkagesResponse
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
    api_instance = openapi_client.ScmRepositoriesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.scm_repositories_git_references_get_to_many_relationship(id, limit=limit)
        print("The response of ScmRepositoriesApi->scm_repositories_git_references_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ScmRepositoriesApi->scm_repositories_git_references_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**ScmRepositoryGitReferencesLinkagesResponse**](ScmRepositoryGitReferencesLinkagesResponse.md)

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

# **scm_repositories_pull_requests_get_to_many_related**
> ScmPullRequestsResponse scm_repositories_pull_requests_get_to_many_related(id, fields_scm_pull_requests=fields_scm_pull_requests, fields_scm_repositories=fields_scm_repositories, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.scm_pull_requests_response import ScmPullRequestsResponse
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
    api_instance = openapi_client.ScmRepositoriesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_scm_pull_requests = ['fields_scm_pull_requests_example'] # List[str] | the fields to include for returned resources of type scmPullRequests (optional)
    fields_scm_repositories = ['fields_scm_repositories_example'] # List[str] | the fields to include for returned resources of type scmRepositories (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.scm_repositories_pull_requests_get_to_many_related(id, fields_scm_pull_requests=fields_scm_pull_requests, fields_scm_repositories=fields_scm_repositories, limit=limit, include=include)
        print("The response of ScmRepositoriesApi->scm_repositories_pull_requests_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ScmRepositoriesApi->scm_repositories_pull_requests_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_scm_pull_requests** | [**List[str]**](str.md)| the fields to include for returned resources of type scmPullRequests | [optional] 
 **fields_scm_repositories** | [**List[str]**](str.md)| the fields to include for returned resources of type scmRepositories | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**ScmPullRequestsResponse**](ScmPullRequestsResponse.md)

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
**200** | List of ScmPullRequests |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **scm_repositories_pull_requests_get_to_many_relationship**
> ScmRepositoryPullRequestsLinkagesResponse scm_repositories_pull_requests_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.scm_repository_pull_requests_linkages_response import ScmRepositoryPullRequestsLinkagesResponse
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
    api_instance = openapi_client.ScmRepositoriesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.scm_repositories_pull_requests_get_to_many_relationship(id, limit=limit)
        print("The response of ScmRepositoriesApi->scm_repositories_pull_requests_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ScmRepositoriesApi->scm_repositories_pull_requests_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**ScmRepositoryPullRequestsLinkagesResponse**](ScmRepositoryPullRequestsLinkagesResponse.md)

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

