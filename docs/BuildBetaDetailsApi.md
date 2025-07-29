# openapi_client.BuildBetaDetailsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**build_beta_details_build_get_to_one_related**](BuildBetaDetailsApi.md#build_beta_details_build_get_to_one_related) | **GET** /v1/buildBetaDetails/{id}/build | 
[**build_beta_details_build_get_to_one_relationship**](BuildBetaDetailsApi.md#build_beta_details_build_get_to_one_relationship) | **GET** /v1/buildBetaDetails/{id}/relationships/build | 
[**build_beta_details_get_collection**](BuildBetaDetailsApi.md#build_beta_details_get_collection) | **GET** /v1/buildBetaDetails | 
[**build_beta_details_get_instance**](BuildBetaDetailsApi.md#build_beta_details_get_instance) | **GET** /v1/buildBetaDetails/{id} | 
[**build_beta_details_update_instance**](BuildBetaDetailsApi.md#build_beta_details_update_instance) | **PATCH** /v1/buildBetaDetails/{id} | 


# **build_beta_details_build_get_to_one_related**
> BuildResponse build_beta_details_build_get_to_one_related(id, fields_builds=fields_builds, fields_pre_release_versions=fields_pre_release_versions, fields_beta_testers=fields_beta_testers, fields_beta_groups=fields_beta_groups, fields_beta_build_localizations=fields_beta_build_localizations, fields_app_encryption_declarations=fields_app_encryption_declarations, fields_beta_app_review_submissions=fields_beta_app_review_submissions, fields_apps=fields_apps, fields_build_beta_details=fields_build_beta_details, fields_app_store_versions=fields_app_store_versions, fields_build_icons=fields_build_icons, fields_build_bundles=fields_build_bundles, include=include, limit_individual_testers=limit_individual_testers, limit_beta_groups=limit_beta_groups, limit_beta_build_localizations=limit_beta_build_localizations, limit_icons=limit_icons, limit_build_bundles=limit_build_bundles)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_response import BuildResponse
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
    api_instance = openapi_client.BuildBetaDetailsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
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
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_individual_testers = 56 # int | maximum number of related individualTesters returned (when they are included) (optional)
    limit_beta_groups = 56 # int | maximum number of related betaGroups returned (when they are included) (optional)
    limit_beta_build_localizations = 56 # int | maximum number of related betaBuildLocalizations returned (when they are included) (optional)
    limit_icons = 56 # int | maximum number of related icons returned (when they are included) (optional)
    limit_build_bundles = 56 # int | maximum number of related buildBundles returned (when they are included) (optional)

    try:
        api_response = api_instance.build_beta_details_build_get_to_one_related(id, fields_builds=fields_builds, fields_pre_release_versions=fields_pre_release_versions, fields_beta_testers=fields_beta_testers, fields_beta_groups=fields_beta_groups, fields_beta_build_localizations=fields_beta_build_localizations, fields_app_encryption_declarations=fields_app_encryption_declarations, fields_beta_app_review_submissions=fields_beta_app_review_submissions, fields_apps=fields_apps, fields_build_beta_details=fields_build_beta_details, fields_app_store_versions=fields_app_store_versions, fields_build_icons=fields_build_icons, fields_build_bundles=fields_build_bundles, include=include, limit_individual_testers=limit_individual_testers, limit_beta_groups=limit_beta_groups, limit_beta_build_localizations=limit_beta_build_localizations, limit_icons=limit_icons, limit_build_bundles=limit_build_bundles)
        print("The response of BuildBetaDetailsApi->build_beta_details_build_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildBetaDetailsApi->build_beta_details_build_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
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
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_individual_testers** | **int**| maximum number of related individualTesters returned (when they are included) | [optional] 
 **limit_beta_groups** | **int**| maximum number of related betaGroups returned (when they are included) | [optional] 
 **limit_beta_build_localizations** | **int**| maximum number of related betaBuildLocalizations returned (when they are included) | [optional] 
 **limit_icons** | **int**| maximum number of related icons returned (when they are included) | [optional] 
 **limit_build_bundles** | **int**| maximum number of related buildBundles returned (when they are included) | [optional] 

### Return type

[**BuildResponse**](BuildResponse.md)

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
**200** | Single Build |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **build_beta_details_build_get_to_one_relationship**
> BuildBetaDetailBuildLinkageResponse build_beta_details_build_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_beta_detail_build_linkage_response import BuildBetaDetailBuildLinkageResponse
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
    api_instance = openapi_client.BuildBetaDetailsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.build_beta_details_build_get_to_one_relationship(id)
        print("The response of BuildBetaDetailsApi->build_beta_details_build_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildBetaDetailsApi->build_beta_details_build_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**BuildBetaDetailBuildLinkageResponse**](BuildBetaDetailBuildLinkageResponse.md)

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

# **build_beta_details_get_collection**
> BuildBetaDetailsResponse build_beta_details_get_collection(filter_build=filter_build, filter_id=filter_id, fields_build_beta_details=fields_build_beta_details, fields_builds=fields_builds, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_beta_details_response import BuildBetaDetailsResponse
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
    api_instance = openapi_client.BuildBetaDetailsApi(api_client)
    filter_build = ['filter_build_example'] # List[str] | filter by id(s) of related 'build' (optional)
    filter_id = ['filter_id_example'] # List[str] | filter by id(s) (optional)
    fields_build_beta_details = ['fields_build_beta_details_example'] # List[str] | the fields to include for returned resources of type buildBetaDetails (optional)
    fields_builds = ['fields_builds_example'] # List[str] | the fields to include for returned resources of type builds (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.build_beta_details_get_collection(filter_build=filter_build, filter_id=filter_id, fields_build_beta_details=fields_build_beta_details, fields_builds=fields_builds, limit=limit, include=include)
        print("The response of BuildBetaDetailsApi->build_beta_details_get_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildBetaDetailsApi->build_beta_details_get_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter_build** | [**List[str]**](str.md)| filter by id(s) of related &#39;build&#39; | [optional] 
 **filter_id** | [**List[str]**](str.md)| filter by id(s) | [optional] 
 **fields_build_beta_details** | [**List[str]**](str.md)| the fields to include for returned resources of type buildBetaDetails | [optional] 
 **fields_builds** | [**List[str]**](str.md)| the fields to include for returned resources of type builds | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**BuildBetaDetailsResponse**](BuildBetaDetailsResponse.md)

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
**200** | List of BuildBetaDetails |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **build_beta_details_get_instance**
> BuildBetaDetailResponse build_beta_details_get_instance(id, fields_build_beta_details=fields_build_beta_details, fields_builds=fields_builds, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_beta_detail_response import BuildBetaDetailResponse
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
    api_instance = openapi_client.BuildBetaDetailsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_build_beta_details = ['fields_build_beta_details_example'] # List[str] | the fields to include for returned resources of type buildBetaDetails (optional)
    fields_builds = ['fields_builds_example'] # List[str] | the fields to include for returned resources of type builds (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.build_beta_details_get_instance(id, fields_build_beta_details=fields_build_beta_details, fields_builds=fields_builds, include=include)
        print("The response of BuildBetaDetailsApi->build_beta_details_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildBetaDetailsApi->build_beta_details_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_build_beta_details** | [**List[str]**](str.md)| the fields to include for returned resources of type buildBetaDetails | [optional] 
 **fields_builds** | [**List[str]**](str.md)| the fields to include for returned resources of type builds | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**BuildBetaDetailResponse**](BuildBetaDetailResponse.md)

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
**200** | Single BuildBetaDetail |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **build_beta_details_update_instance**
> BuildBetaDetailResponse build_beta_details_update_instance(id, build_beta_detail_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_beta_detail_response import BuildBetaDetailResponse
from openapi_client.models.build_beta_detail_update_request import BuildBetaDetailUpdateRequest
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
    api_instance = openapi_client.BuildBetaDetailsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    build_beta_detail_update_request = openapi_client.BuildBetaDetailUpdateRequest() # BuildBetaDetailUpdateRequest | BuildBetaDetail representation

    try:
        api_response = api_instance.build_beta_details_update_instance(id, build_beta_detail_update_request)
        print("The response of BuildBetaDetailsApi->build_beta_details_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildBetaDetailsApi->build_beta_details_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **build_beta_detail_update_request** | [**BuildBetaDetailUpdateRequest**](BuildBetaDetailUpdateRequest.md)| BuildBetaDetail representation | 

### Return type

[**BuildBetaDetailResponse**](BuildBetaDetailResponse.md)

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
**200** | Single BuildBetaDetail |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

