# openapi_client.BuildsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**builds_app_encryption_declaration_get_to_one_related**](BuildsApi.md#builds_app_encryption_declaration_get_to_one_related) | **GET** /v1/builds/{id}/appEncryptionDeclaration | 
[**builds_app_encryption_declaration_get_to_one_relationship**](BuildsApi.md#builds_app_encryption_declaration_get_to_one_relationship) | **GET** /v1/builds/{id}/relationships/appEncryptionDeclaration | 
[**builds_app_encryption_declaration_update_to_one_relationship**](BuildsApi.md#builds_app_encryption_declaration_update_to_one_relationship) | **PATCH** /v1/builds/{id}/relationships/appEncryptionDeclaration | 
[**builds_app_get_to_one_related**](BuildsApi.md#builds_app_get_to_one_related) | **GET** /v1/builds/{id}/app | 
[**builds_app_get_to_one_relationship**](BuildsApi.md#builds_app_get_to_one_relationship) | **GET** /v1/builds/{id}/relationships/app | 
[**builds_app_store_version_get_to_one_related**](BuildsApi.md#builds_app_store_version_get_to_one_related) | **GET** /v1/builds/{id}/appStoreVersion | 
[**builds_app_store_version_get_to_one_relationship**](BuildsApi.md#builds_app_store_version_get_to_one_relationship) | **GET** /v1/builds/{id}/relationships/appStoreVersion | 
[**builds_beta_app_review_submission_get_to_one_related**](BuildsApi.md#builds_beta_app_review_submission_get_to_one_related) | **GET** /v1/builds/{id}/betaAppReviewSubmission | 
[**builds_beta_app_review_submission_get_to_one_relationship**](BuildsApi.md#builds_beta_app_review_submission_get_to_one_relationship) | **GET** /v1/builds/{id}/relationships/betaAppReviewSubmission | 
[**builds_beta_build_localizations_get_to_many_related**](BuildsApi.md#builds_beta_build_localizations_get_to_many_related) | **GET** /v1/builds/{id}/betaBuildLocalizations | 
[**builds_beta_build_localizations_get_to_many_relationship**](BuildsApi.md#builds_beta_build_localizations_get_to_many_relationship) | **GET** /v1/builds/{id}/relationships/betaBuildLocalizations | 
[**builds_beta_build_usages_get_metrics**](BuildsApi.md#builds_beta_build_usages_get_metrics) | **GET** /v1/builds/{id}/metrics/betaBuildUsages | 
[**builds_beta_groups_create_to_many_relationship**](BuildsApi.md#builds_beta_groups_create_to_many_relationship) | **POST** /v1/builds/{id}/relationships/betaGroups | 
[**builds_beta_groups_delete_to_many_relationship**](BuildsApi.md#builds_beta_groups_delete_to_many_relationship) | **DELETE** /v1/builds/{id}/relationships/betaGroups | 
[**builds_build_beta_detail_get_to_one_related**](BuildsApi.md#builds_build_beta_detail_get_to_one_related) | **GET** /v1/builds/{id}/buildBetaDetail | 
[**builds_build_beta_detail_get_to_one_relationship**](BuildsApi.md#builds_build_beta_detail_get_to_one_relationship) | **GET** /v1/builds/{id}/relationships/buildBetaDetail | 
[**builds_diagnostic_signatures_get_to_many_related**](BuildsApi.md#builds_diagnostic_signatures_get_to_many_related) | **GET** /v1/builds/{id}/diagnosticSignatures | 
[**builds_diagnostic_signatures_get_to_many_relationship**](BuildsApi.md#builds_diagnostic_signatures_get_to_many_relationship) | **GET** /v1/builds/{id}/relationships/diagnosticSignatures | 
[**builds_get_collection**](BuildsApi.md#builds_get_collection) | **GET** /v1/builds | 
[**builds_get_instance**](BuildsApi.md#builds_get_instance) | **GET** /v1/builds/{id} | 
[**builds_icons_get_to_many_related**](BuildsApi.md#builds_icons_get_to_many_related) | **GET** /v1/builds/{id}/icons | 
[**builds_icons_get_to_many_relationship**](BuildsApi.md#builds_icons_get_to_many_relationship) | **GET** /v1/builds/{id}/relationships/icons | 
[**builds_individual_testers_create_to_many_relationship**](BuildsApi.md#builds_individual_testers_create_to_many_relationship) | **POST** /v1/builds/{id}/relationships/individualTesters | 
[**builds_individual_testers_delete_to_many_relationship**](BuildsApi.md#builds_individual_testers_delete_to_many_relationship) | **DELETE** /v1/builds/{id}/relationships/individualTesters | 
[**builds_individual_testers_get_to_many_related**](BuildsApi.md#builds_individual_testers_get_to_many_related) | **GET** /v1/builds/{id}/individualTesters | 
[**builds_individual_testers_get_to_many_relationship**](BuildsApi.md#builds_individual_testers_get_to_many_relationship) | **GET** /v1/builds/{id}/relationships/individualTesters | 
[**builds_perf_power_metrics_get_to_many_related**](BuildsApi.md#builds_perf_power_metrics_get_to_many_related) | **GET** /v1/builds/{id}/perfPowerMetrics | 
[**builds_pre_release_version_get_to_one_related**](BuildsApi.md#builds_pre_release_version_get_to_one_related) | **GET** /v1/builds/{id}/preReleaseVersion | 
[**builds_pre_release_version_get_to_one_relationship**](BuildsApi.md#builds_pre_release_version_get_to_one_relationship) | **GET** /v1/builds/{id}/relationships/preReleaseVersion | 
[**builds_update_instance**](BuildsApi.md#builds_update_instance) | **PATCH** /v1/builds/{id} | 


# **builds_app_encryption_declaration_get_to_one_related**
> AppEncryptionDeclarationWithoutIncludesResponse builds_app_encryption_declaration_get_to_one_related(id, fields_app_encryption_declarations=fields_app_encryption_declarations)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_encryption_declaration_without_includes_response import AppEncryptionDeclarationWithoutIncludesResponse
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_encryption_declarations = ['fields_app_encryption_declarations_example'] # List[str] | the fields to include for returned resources of type appEncryptionDeclarations (optional)

    try:
        api_response = api_instance.builds_app_encryption_declaration_get_to_one_related(id, fields_app_encryption_declarations=fields_app_encryption_declarations)
        print("The response of BuildsApi->builds_app_encryption_declaration_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_app_encryption_declaration_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_encryption_declarations** | [**List[str]**](str.md)| the fields to include for returned resources of type appEncryptionDeclarations | [optional] 

### Return type

[**AppEncryptionDeclarationWithoutIncludesResponse**](AppEncryptionDeclarationWithoutIncludesResponse.md)

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
**200** | Single AppEncryptionDeclaration with get |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **builds_app_encryption_declaration_get_to_one_relationship**
> BuildAppEncryptionDeclarationLinkageResponse builds_app_encryption_declaration_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_app_encryption_declaration_linkage_response import BuildAppEncryptionDeclarationLinkageResponse
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.builds_app_encryption_declaration_get_to_one_relationship(id)
        print("The response of BuildsApi->builds_app_encryption_declaration_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_app_encryption_declaration_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**BuildAppEncryptionDeclarationLinkageResponse**](BuildAppEncryptionDeclarationLinkageResponse.md)

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

# **builds_app_encryption_declaration_update_to_one_relationship**
> builds_app_encryption_declaration_update_to_one_relationship(id, build_app_encryption_declaration_linkage_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_app_encryption_declaration_linkage_request import BuildAppEncryptionDeclarationLinkageRequest
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    build_app_encryption_declaration_linkage_request = openapi_client.BuildAppEncryptionDeclarationLinkageRequest() # BuildAppEncryptionDeclarationLinkageRequest | Related linkage

    try:
        api_instance.builds_app_encryption_declaration_update_to_one_relationship(id, build_app_encryption_declaration_linkage_request)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_app_encryption_declaration_update_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **build_app_encryption_declaration_linkage_request** | [**BuildAppEncryptionDeclarationLinkageRequest**](BuildAppEncryptionDeclarationLinkageRequest.md)| Related linkage | 

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**422** | Unprocessable request entity error(s) |  -  |
**409** | Request entity error(s) |  -  |
**204** | Success (no content) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **builds_app_get_to_one_related**
> AppWithoutIncludesResponse builds_app_get_to_one_related(id, fields_apps=fields_apps)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_without_includes_response import AppWithoutIncludesResponse
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_apps = ['fields_apps_example'] # List[str] | the fields to include for returned resources of type apps (optional)

    try:
        api_response = api_instance.builds_app_get_to_one_related(id, fields_apps=fields_apps)
        print("The response of BuildsApi->builds_app_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_app_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_apps** | [**List[str]**](str.md)| the fields to include for returned resources of type apps | [optional] 

### Return type

[**AppWithoutIncludesResponse**](AppWithoutIncludesResponse.md)

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
**200** | Single App with get |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **builds_app_get_to_one_relationship**
> BuildAppLinkageResponse builds_app_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_app_linkage_response import BuildAppLinkageResponse
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.builds_app_get_to_one_relationship(id)
        print("The response of BuildsApi->builds_app_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_app_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**BuildAppLinkageResponse**](BuildAppLinkageResponse.md)

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

# **builds_app_store_version_get_to_one_related**
> AppStoreVersionResponse builds_app_store_version_get_to_one_related(id, fields_app_store_versions=fields_app_store_versions, fields_apps=fields_apps, fields_age_rating_declarations=fields_age_rating_declarations, fields_app_store_version_localizations=fields_app_store_version_localizations, fields_builds=fields_builds, fields_app_store_version_phased_releases=fields_app_store_version_phased_releases, fields_game_center_app_versions=fields_game_center_app_versions, fields_routing_app_coverages=fields_routing_app_coverages, fields_app_store_review_details=fields_app_store_review_details, fields_app_store_version_submissions=fields_app_store_version_submissions, fields_app_clip_default_experiences=fields_app_clip_default_experiences, fields_app_store_version_experiments=fields_app_store_version_experiments, fields_alternative_distribution_packages=fields_alternative_distribution_packages, include=include, limit_app_store_version_localizations=limit_app_store_version_localizations, limit_app_store_version_experiments=limit_app_store_version_experiments, limit_app_store_version_experiments_v2=limit_app_store_version_experiments_v2)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_store_version_response import AppStoreVersionResponse
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_app_store_versions = ['fields_app_store_versions_example'] # List[str] | the fields to include for returned resources of type appStoreVersions (optional)
    fields_apps = ['fields_apps_example'] # List[str] | the fields to include for returned resources of type apps (optional)
    fields_age_rating_declarations = ['fields_age_rating_declarations_example'] # List[str] | the fields to include for returned resources of type ageRatingDeclarations (optional)
    fields_app_store_version_localizations = ['fields_app_store_version_localizations_example'] # List[str] | the fields to include for returned resources of type appStoreVersionLocalizations (optional)
    fields_builds = ['fields_builds_example'] # List[str] | the fields to include for returned resources of type builds (optional)
    fields_app_store_version_phased_releases = ['fields_app_store_version_phased_releases_example'] # List[str] | the fields to include for returned resources of type appStoreVersionPhasedReleases (optional)
    fields_game_center_app_versions = ['fields_game_center_app_versions_example'] # List[str] | the fields to include for returned resources of type gameCenterAppVersions (optional)
    fields_routing_app_coverages = ['fields_routing_app_coverages_example'] # List[str] | the fields to include for returned resources of type routingAppCoverages (optional)
    fields_app_store_review_details = ['fields_app_store_review_details_example'] # List[str] | the fields to include for returned resources of type appStoreReviewDetails (optional)
    fields_app_store_version_submissions = ['fields_app_store_version_submissions_example'] # List[str] | the fields to include for returned resources of type appStoreVersionSubmissions (optional)
    fields_app_clip_default_experiences = ['fields_app_clip_default_experiences_example'] # List[str] | the fields to include for returned resources of type appClipDefaultExperiences (optional)
    fields_app_store_version_experiments = ['fields_app_store_version_experiments_example'] # List[str] | the fields to include for returned resources of type appStoreVersionExperiments (optional)
    fields_alternative_distribution_packages = ['fields_alternative_distribution_packages_example'] # List[str] | the fields to include for returned resources of type alternativeDistributionPackages (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_store_version_localizations = 56 # int | maximum number of related appStoreVersionLocalizations returned (when they are included) (optional)
    limit_app_store_version_experiments = 56 # int | maximum number of related appStoreVersionExperiments returned (when they are included) (optional)
    limit_app_store_version_experiments_v2 = 56 # int | maximum number of related appStoreVersionExperimentsV2 returned (when they are included) (optional)

    try:
        api_response = api_instance.builds_app_store_version_get_to_one_related(id, fields_app_store_versions=fields_app_store_versions, fields_apps=fields_apps, fields_age_rating_declarations=fields_age_rating_declarations, fields_app_store_version_localizations=fields_app_store_version_localizations, fields_builds=fields_builds, fields_app_store_version_phased_releases=fields_app_store_version_phased_releases, fields_game_center_app_versions=fields_game_center_app_versions, fields_routing_app_coverages=fields_routing_app_coverages, fields_app_store_review_details=fields_app_store_review_details, fields_app_store_version_submissions=fields_app_store_version_submissions, fields_app_clip_default_experiences=fields_app_clip_default_experiences, fields_app_store_version_experiments=fields_app_store_version_experiments, fields_alternative_distribution_packages=fields_alternative_distribution_packages, include=include, limit_app_store_version_localizations=limit_app_store_version_localizations, limit_app_store_version_experiments=limit_app_store_version_experiments, limit_app_store_version_experiments_v2=limit_app_store_version_experiments_v2)
        print("The response of BuildsApi->builds_app_store_version_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_app_store_version_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_app_store_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersions | [optional] 
 **fields_apps** | [**List[str]**](str.md)| the fields to include for returned resources of type apps | [optional] 
 **fields_age_rating_declarations** | [**List[str]**](str.md)| the fields to include for returned resources of type ageRatingDeclarations | [optional] 
 **fields_app_store_version_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionLocalizations | [optional] 
 **fields_builds** | [**List[str]**](str.md)| the fields to include for returned resources of type builds | [optional] 
 **fields_app_store_version_phased_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionPhasedReleases | [optional] 
 **fields_game_center_app_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAppVersions | [optional] 
 **fields_routing_app_coverages** | [**List[str]**](str.md)| the fields to include for returned resources of type routingAppCoverages | [optional] 
 **fields_app_store_review_details** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreReviewDetails | [optional] 
 **fields_app_store_version_submissions** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionSubmissions | [optional] 
 **fields_app_clip_default_experiences** | [**List[str]**](str.md)| the fields to include for returned resources of type appClipDefaultExperiences | [optional] 
 **fields_app_store_version_experiments** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionExperiments | [optional] 
 **fields_alternative_distribution_packages** | [**List[str]**](str.md)| the fields to include for returned resources of type alternativeDistributionPackages | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_store_version_localizations** | **int**| maximum number of related appStoreVersionLocalizations returned (when they are included) | [optional] 
 **limit_app_store_version_experiments** | **int**| maximum number of related appStoreVersionExperiments returned (when they are included) | [optional] 
 **limit_app_store_version_experiments_v2** | **int**| maximum number of related appStoreVersionExperimentsV2 returned (when they are included) | [optional] 

### Return type

[**AppStoreVersionResponse**](AppStoreVersionResponse.md)

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
**200** | Single AppStoreVersion |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **builds_app_store_version_get_to_one_relationship**
> BuildAppStoreVersionLinkageResponse builds_app_store_version_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_app_store_version_linkage_response import BuildAppStoreVersionLinkageResponse
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.builds_app_store_version_get_to_one_relationship(id)
        print("The response of BuildsApi->builds_app_store_version_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_app_store_version_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**BuildAppStoreVersionLinkageResponse**](BuildAppStoreVersionLinkageResponse.md)

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

# **builds_beta_app_review_submission_get_to_one_related**
> BetaAppReviewSubmissionWithoutIncludesResponse builds_beta_app_review_submission_get_to_one_related(id, fields_beta_app_review_submissions=fields_beta_app_review_submissions)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.beta_app_review_submission_without_includes_response import BetaAppReviewSubmissionWithoutIncludesResponse
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_beta_app_review_submissions = ['fields_beta_app_review_submissions_example'] # List[str] | the fields to include for returned resources of type betaAppReviewSubmissions (optional)

    try:
        api_response = api_instance.builds_beta_app_review_submission_get_to_one_related(id, fields_beta_app_review_submissions=fields_beta_app_review_submissions)
        print("The response of BuildsApi->builds_beta_app_review_submission_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_beta_app_review_submission_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_beta_app_review_submissions** | [**List[str]**](str.md)| the fields to include for returned resources of type betaAppReviewSubmissions | [optional] 

### Return type

[**BetaAppReviewSubmissionWithoutIncludesResponse**](BetaAppReviewSubmissionWithoutIncludesResponse.md)

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
**200** | Single BetaAppReviewSubmission with get |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **builds_beta_app_review_submission_get_to_one_relationship**
> BuildBetaAppReviewSubmissionLinkageResponse builds_beta_app_review_submission_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_beta_app_review_submission_linkage_response import BuildBetaAppReviewSubmissionLinkageResponse
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.builds_beta_app_review_submission_get_to_one_relationship(id)
        print("The response of BuildsApi->builds_beta_app_review_submission_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_beta_app_review_submission_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**BuildBetaAppReviewSubmissionLinkageResponse**](BuildBetaAppReviewSubmissionLinkageResponse.md)

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

# **builds_beta_build_localizations_get_to_many_related**
> BetaBuildLocalizationsWithoutIncludesResponse builds_beta_build_localizations_get_to_many_related(id, fields_beta_build_localizations=fields_beta_build_localizations, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.beta_build_localizations_without_includes_response import BetaBuildLocalizationsWithoutIncludesResponse
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_beta_build_localizations = ['fields_beta_build_localizations_example'] # List[str] | the fields to include for returned resources of type betaBuildLocalizations (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.builds_beta_build_localizations_get_to_many_related(id, fields_beta_build_localizations=fields_beta_build_localizations, limit=limit)
        print("The response of BuildsApi->builds_beta_build_localizations_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_beta_build_localizations_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_beta_build_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type betaBuildLocalizations | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**BetaBuildLocalizationsWithoutIncludesResponse**](BetaBuildLocalizationsWithoutIncludesResponse.md)

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
**200** | List of BetaBuildLocalizations with get |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **builds_beta_build_localizations_get_to_many_relationship**
> BuildBetaBuildLocalizationsLinkagesResponse builds_beta_build_localizations_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_beta_build_localizations_linkages_response import BuildBetaBuildLocalizationsLinkagesResponse
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.builds_beta_build_localizations_get_to_many_relationship(id, limit=limit)
        print("The response of BuildsApi->builds_beta_build_localizations_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_beta_build_localizations_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**BuildBetaBuildLocalizationsLinkagesResponse**](BuildBetaBuildLocalizationsLinkagesResponse.md)

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

# **builds_beta_build_usages_get_metrics**
> BetaBuildUsagesV1MetricResponse builds_beta_build_usages_get_metrics(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.beta_build_usages_v1_metric_response import BetaBuildUsagesV1MetricResponse
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.builds_beta_build_usages_get_metrics(id, limit=limit)
        print("The response of BuildsApi->builds_beta_build_usages_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_beta_build_usages_get_metrics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum number of groups to return per page | [optional] 

### Return type

[**BetaBuildUsagesV1MetricResponse**](BetaBuildUsagesV1MetricResponse.md)

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
**200** | Metrics data response |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **builds_beta_groups_create_to_many_relationship**
> builds_beta_groups_create_to_many_relationship(id, build_beta_groups_linkages_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_beta_groups_linkages_request import BuildBetaGroupsLinkagesRequest
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    build_beta_groups_linkages_request = openapi_client.BuildBetaGroupsLinkagesRequest() # BuildBetaGroupsLinkagesRequest | List of related linkages

    try:
        api_instance.builds_beta_groups_create_to_many_relationship(id, build_beta_groups_linkages_request)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_beta_groups_create_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **build_beta_groups_linkages_request** | [**BuildBetaGroupsLinkagesRequest**](BuildBetaGroupsLinkagesRequest.md)| List of related linkages | 

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**422** | Unprocessable request entity error(s) |  -  |
**409** | Request entity error(s) |  -  |
**204** | Success (no content) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **builds_beta_groups_delete_to_many_relationship**
> builds_beta_groups_delete_to_many_relationship(id, build_beta_groups_linkages_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_beta_groups_linkages_request import BuildBetaGroupsLinkagesRequest
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    build_beta_groups_linkages_request = openapi_client.BuildBetaGroupsLinkagesRequest() # BuildBetaGroupsLinkagesRequest | List of related linkages

    try:
        api_instance.builds_beta_groups_delete_to_many_relationship(id, build_beta_groups_linkages_request)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_beta_groups_delete_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **build_beta_groups_linkages_request** | [**BuildBetaGroupsLinkagesRequest**](BuildBetaGroupsLinkagesRequest.md)| List of related linkages | 

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**422** | Unprocessable request entity error(s) |  -  |
**409** | Request entity error(s) |  -  |
**204** | Success (no content) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **builds_build_beta_detail_get_to_one_related**
> BuildBetaDetailResponse builds_build_beta_detail_get_to_one_related(id, fields_build_beta_details=fields_build_beta_details, fields_builds=fields_builds, include=include)

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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_build_beta_details = ['fields_build_beta_details_example'] # List[str] | the fields to include for returned resources of type buildBetaDetails (optional)
    fields_builds = ['fields_builds_example'] # List[str] | the fields to include for returned resources of type builds (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.builds_build_beta_detail_get_to_one_related(id, fields_build_beta_details=fields_build_beta_details, fields_builds=fields_builds, include=include)
        print("The response of BuildsApi->builds_build_beta_detail_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_build_beta_detail_get_to_one_related: %s\n" % e)
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

# **builds_build_beta_detail_get_to_one_relationship**
> BuildBuildBetaDetailLinkageResponse builds_build_beta_detail_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_build_beta_detail_linkage_response import BuildBuildBetaDetailLinkageResponse
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.builds_build_beta_detail_get_to_one_relationship(id)
        print("The response of BuildsApi->builds_build_beta_detail_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_build_beta_detail_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**BuildBuildBetaDetailLinkageResponse**](BuildBuildBetaDetailLinkageResponse.md)

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

# **builds_diagnostic_signatures_get_to_many_related**
> DiagnosticSignaturesResponse builds_diagnostic_signatures_get_to_many_related(id, filter_diagnostic_type=filter_diagnostic_type, fields_diagnostic_signatures=fields_diagnostic_signatures, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.diagnostic_signatures_response import DiagnosticSignaturesResponse
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_diagnostic_type = ['filter_diagnostic_type_example'] # List[str] | filter by attribute 'diagnosticType' (optional)
    fields_diagnostic_signatures = ['fields_diagnostic_signatures_example'] # List[str] | the fields to include for returned resources of type diagnosticSignatures (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.builds_diagnostic_signatures_get_to_many_related(id, filter_diagnostic_type=filter_diagnostic_type, fields_diagnostic_signatures=fields_diagnostic_signatures, limit=limit)
        print("The response of BuildsApi->builds_diagnostic_signatures_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_diagnostic_signatures_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_diagnostic_type** | [**List[str]**](str.md)| filter by attribute &#39;diagnosticType&#39; | [optional] 
 **fields_diagnostic_signatures** | [**List[str]**](str.md)| the fields to include for returned resources of type diagnosticSignatures | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**DiagnosticSignaturesResponse**](DiagnosticSignaturesResponse.md)

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
**200** | List of DiagnosticSignatures |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **builds_diagnostic_signatures_get_to_many_relationship**
> BuildDiagnosticSignaturesLinkagesResponse builds_diagnostic_signatures_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_diagnostic_signatures_linkages_response import BuildDiagnosticSignaturesLinkagesResponse
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.builds_diagnostic_signatures_get_to_many_relationship(id, limit=limit)
        print("The response of BuildsApi->builds_diagnostic_signatures_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_diagnostic_signatures_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**BuildDiagnosticSignaturesLinkagesResponse**](BuildDiagnosticSignaturesLinkagesResponse.md)

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

# **builds_get_collection**
> BuildsResponse builds_get_collection(filter_version=filter_version, filter_expired=filter_expired, filter_processing_state=filter_processing_state, filter_beta_app_review_submission_beta_review_state=filter_beta_app_review_submission_beta_review_state, filter_uses_non_exempt_encryption=filter_uses_non_exempt_encryption, filter_pre_release_version_version=filter_pre_release_version_version, filter_pre_release_version_platform=filter_pre_release_version_platform, filter_build_audience_type=filter_build_audience_type, filter_pre_release_version=filter_pre_release_version, filter_app=filter_app, filter_beta_groups=filter_beta_groups, filter_app_store_version=filter_app_store_version, filter_id=filter_id, exists_uses_non_exempt_encryption=exists_uses_non_exempt_encryption, sort=sort, fields_builds=fields_builds, fields_pre_release_versions=fields_pre_release_versions, fields_beta_testers=fields_beta_testers, fields_beta_build_localizations=fields_beta_build_localizations, fields_app_encryption_declarations=fields_app_encryption_declarations, fields_beta_app_review_submissions=fields_beta_app_review_submissions, fields_apps=fields_apps, fields_build_beta_details=fields_build_beta_details, fields_app_store_versions=fields_app_store_versions, fields_build_icons=fields_build_icons, limit=limit, include=include, limit_beta_build_localizations=limit_beta_build_localizations, limit_beta_groups=limit_beta_groups, limit_build_bundles=limit_build_bundles, limit_icons=limit_icons, limit_individual_testers=limit_individual_testers)

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
    api_instance = openapi_client.BuildsApi(api_client)
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
    fields_beta_build_localizations = ['fields_beta_build_localizations_example'] # List[str] | the fields to include for returned resources of type betaBuildLocalizations (optional)
    fields_app_encryption_declarations = ['fields_app_encryption_declarations_example'] # List[str] | the fields to include for returned resources of type appEncryptionDeclarations (optional)
    fields_beta_app_review_submissions = ['fields_beta_app_review_submissions_example'] # List[str] | the fields to include for returned resources of type betaAppReviewSubmissions (optional)
    fields_apps = ['fields_apps_example'] # List[str] | the fields to include for returned resources of type apps (optional)
    fields_build_beta_details = ['fields_build_beta_details_example'] # List[str] | the fields to include for returned resources of type buildBetaDetails (optional)
    fields_app_store_versions = ['fields_app_store_versions_example'] # List[str] | the fields to include for returned resources of type appStoreVersions (optional)
    fields_build_icons = ['fields_build_icons_example'] # List[str] | the fields to include for returned resources of type buildIcons (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_beta_build_localizations = 56 # int | maximum number of related betaBuildLocalizations returned (when they are included) (optional)
    limit_beta_groups = 56 # int | maximum number of related betaGroups returned (when they are included) (optional)
    limit_build_bundles = 56 # int | maximum number of related buildBundles returned (when they are included) (optional)
    limit_icons = 56 # int | maximum number of related icons returned (when they are included) (optional)
    limit_individual_testers = 56 # int | maximum number of related individualTesters returned (when they are included) (optional)

    try:
        api_response = api_instance.builds_get_collection(filter_version=filter_version, filter_expired=filter_expired, filter_processing_state=filter_processing_state, filter_beta_app_review_submission_beta_review_state=filter_beta_app_review_submission_beta_review_state, filter_uses_non_exempt_encryption=filter_uses_non_exempt_encryption, filter_pre_release_version_version=filter_pre_release_version_version, filter_pre_release_version_platform=filter_pre_release_version_platform, filter_build_audience_type=filter_build_audience_type, filter_pre_release_version=filter_pre_release_version, filter_app=filter_app, filter_beta_groups=filter_beta_groups, filter_app_store_version=filter_app_store_version, filter_id=filter_id, exists_uses_non_exempt_encryption=exists_uses_non_exempt_encryption, sort=sort, fields_builds=fields_builds, fields_pre_release_versions=fields_pre_release_versions, fields_beta_testers=fields_beta_testers, fields_beta_build_localizations=fields_beta_build_localizations, fields_app_encryption_declarations=fields_app_encryption_declarations, fields_beta_app_review_submissions=fields_beta_app_review_submissions, fields_apps=fields_apps, fields_build_beta_details=fields_build_beta_details, fields_app_store_versions=fields_app_store_versions, fields_build_icons=fields_build_icons, limit=limit, include=include, limit_beta_build_localizations=limit_beta_build_localizations, limit_beta_groups=limit_beta_groups, limit_build_bundles=limit_build_bundles, limit_icons=limit_icons, limit_individual_testers=limit_individual_testers)
        print("The response of BuildsApi->builds_get_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_get_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
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
 **fields_beta_build_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type betaBuildLocalizations | [optional] 
 **fields_app_encryption_declarations** | [**List[str]**](str.md)| the fields to include for returned resources of type appEncryptionDeclarations | [optional] 
 **fields_beta_app_review_submissions** | [**List[str]**](str.md)| the fields to include for returned resources of type betaAppReviewSubmissions | [optional] 
 **fields_apps** | [**List[str]**](str.md)| the fields to include for returned resources of type apps | [optional] 
 **fields_build_beta_details** | [**List[str]**](str.md)| the fields to include for returned resources of type buildBetaDetails | [optional] 
 **fields_app_store_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersions | [optional] 
 **fields_build_icons** | [**List[str]**](str.md)| the fields to include for returned resources of type buildIcons | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_beta_build_localizations** | **int**| maximum number of related betaBuildLocalizations returned (when they are included) | [optional] 
 **limit_beta_groups** | **int**| maximum number of related betaGroups returned (when they are included) | [optional] 
 **limit_build_bundles** | **int**| maximum number of related buildBundles returned (when they are included) | [optional] 
 **limit_icons** | **int**| maximum number of related icons returned (when they are included) | [optional] 
 **limit_individual_testers** | **int**| maximum number of related individualTesters returned (when they are included) | [optional] 

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
**200** | List of Builds |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **builds_get_instance**
> BuildResponse builds_get_instance(id, fields_builds=fields_builds, fields_pre_release_versions=fields_pre_release_versions, fields_beta_testers=fields_beta_testers, fields_beta_build_localizations=fields_beta_build_localizations, fields_app_encryption_declarations=fields_app_encryption_declarations, fields_beta_app_review_submissions=fields_beta_app_review_submissions, fields_apps=fields_apps, fields_build_beta_details=fields_build_beta_details, fields_app_store_versions=fields_app_store_versions, fields_build_icons=fields_build_icons, include=include, limit_beta_build_localizations=limit_beta_build_localizations, limit_beta_groups=limit_beta_groups, limit_build_bundles=limit_build_bundles, limit_icons=limit_icons, limit_individual_testers=limit_individual_testers)

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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_builds = ['fields_builds_example'] # List[str] | the fields to include for returned resources of type builds (optional)
    fields_pre_release_versions = ['fields_pre_release_versions_example'] # List[str] | the fields to include for returned resources of type preReleaseVersions (optional)
    fields_beta_testers = ['fields_beta_testers_example'] # List[str] | the fields to include for returned resources of type betaTesters (optional)
    fields_beta_build_localizations = ['fields_beta_build_localizations_example'] # List[str] | the fields to include for returned resources of type betaBuildLocalizations (optional)
    fields_app_encryption_declarations = ['fields_app_encryption_declarations_example'] # List[str] | the fields to include for returned resources of type appEncryptionDeclarations (optional)
    fields_beta_app_review_submissions = ['fields_beta_app_review_submissions_example'] # List[str] | the fields to include for returned resources of type betaAppReviewSubmissions (optional)
    fields_apps = ['fields_apps_example'] # List[str] | the fields to include for returned resources of type apps (optional)
    fields_build_beta_details = ['fields_build_beta_details_example'] # List[str] | the fields to include for returned resources of type buildBetaDetails (optional)
    fields_app_store_versions = ['fields_app_store_versions_example'] # List[str] | the fields to include for returned resources of type appStoreVersions (optional)
    fields_build_icons = ['fields_build_icons_example'] # List[str] | the fields to include for returned resources of type buildIcons (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_beta_build_localizations = 56 # int | maximum number of related betaBuildLocalizations returned (when they are included) (optional)
    limit_beta_groups = 56 # int | maximum number of related betaGroups returned (when they are included) (optional)
    limit_build_bundles = 56 # int | maximum number of related buildBundles returned (when they are included) (optional)
    limit_icons = 56 # int | maximum number of related icons returned (when they are included) (optional)
    limit_individual_testers = 56 # int | maximum number of related individualTesters returned (when they are included) (optional)

    try:
        api_response = api_instance.builds_get_instance(id, fields_builds=fields_builds, fields_pre_release_versions=fields_pre_release_versions, fields_beta_testers=fields_beta_testers, fields_beta_build_localizations=fields_beta_build_localizations, fields_app_encryption_declarations=fields_app_encryption_declarations, fields_beta_app_review_submissions=fields_beta_app_review_submissions, fields_apps=fields_apps, fields_build_beta_details=fields_build_beta_details, fields_app_store_versions=fields_app_store_versions, fields_build_icons=fields_build_icons, include=include, limit_beta_build_localizations=limit_beta_build_localizations, limit_beta_groups=limit_beta_groups, limit_build_bundles=limit_build_bundles, limit_icons=limit_icons, limit_individual_testers=limit_individual_testers)
        print("The response of BuildsApi->builds_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_builds** | [**List[str]**](str.md)| the fields to include for returned resources of type builds | [optional] 
 **fields_pre_release_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type preReleaseVersions | [optional] 
 **fields_beta_testers** | [**List[str]**](str.md)| the fields to include for returned resources of type betaTesters | [optional] 
 **fields_beta_build_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type betaBuildLocalizations | [optional] 
 **fields_app_encryption_declarations** | [**List[str]**](str.md)| the fields to include for returned resources of type appEncryptionDeclarations | [optional] 
 **fields_beta_app_review_submissions** | [**List[str]**](str.md)| the fields to include for returned resources of type betaAppReviewSubmissions | [optional] 
 **fields_apps** | [**List[str]**](str.md)| the fields to include for returned resources of type apps | [optional] 
 **fields_build_beta_details** | [**List[str]**](str.md)| the fields to include for returned resources of type buildBetaDetails | [optional] 
 **fields_app_store_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersions | [optional] 
 **fields_build_icons** | [**List[str]**](str.md)| the fields to include for returned resources of type buildIcons | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_beta_build_localizations** | **int**| maximum number of related betaBuildLocalizations returned (when they are included) | [optional] 
 **limit_beta_groups** | **int**| maximum number of related betaGroups returned (when they are included) | [optional] 
 **limit_build_bundles** | **int**| maximum number of related buildBundles returned (when they are included) | [optional] 
 **limit_icons** | **int**| maximum number of related icons returned (when they are included) | [optional] 
 **limit_individual_testers** | **int**| maximum number of related individualTesters returned (when they are included) | [optional] 

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

# **builds_icons_get_to_many_related**
> BuildIconsWithoutIncludesResponse builds_icons_get_to_many_related(id, fields_build_icons=fields_build_icons, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_icons_without_includes_response import BuildIconsWithoutIncludesResponse
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_build_icons = ['fields_build_icons_example'] # List[str] | the fields to include for returned resources of type buildIcons (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.builds_icons_get_to_many_related(id, fields_build_icons=fields_build_icons, limit=limit)
        print("The response of BuildsApi->builds_icons_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_icons_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_build_icons** | [**List[str]**](str.md)| the fields to include for returned resources of type buildIcons | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**BuildIconsWithoutIncludesResponse**](BuildIconsWithoutIncludesResponse.md)

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
**200** | List of BuildIcons with get |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **builds_icons_get_to_many_relationship**
> BuildIconsLinkagesResponse builds_icons_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_icons_linkages_response import BuildIconsLinkagesResponse
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.builds_icons_get_to_many_relationship(id, limit=limit)
        print("The response of BuildsApi->builds_icons_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_icons_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**BuildIconsLinkagesResponse**](BuildIconsLinkagesResponse.md)

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

# **builds_individual_testers_create_to_many_relationship**
> builds_individual_testers_create_to_many_relationship(id, build_individual_testers_linkages_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_individual_testers_linkages_request import BuildIndividualTestersLinkagesRequest
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    build_individual_testers_linkages_request = openapi_client.BuildIndividualTestersLinkagesRequest() # BuildIndividualTestersLinkagesRequest | List of related linkages

    try:
        api_instance.builds_individual_testers_create_to_many_relationship(id, build_individual_testers_linkages_request)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_individual_testers_create_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **build_individual_testers_linkages_request** | [**BuildIndividualTestersLinkagesRequest**](BuildIndividualTestersLinkagesRequest.md)| List of related linkages | 

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**422** | Unprocessable request entity error(s) |  -  |
**409** | Request entity error(s) |  -  |
**204** | Success (no content) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **builds_individual_testers_delete_to_many_relationship**
> builds_individual_testers_delete_to_many_relationship(id, build_individual_testers_linkages_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_individual_testers_linkages_request import BuildIndividualTestersLinkagesRequest
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    build_individual_testers_linkages_request = openapi_client.BuildIndividualTestersLinkagesRequest() # BuildIndividualTestersLinkagesRequest | List of related linkages

    try:
        api_instance.builds_individual_testers_delete_to_many_relationship(id, build_individual_testers_linkages_request)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_individual_testers_delete_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **build_individual_testers_linkages_request** | [**BuildIndividualTestersLinkagesRequest**](BuildIndividualTestersLinkagesRequest.md)| List of related linkages | 

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**422** | Unprocessable request entity error(s) |  -  |
**409** | Request entity error(s) |  -  |
**204** | Success (no content) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **builds_individual_testers_get_to_many_related**
> BetaTestersWithoutIncludesResponse builds_individual_testers_get_to_many_related(id, fields_beta_testers=fields_beta_testers, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.beta_testers_without_includes_response import BetaTestersWithoutIncludesResponse
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_beta_testers = ['fields_beta_testers_example'] # List[str] | the fields to include for returned resources of type betaTesters (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.builds_individual_testers_get_to_many_related(id, fields_beta_testers=fields_beta_testers, limit=limit)
        print("The response of BuildsApi->builds_individual_testers_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_individual_testers_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_beta_testers** | [**List[str]**](str.md)| the fields to include for returned resources of type betaTesters | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**BetaTestersWithoutIncludesResponse**](BetaTestersWithoutIncludesResponse.md)

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
**200** | List of BetaTesters with get |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **builds_individual_testers_get_to_many_relationship**
> BuildIndividualTestersLinkagesResponse builds_individual_testers_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_individual_testers_linkages_response import BuildIndividualTestersLinkagesResponse
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.builds_individual_testers_get_to_many_relationship(id, limit=limit)
        print("The response of BuildsApi->builds_individual_testers_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_individual_testers_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**BuildIndividualTestersLinkagesResponse**](BuildIndividualTestersLinkagesResponse.md)

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

# **builds_perf_power_metrics_get_to_many_related**
> XcodeMetrics builds_perf_power_metrics_get_to_many_related(id, filter_platform=filter_platform, filter_metric_type=filter_metric_type, filter_device_type=filter_device_type)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.xcode_metrics import XcodeMetrics
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_platform = ['filter_platform_example'] # List[str] | filter by attribute 'platform' (optional)
    filter_metric_type = ['filter_metric_type_example'] # List[str] | filter by attribute 'metricType' (optional)
    filter_device_type = ['filter_device_type_example'] # List[str] | filter by attribute 'deviceType' (optional)

    try:
        api_response = api_instance.builds_perf_power_metrics_get_to_many_related(id, filter_platform=filter_platform, filter_metric_type=filter_metric_type, filter_device_type=filter_device_type)
        print("The response of BuildsApi->builds_perf_power_metrics_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_perf_power_metrics_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_platform** | [**List[str]**](str.md)| filter by attribute &#39;platform&#39; | [optional] 
 **filter_metric_type** | [**List[str]**](str.md)| filter by attribute &#39;metricType&#39; | [optional] 
 **filter_device_type** | [**List[str]**](str.md)| filter by attribute &#39;deviceType&#39; | [optional] 

### Return type

[**XcodeMetrics**](XcodeMetrics.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, application/vnd.apple.xcode-metrics+json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of PerfPowerMetrics |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **builds_pre_release_version_get_to_one_related**
> PrereleaseVersionWithoutIncludesResponse builds_pre_release_version_get_to_one_related(id, fields_pre_release_versions=fields_pre_release_versions)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.prerelease_version_without_includes_response import PrereleaseVersionWithoutIncludesResponse
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_pre_release_versions = ['fields_pre_release_versions_example'] # List[str] | the fields to include for returned resources of type preReleaseVersions (optional)

    try:
        api_response = api_instance.builds_pre_release_version_get_to_one_related(id, fields_pre_release_versions=fields_pre_release_versions)
        print("The response of BuildsApi->builds_pre_release_version_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_pre_release_version_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_pre_release_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type preReleaseVersions | [optional] 

### Return type

[**PrereleaseVersionWithoutIncludesResponse**](PrereleaseVersionWithoutIncludesResponse.md)

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
**200** | Single PrereleaseVersion with get |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **builds_pre_release_version_get_to_one_relationship**
> BuildPreReleaseVersionLinkageResponse builds_pre_release_version_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_pre_release_version_linkage_response import BuildPreReleaseVersionLinkageResponse
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.builds_pre_release_version_get_to_one_relationship(id)
        print("The response of BuildsApi->builds_pre_release_version_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_pre_release_version_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**BuildPreReleaseVersionLinkageResponse**](BuildPreReleaseVersionLinkageResponse.md)

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

# **builds_update_instance**
> BuildResponse builds_update_instance(id, build_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.build_response import BuildResponse
from openapi_client.models.build_update_request import BuildUpdateRequest
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
    api_instance = openapi_client.BuildsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    build_update_request = openapi_client.BuildUpdateRequest() # BuildUpdateRequest | Build representation

    try:
        api_response = api_instance.builds_update_instance(id, build_update_request)
        print("The response of BuildsApi->builds_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildsApi->builds_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **build_update_request** | [**BuildUpdateRequest**](BuildUpdateRequest.md)| Build representation | 

### Return type

[**BuildResponse**](BuildResponse.md)

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
**200** | Single Build |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

