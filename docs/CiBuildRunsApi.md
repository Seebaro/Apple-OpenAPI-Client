# openapi_client.CiBuildRunsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ci_build_runs_actions_get_to_many_related**](CiBuildRunsApi.md#ci_build_runs_actions_get_to_many_related) | **GET** /v1/ciBuildRuns/{id}/actions | 
[**ci_build_runs_actions_get_to_many_relationship**](CiBuildRunsApi.md#ci_build_runs_actions_get_to_many_relationship) | **GET** /v1/ciBuildRuns/{id}/relationships/actions | 
[**ci_build_runs_builds_get_to_many_related**](CiBuildRunsApi.md#ci_build_runs_builds_get_to_many_related) | **GET** /v1/ciBuildRuns/{id}/builds | 
[**ci_build_runs_builds_get_to_many_relationship**](CiBuildRunsApi.md#ci_build_runs_builds_get_to_many_relationship) | **GET** /v1/ciBuildRuns/{id}/relationships/builds | 
[**ci_build_runs_create_instance**](CiBuildRunsApi.md#ci_build_runs_create_instance) | **POST** /v1/ciBuildRuns | 
[**ci_build_runs_get_instance**](CiBuildRunsApi.md#ci_build_runs_get_instance) | **GET** /v1/ciBuildRuns/{id} | 


# **ci_build_runs_actions_get_to_many_related**
> CiBuildActionsResponse ci_build_runs_actions_get_to_many_related(id, fields_ci_build_actions=fields_ci_build_actions, fields_ci_build_runs=fields_ci_build_runs, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_build_actions_response import CiBuildActionsResponse
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
    api_instance = openapi_client.CiBuildRunsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_ci_build_actions = ['fields_ci_build_actions_example'] # List[str] | the fields to include for returned resources of type ciBuildActions (optional)
    fields_ci_build_runs = ['fields_ci_build_runs_example'] # List[str] | the fields to include for returned resources of type ciBuildRuns (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.ci_build_runs_actions_get_to_many_related(id, fields_ci_build_actions=fields_ci_build_actions, fields_ci_build_runs=fields_ci_build_runs, limit=limit, include=include)
        print("The response of CiBuildRunsApi->ci_build_runs_actions_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiBuildRunsApi->ci_build_runs_actions_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_ci_build_actions** | [**List[str]**](str.md)| the fields to include for returned resources of type ciBuildActions | [optional] 
 **fields_ci_build_runs** | [**List[str]**](str.md)| the fields to include for returned resources of type ciBuildRuns | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**CiBuildActionsResponse**](CiBuildActionsResponse.md)

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
**200** | List of CiBuildActions |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_build_runs_actions_get_to_many_relationship**
> CiBuildRunActionsLinkagesResponse ci_build_runs_actions_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_build_run_actions_linkages_response import CiBuildRunActionsLinkagesResponse
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
    api_instance = openapi_client.CiBuildRunsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.ci_build_runs_actions_get_to_many_relationship(id, limit=limit)
        print("The response of CiBuildRunsApi->ci_build_runs_actions_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiBuildRunsApi->ci_build_runs_actions_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**CiBuildRunActionsLinkagesResponse**](CiBuildRunActionsLinkagesResponse.md)

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

# **ci_build_runs_builds_get_to_many_related**
> BuildsResponse ci_build_runs_builds_get_to_many_related(id, filter_version=filter_version, filter_expired=filter_expired, filter_processing_state=filter_processing_state, filter_beta_app_review_submission_beta_review_state=filter_beta_app_review_submission_beta_review_state, filter_uses_non_exempt_encryption=filter_uses_non_exempt_encryption, filter_pre_release_version_version=filter_pre_release_version_version, filter_pre_release_version_platform=filter_pre_release_version_platform, filter_build_audience_type=filter_build_audience_type, filter_pre_release_version=filter_pre_release_version, filter_app=filter_app, filter_beta_groups=filter_beta_groups, filter_app_store_version=filter_app_store_version, filter_id=filter_id, exists_uses_non_exempt_encryption=exists_uses_non_exempt_encryption, sort=sort, fields_builds=fields_builds, fields_pre_release_versions=fields_pre_release_versions, fields_beta_testers=fields_beta_testers, fields_beta_groups=fields_beta_groups, fields_beta_build_localizations=fields_beta_build_localizations, fields_app_encryption_declarations=fields_app_encryption_declarations, fields_beta_app_review_submissions=fields_beta_app_review_submissions, fields_apps=fields_apps, fields_build_beta_details=fields_build_beta_details, fields_app_store_versions=fields_app_store_versions, fields_build_icons=fields_build_icons, fields_build_bundles=fields_build_bundles, limit=limit, include=include, limit_individual_testers=limit_individual_testers, limit_beta_groups=limit_beta_groups, limit_beta_build_localizations=limit_beta_build_localizations, limit_icons=limit_icons, limit_build_bundles=limit_build_bundles)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.builds_response import BuildsResponse
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
    api_instance = openapi_client.CiBuildRunsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_version = ['filter_version_example'] # List[str] | filter by attribute 'version' (optional)
    filter_expired = ['filter_expired_example'] # List[str] | filter by attribute 'expired' (optional)
    filter_processing_state = ['filter_processing_state_example'] # List[str] | filter by attribute 'processingState' (optional)
    filter_beta_app_review_submission_beta_review_state = ['filter_beta_app_review_submission_beta_review_state_example'] # List[str] | filter by attribute 'betaAppReviewSubmission.betaReviewState' (optional)
    filter_uses_non_exempt_encryption = ['filter_uses_non_exempt_encryption_example'] # List[str] | filter by attribute 'usesNonExemptEncryption' (optional)
    filter_pre_release_version_version = ['filter_pre_release_version_version_example'] # List[str] | filter by attribute 'preReleaseVersion.version' (optional)
    filter_pre_release_version_platform = ['filter_pre_release_version_platform_example'] # List[str] | filter by attribute 'preReleaseVersion.platform' (optional)
    filter_build_audience_type = ['filter_build_audience_type_example'] # List[str] | filter by attribute 'buildAudienceType' (optional)
    filter_pre_release_version = ['filter_pre_release_version_example'] # List[str] | filter by id(s) of related 'preReleaseVersion' (optional)
    filter_app = ['filter_app_example'] # List[str] | filter by id(s) of related 'app' (optional)
    filter_beta_groups = ['filter_beta_groups_example'] # List[str] | filter by id(s) of related 'betaGroups' (optional)
    filter_app_store_version = ['filter_app_store_version_example'] # List[str] | filter by id(s) of related 'appStoreVersion' (optional)
    filter_id = ['filter_id_example'] # List[str] | filter by id(s) (optional)
    exists_uses_non_exempt_encryption = True # bool | filter by attribute 'usesNonExemptEncryption' (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; resources will be sorted as specified (optional)
    fields_builds = ['fields_builds_example'] # List[str] | the fields to include for returned resources of type builds (optional)
    fields_pre_release_versions = ['fields_pre_release_versions_example'] # List[str] | the fields to include for returned resources of type preReleaseVersions (optional)
    fields_beta_testers = ['fields_beta_testers_example'] # List[str] | the fields to include for returned resources of type betaTesters (optional)
    fields_beta_groups = ['fields_beta_groups_example'] # List[str] | the fields to include for returned resources of type betaGroups (optional)
    fields_beta_build_localizations = ['fields_beta_build_localizations_example'] # List[str] | the fields to include for returned resources of type betaBuildLocalizations (optional)
    fields_app_encryption_declarations = ['fields_app_encryption_declarations_example'] # List[str] | the fields to include for returned resources of type appEncryptionDeclarations (optional)
    fields_beta_app_review_submissions = ['fields_beta_app_review_submissions_example'] # List[str] | the fields to include for returned resources of type betaAppReviewSubmissions (optional)
    fields_apps = ['fields_apps_example'] # List[str] | the fields to include for returned resources of type apps (optional)
    fields_build_beta_details = ['fields_build_beta_details_example'] # List[str] | the fields to include for returned resources of type buildBetaDetails (optional)
    fields_app_store_versions = ['fields_app_store_versions_example'] # List[str] | the fields to include for returned resources of type appStoreVersions (optional)
    fields_build_icons = ['fields_build_icons_example'] # List[str] | the fields to include for returned resources of type buildIcons (optional)
    fields_build_bundles = ['fields_build_bundles_example'] # List[str] | the fields to include for returned resources of type buildBundles (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_individual_testers = 56 # int | maximum number of related individualTesters returned (when they are included) (optional)
    limit_beta_groups = 56 # int | maximum number of related betaGroups returned (when they are included) (optional)
    limit_beta_build_localizations = 56 # int | maximum number of related betaBuildLocalizations returned (when they are included) (optional)
    limit_icons = 56 # int | maximum number of related icons returned (when they are included) (optional)
    limit_build_bundles = 56 # int | maximum number of related buildBundles returned (when they are included) (optional)

    try:
        api_response = api_instance.ci_build_runs_builds_get_to_many_related(id, filter_version=filter_version, filter_expired=filter_expired, filter_processing_state=filter_processing_state, filter_beta_app_review_submission_beta_review_state=filter_beta_app_review_submission_beta_review_state, filter_uses_non_exempt_encryption=filter_uses_non_exempt_encryption, filter_pre_release_version_version=filter_pre_release_version_version, filter_pre_release_version_platform=filter_pre_release_version_platform, filter_build_audience_type=filter_build_audience_type, filter_pre_release_version=filter_pre_release_version, filter_app=filter_app, filter_beta_groups=filter_beta_groups, filter_app_store_version=filter_app_store_version, filter_id=filter_id, exists_uses_non_exempt_encryption=exists_uses_non_exempt_encryption, sort=sort, fields_builds=fields_builds, fields_pre_release_versions=fields_pre_release_versions, fields_beta_testers=fields_beta_testers, fields_beta_groups=fields_beta_groups, fields_beta_build_localizations=fields_beta_build_localizations, fields_app_encryption_declarations=fields_app_encryption_declarations, fields_beta_app_review_submissions=fields_beta_app_review_submissions, fields_apps=fields_apps, fields_build_beta_details=fields_build_beta_details, fields_app_store_versions=fields_app_store_versions, fields_build_icons=fields_build_icons, fields_build_bundles=fields_build_bundles, limit=limit, include=include, limit_individual_testers=limit_individual_testers, limit_beta_groups=limit_beta_groups, limit_beta_build_localizations=limit_beta_build_localizations, limit_icons=limit_icons, limit_build_bundles=limit_build_bundles)
        print("The response of CiBuildRunsApi->ci_build_runs_builds_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiBuildRunsApi->ci_build_runs_builds_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_version** | [**List[str]**](str.md)| filter by attribute &#39;version&#39; | [optional] 
 **filter_expired** | [**List[str]**](str.md)| filter by attribute &#39;expired&#39; | [optional] 
 **filter_processing_state** | [**List[str]**](str.md)| filter by attribute &#39;processingState&#39; | [optional] 
 **filter_beta_app_review_submission_beta_review_state** | [**List[str]**](str.md)| filter by attribute &#39;betaAppReviewSubmission.betaReviewState&#39; | [optional] 
 **filter_uses_non_exempt_encryption** | [**List[str]**](str.md)| filter by attribute &#39;usesNonExemptEncryption&#39; | [optional] 
 **filter_pre_release_version_version** | [**List[str]**](str.md)| filter by attribute &#39;preReleaseVersion.version&#39; | [optional] 
 **filter_pre_release_version_platform** | [**List[str]**](str.md)| filter by attribute &#39;preReleaseVersion.platform&#39; | [optional] 
 **filter_build_audience_type** | [**List[str]**](str.md)| filter by attribute &#39;buildAudienceType&#39; | [optional] 
 **filter_pre_release_version** | [**List[str]**](str.md)| filter by id(s) of related &#39;preReleaseVersion&#39; | [optional] 
 **filter_app** | [**List[str]**](str.md)| filter by id(s) of related &#39;app&#39; | [optional] 
 **filter_beta_groups** | [**List[str]**](str.md)| filter by id(s) of related &#39;betaGroups&#39; | [optional] 
 **filter_app_store_version** | [**List[str]**](str.md)| filter by id(s) of related &#39;appStoreVersion&#39; | [optional] 
 **filter_id** | [**List[str]**](str.md)| filter by id(s) | [optional] 
 **exists_uses_non_exempt_encryption** | **bool**| filter by attribute &#39;usesNonExemptEncryption&#39; | [optional] 
 **sort** | [**List[str]**](str.md)| comma-separated list of sort expressions; resources will be sorted as specified | [optional] 
 **fields_builds** | [**List[str]**](str.md)| the fields to include for returned resources of type builds | [optional] 
 **fields_pre_release_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type preReleaseVersions | [optional] 
 **fields_beta_testers** | [**List[str]**](str.md)| the fields to include for returned resources of type betaTesters | [optional] 
 **fields_beta_groups** | [**List[str]**](str.md)| the fields to include for returned resources of type betaGroups | [optional] 
 **fields_beta_build_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type betaBuildLocalizations | [optional] 
 **fields_app_encryption_declarations** | [**List[str]**](str.md)| the fields to include for returned resources of type appEncryptionDeclarations | [optional] 
 **fields_beta_app_review_submissions** | [**List[str]**](str.md)| the fields to include for returned resources of type betaAppReviewSubmissions | [optional] 
 **fields_apps** | [**List[str]**](str.md)| the fields to include for returned resources of type apps | [optional] 
 **fields_build_beta_details** | [**List[str]**](str.md)| the fields to include for returned resources of type buildBetaDetails | [optional] 
 **fields_app_store_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersions | [optional] 
 **fields_build_icons** | [**List[str]**](str.md)| the fields to include for returned resources of type buildIcons | [optional] 
 **fields_build_bundles** | [**List[str]**](str.md)| the fields to include for returned resources of type buildBundles | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_individual_testers** | **int**| maximum number of related individualTesters returned (when they are included) | [optional] 
 **limit_beta_groups** | **int**| maximum number of related betaGroups returned (when they are included) | [optional] 
 **limit_beta_build_localizations** | **int**| maximum number of related betaBuildLocalizations returned (when they are included) | [optional] 
 **limit_icons** | **int**| maximum number of related icons returned (when they are included) | [optional] 
 **limit_build_bundles** | **int**| maximum number of related buildBundles returned (when they are included) | [optional] 

### Return type

[**BuildsResponse**](BuildsResponse.md)

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
**200** | List of Builds |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_build_runs_builds_get_to_many_relationship**
> CiBuildRunBuildsLinkagesResponse ci_build_runs_builds_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_build_run_builds_linkages_response import CiBuildRunBuildsLinkagesResponse
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
    api_instance = openapi_client.CiBuildRunsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.ci_build_runs_builds_get_to_many_relationship(id, limit=limit)
        print("The response of CiBuildRunsApi->ci_build_runs_builds_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiBuildRunsApi->ci_build_runs_builds_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**CiBuildRunBuildsLinkagesResponse**](CiBuildRunBuildsLinkagesResponse.md)

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

# **ci_build_runs_create_instance**
> CiBuildRunResponse ci_build_runs_create_instance(ci_build_run_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_build_run_create_request import CiBuildRunCreateRequest
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
    api_instance = openapi_client.CiBuildRunsApi(api_client)
    ci_build_run_create_request = openapi_client.CiBuildRunCreateRequest() # CiBuildRunCreateRequest | CiBuildRun representation

    try:
        api_response = api_instance.ci_build_runs_create_instance(ci_build_run_create_request)
        print("The response of CiBuildRunsApi->ci_build_runs_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiBuildRunsApi->ci_build_runs_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ci_build_run_create_request** | [**CiBuildRunCreateRequest**](CiBuildRunCreateRequest.md)| CiBuildRun representation | 

### Return type

[**CiBuildRunResponse**](CiBuildRunResponse.md)

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
**201** | Single CiBuildRun |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_build_runs_get_instance**
> CiBuildRunResponse ci_build_runs_get_instance(id, fields_ci_build_runs=fields_ci_build_runs, fields_builds=fields_builds, include=include, limit_builds=limit_builds)

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
    api_instance = openapi_client.CiBuildRunsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_ci_build_runs = ['fields_ci_build_runs_example'] # List[str] | the fields to include for returned resources of type ciBuildRuns (optional)
    fields_builds = ['fields_builds_example'] # List[str] | the fields to include for returned resources of type builds (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_builds = 56 # int | maximum number of related builds returned (when they are included) (optional)

    try:
        api_response = api_instance.ci_build_runs_get_instance(id, fields_ci_build_runs=fields_ci_build_runs, fields_builds=fields_builds, include=include, limit_builds=limit_builds)
        print("The response of CiBuildRunsApi->ci_build_runs_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiBuildRunsApi->ci_build_runs_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_ci_build_runs** | [**List[str]**](str.md)| the fields to include for returned resources of type ciBuildRuns | [optional] 
 **fields_builds** | [**List[str]**](str.md)| the fields to include for returned resources of type builds | [optional] 
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

