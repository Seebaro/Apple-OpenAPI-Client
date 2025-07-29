# openapi_client.CiProductsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ci_products_additional_repositories_get_to_many_related**](CiProductsApi.md#ci_products_additional_repositories_get_to_many_related) | **GET** /v1/ciProducts/{id}/additionalRepositories | 
[**ci_products_additional_repositories_get_to_many_relationship**](CiProductsApi.md#ci_products_additional_repositories_get_to_many_relationship) | **GET** /v1/ciProducts/{id}/relationships/additionalRepositories | 
[**ci_products_app_get_to_one_related**](CiProductsApi.md#ci_products_app_get_to_one_related) | **GET** /v1/ciProducts/{id}/app | 
[**ci_products_app_get_to_one_relationship**](CiProductsApi.md#ci_products_app_get_to_one_relationship) | **GET** /v1/ciProducts/{id}/relationships/app | 
[**ci_products_build_runs_get_to_many_related**](CiProductsApi.md#ci_products_build_runs_get_to_many_related) | **GET** /v1/ciProducts/{id}/buildRuns | 
[**ci_products_build_runs_get_to_many_relationship**](CiProductsApi.md#ci_products_build_runs_get_to_many_relationship) | **GET** /v1/ciProducts/{id}/relationships/buildRuns | 
[**ci_products_delete_instance**](CiProductsApi.md#ci_products_delete_instance) | **DELETE** /v1/ciProducts/{id} | 
[**ci_products_get_collection**](CiProductsApi.md#ci_products_get_collection) | **GET** /v1/ciProducts | 
[**ci_products_get_instance**](CiProductsApi.md#ci_products_get_instance) | **GET** /v1/ciProducts/{id} | 
[**ci_products_primary_repositories_get_to_many_related**](CiProductsApi.md#ci_products_primary_repositories_get_to_many_related) | **GET** /v1/ciProducts/{id}/primaryRepositories | 
[**ci_products_primary_repositories_get_to_many_relationship**](CiProductsApi.md#ci_products_primary_repositories_get_to_many_relationship) | **GET** /v1/ciProducts/{id}/relationships/primaryRepositories | 
[**ci_products_workflows_get_to_many_related**](CiProductsApi.md#ci_products_workflows_get_to_many_related) | **GET** /v1/ciProducts/{id}/workflows | 
[**ci_products_workflows_get_to_many_relationship**](CiProductsApi.md#ci_products_workflows_get_to_many_relationship) | **GET** /v1/ciProducts/{id}/relationships/workflows | 


# **ci_products_additional_repositories_get_to_many_related**
> ScmRepositoriesResponse ci_products_additional_repositories_get_to_many_related(id, filter_id=filter_id, fields_scm_repositories=fields_scm_repositories, fields_scm_providers=fields_scm_providers, fields_scm_git_references=fields_scm_git_references, limit=limit, include=include)

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
    api_instance = openapi_client.CiProductsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_id = ['filter_id_example'] # List[str] | filter by id(s) (optional)
    fields_scm_repositories = ['fields_scm_repositories_example'] # List[str] | the fields to include for returned resources of type scmRepositories (optional)
    fields_scm_providers = ['fields_scm_providers_example'] # List[str] | the fields to include for returned resources of type scmProviders (optional)
    fields_scm_git_references = ['fields_scm_git_references_example'] # List[str] | the fields to include for returned resources of type scmGitReferences (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.ci_products_additional_repositories_get_to_many_related(id, filter_id=filter_id, fields_scm_repositories=fields_scm_repositories, fields_scm_providers=fields_scm_providers, fields_scm_git_references=fields_scm_git_references, limit=limit, include=include)
        print("The response of CiProductsApi->ci_products_additional_repositories_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiProductsApi->ci_products_additional_repositories_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_id** | [**List[str]**](str.md)| filter by id(s) | [optional] 
 **fields_scm_repositories** | [**List[str]**](str.md)| the fields to include for returned resources of type scmRepositories | [optional] 
 **fields_scm_providers** | [**List[str]**](str.md)| the fields to include for returned resources of type scmProviders | [optional] 
 **fields_scm_git_references** | [**List[str]**](str.md)| the fields to include for returned resources of type scmGitReferences | [optional] 
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
**404** | Not found error |  -  |
**200** | List of ScmRepositories |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_products_additional_repositories_get_to_many_relationship**
> CiProductAdditionalRepositoriesLinkagesResponse ci_products_additional_repositories_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_product_additional_repositories_linkages_response import CiProductAdditionalRepositoriesLinkagesResponse
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
    api_instance = openapi_client.CiProductsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.ci_products_additional_repositories_get_to_many_relationship(id, limit=limit)
        print("The response of CiProductsApi->ci_products_additional_repositories_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiProductsApi->ci_products_additional_repositories_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**CiProductAdditionalRepositoriesLinkagesResponse**](CiProductAdditionalRepositoriesLinkagesResponse.md)

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

# **ci_products_app_get_to_one_related**
> AppResponse ci_products_app_get_to_one_related(id, fields_apps=fields_apps, fields_app_encryption_declarations=fields_app_encryption_declarations, fields_ci_products=fields_ci_products, fields_beta_groups=fields_beta_groups, fields_app_store_versions=fields_app_store_versions, fields_pre_release_versions=fields_pre_release_versions, fields_beta_app_localizations=fields_beta_app_localizations, fields_builds=fields_builds, fields_beta_license_agreements=fields_beta_license_agreements, fields_beta_app_review_details=fields_beta_app_review_details, fields_app_infos=fields_app_infos, fields_app_clips=fields_app_clips, fields_end_user_license_agreements=fields_end_user_license_agreements, fields_in_app_purchases=fields_in_app_purchases, fields_subscription_groups=fields_subscription_groups, fields_game_center_enabled_versions=fields_game_center_enabled_versions, fields_app_custom_product_pages=fields_app_custom_product_pages, fields_promoted_purchases=fields_promoted_purchases, fields_app_events=fields_app_events, fields_review_submissions=fields_review_submissions, fields_subscription_grace_periods=fields_subscription_grace_periods, fields_game_center_details=fields_game_center_details, fields_app_store_version_experiments=fields_app_store_version_experiments, include=include, limit_app_encryption_declarations=limit_app_encryption_declarations, limit_beta_groups=limit_beta_groups, limit_app_store_versions=limit_app_store_versions, limit_pre_release_versions=limit_pre_release_versions, limit_beta_app_localizations=limit_beta_app_localizations, limit_builds=limit_builds, limit_app_infos=limit_app_infos, limit_app_clips=limit_app_clips, limit_in_app_purchases=limit_in_app_purchases, limit_subscription_groups=limit_subscription_groups, limit_game_center_enabled_versions=limit_game_center_enabled_versions, limit_app_custom_product_pages=limit_app_custom_product_pages, limit_in_app_purchases_v2=limit_in_app_purchases_v2, limit_promoted_purchases=limit_promoted_purchases, limit_app_events=limit_app_events, limit_review_submissions=limit_review_submissions, limit_app_store_version_experiments_v2=limit_app_store_version_experiments_v2)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.app_response import AppResponse
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
    api_instance = openapi_client.CiProductsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_apps = ['fields_apps_example'] # List[str] | the fields to include for returned resources of type apps (optional)
    fields_app_encryption_declarations = ['fields_app_encryption_declarations_example'] # List[str] | the fields to include for returned resources of type appEncryptionDeclarations (optional)
    fields_ci_products = ['fields_ci_products_example'] # List[str] | the fields to include for returned resources of type ciProducts (optional)
    fields_beta_groups = ['fields_beta_groups_example'] # List[str] | the fields to include for returned resources of type betaGroups (optional)
    fields_app_store_versions = ['fields_app_store_versions_example'] # List[str] | the fields to include for returned resources of type appStoreVersions (optional)
    fields_pre_release_versions = ['fields_pre_release_versions_example'] # List[str] | the fields to include for returned resources of type preReleaseVersions (optional)
    fields_beta_app_localizations = ['fields_beta_app_localizations_example'] # List[str] | the fields to include for returned resources of type betaAppLocalizations (optional)
    fields_builds = ['fields_builds_example'] # List[str] | the fields to include for returned resources of type builds (optional)
    fields_beta_license_agreements = ['fields_beta_license_agreements_example'] # List[str] | the fields to include for returned resources of type betaLicenseAgreements (optional)
    fields_beta_app_review_details = ['fields_beta_app_review_details_example'] # List[str] | the fields to include for returned resources of type betaAppReviewDetails (optional)
    fields_app_infos = ['fields_app_infos_example'] # List[str] | the fields to include for returned resources of type appInfos (optional)
    fields_app_clips = ['fields_app_clips_example'] # List[str] | the fields to include for returned resources of type appClips (optional)
    fields_end_user_license_agreements = ['fields_end_user_license_agreements_example'] # List[str] | the fields to include for returned resources of type endUserLicenseAgreements (optional)
    fields_in_app_purchases = ['fields_in_app_purchases_example'] # List[str] | the fields to include for returned resources of type inAppPurchases (optional)
    fields_subscription_groups = ['fields_subscription_groups_example'] # List[str] | the fields to include for returned resources of type subscriptionGroups (optional)
    fields_game_center_enabled_versions = ['fields_game_center_enabled_versions_example'] # List[str] | the fields to include for returned resources of type gameCenterEnabledVersions (optional)
    fields_app_custom_product_pages = ['fields_app_custom_product_pages_example'] # List[str] | the fields to include for returned resources of type appCustomProductPages (optional)
    fields_promoted_purchases = ['fields_promoted_purchases_example'] # List[str] | the fields to include for returned resources of type promotedPurchases (optional)
    fields_app_events = ['fields_app_events_example'] # List[str] | the fields to include for returned resources of type appEvents (optional)
    fields_review_submissions = ['fields_review_submissions_example'] # List[str] | the fields to include for returned resources of type reviewSubmissions (optional)
    fields_subscription_grace_periods = ['fields_subscription_grace_periods_example'] # List[str] | the fields to include for returned resources of type subscriptionGracePeriods (optional)
    fields_game_center_details = ['fields_game_center_details_example'] # List[str] | the fields to include for returned resources of type gameCenterDetails (optional)
    fields_app_store_version_experiments = ['fields_app_store_version_experiments_example'] # List[str] | the fields to include for returned resources of type appStoreVersionExperiments (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_app_encryption_declarations = 56 # int | maximum number of related appEncryptionDeclarations returned (when they are included) (optional)
    limit_beta_groups = 56 # int | maximum number of related betaGroups returned (when they are included) (optional)
    limit_app_store_versions = 56 # int | maximum number of related appStoreVersions returned (when they are included) (optional)
    limit_pre_release_versions = 56 # int | maximum number of related preReleaseVersions returned (when they are included) (optional)
    limit_beta_app_localizations = 56 # int | maximum number of related betaAppLocalizations returned (when they are included) (optional)
    limit_builds = 56 # int | maximum number of related builds returned (when they are included) (optional)
    limit_app_infos = 56 # int | maximum number of related appInfos returned (when they are included) (optional)
    limit_app_clips = 56 # int | maximum number of related appClips returned (when they are included) (optional)
    limit_in_app_purchases = 56 # int | maximum number of related inAppPurchases returned (when they are included) (optional)
    limit_subscription_groups = 56 # int | maximum number of related subscriptionGroups returned (when they are included) (optional)
    limit_game_center_enabled_versions = 56 # int | maximum number of related gameCenterEnabledVersions returned (when they are included) (optional)
    limit_app_custom_product_pages = 56 # int | maximum number of related appCustomProductPages returned (when they are included) (optional)
    limit_in_app_purchases_v2 = 56 # int | maximum number of related inAppPurchasesV2 returned (when they are included) (optional)
    limit_promoted_purchases = 56 # int | maximum number of related promotedPurchases returned (when they are included) (optional)
    limit_app_events = 56 # int | maximum number of related appEvents returned (when they are included) (optional)
    limit_review_submissions = 56 # int | maximum number of related reviewSubmissions returned (when they are included) (optional)
    limit_app_store_version_experiments_v2 = 56 # int | maximum number of related appStoreVersionExperimentsV2 returned (when they are included) (optional)

    try:
        api_response = api_instance.ci_products_app_get_to_one_related(id, fields_apps=fields_apps, fields_app_encryption_declarations=fields_app_encryption_declarations, fields_ci_products=fields_ci_products, fields_beta_groups=fields_beta_groups, fields_app_store_versions=fields_app_store_versions, fields_pre_release_versions=fields_pre_release_versions, fields_beta_app_localizations=fields_beta_app_localizations, fields_builds=fields_builds, fields_beta_license_agreements=fields_beta_license_agreements, fields_beta_app_review_details=fields_beta_app_review_details, fields_app_infos=fields_app_infos, fields_app_clips=fields_app_clips, fields_end_user_license_agreements=fields_end_user_license_agreements, fields_in_app_purchases=fields_in_app_purchases, fields_subscription_groups=fields_subscription_groups, fields_game_center_enabled_versions=fields_game_center_enabled_versions, fields_app_custom_product_pages=fields_app_custom_product_pages, fields_promoted_purchases=fields_promoted_purchases, fields_app_events=fields_app_events, fields_review_submissions=fields_review_submissions, fields_subscription_grace_periods=fields_subscription_grace_periods, fields_game_center_details=fields_game_center_details, fields_app_store_version_experiments=fields_app_store_version_experiments, include=include, limit_app_encryption_declarations=limit_app_encryption_declarations, limit_beta_groups=limit_beta_groups, limit_app_store_versions=limit_app_store_versions, limit_pre_release_versions=limit_pre_release_versions, limit_beta_app_localizations=limit_beta_app_localizations, limit_builds=limit_builds, limit_app_infos=limit_app_infos, limit_app_clips=limit_app_clips, limit_in_app_purchases=limit_in_app_purchases, limit_subscription_groups=limit_subscription_groups, limit_game_center_enabled_versions=limit_game_center_enabled_versions, limit_app_custom_product_pages=limit_app_custom_product_pages, limit_in_app_purchases_v2=limit_in_app_purchases_v2, limit_promoted_purchases=limit_promoted_purchases, limit_app_events=limit_app_events, limit_review_submissions=limit_review_submissions, limit_app_store_version_experiments_v2=limit_app_store_version_experiments_v2)
        print("The response of CiProductsApi->ci_products_app_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiProductsApi->ci_products_app_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_apps** | [**List[str]**](str.md)| the fields to include for returned resources of type apps | [optional] 
 **fields_app_encryption_declarations** | [**List[str]**](str.md)| the fields to include for returned resources of type appEncryptionDeclarations | [optional] 
 **fields_ci_products** | [**List[str]**](str.md)| the fields to include for returned resources of type ciProducts | [optional] 
 **fields_beta_groups** | [**List[str]**](str.md)| the fields to include for returned resources of type betaGroups | [optional] 
 **fields_app_store_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersions | [optional] 
 **fields_pre_release_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type preReleaseVersions | [optional] 
 **fields_beta_app_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type betaAppLocalizations | [optional] 
 **fields_builds** | [**List[str]**](str.md)| the fields to include for returned resources of type builds | [optional] 
 **fields_beta_license_agreements** | [**List[str]**](str.md)| the fields to include for returned resources of type betaLicenseAgreements | [optional] 
 **fields_beta_app_review_details** | [**List[str]**](str.md)| the fields to include for returned resources of type betaAppReviewDetails | [optional] 
 **fields_app_infos** | [**List[str]**](str.md)| the fields to include for returned resources of type appInfos | [optional] 
 **fields_app_clips** | [**List[str]**](str.md)| the fields to include for returned resources of type appClips | [optional] 
 **fields_end_user_license_agreements** | [**List[str]**](str.md)| the fields to include for returned resources of type endUserLicenseAgreements | [optional] 
 **fields_in_app_purchases** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchases | [optional] 
 **fields_subscription_groups** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionGroups | [optional] 
 **fields_game_center_enabled_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterEnabledVersions | [optional] 
 **fields_app_custom_product_pages** | [**List[str]**](str.md)| the fields to include for returned resources of type appCustomProductPages | [optional] 
 **fields_promoted_purchases** | [**List[str]**](str.md)| the fields to include for returned resources of type promotedPurchases | [optional] 
 **fields_app_events** | [**List[str]**](str.md)| the fields to include for returned resources of type appEvents | [optional] 
 **fields_review_submissions** | [**List[str]**](str.md)| the fields to include for returned resources of type reviewSubmissions | [optional] 
 **fields_subscription_grace_periods** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionGracePeriods | [optional] 
 **fields_game_center_details** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterDetails | [optional] 
 **fields_app_store_version_experiments** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionExperiments | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_app_encryption_declarations** | **int**| maximum number of related appEncryptionDeclarations returned (when they are included) | [optional] 
 **limit_beta_groups** | **int**| maximum number of related betaGroups returned (when they are included) | [optional] 
 **limit_app_store_versions** | **int**| maximum number of related appStoreVersions returned (when they are included) | [optional] 
 **limit_pre_release_versions** | **int**| maximum number of related preReleaseVersions returned (when they are included) | [optional] 
 **limit_beta_app_localizations** | **int**| maximum number of related betaAppLocalizations returned (when they are included) | [optional] 
 **limit_builds** | **int**| maximum number of related builds returned (when they are included) | [optional] 
 **limit_app_infos** | **int**| maximum number of related appInfos returned (when they are included) | [optional] 
 **limit_app_clips** | **int**| maximum number of related appClips returned (when they are included) | [optional] 
 **limit_in_app_purchases** | **int**| maximum number of related inAppPurchases returned (when they are included) | [optional] 
 **limit_subscription_groups** | **int**| maximum number of related subscriptionGroups returned (when they are included) | [optional] 
 **limit_game_center_enabled_versions** | **int**| maximum number of related gameCenterEnabledVersions returned (when they are included) | [optional] 
 **limit_app_custom_product_pages** | **int**| maximum number of related appCustomProductPages returned (when they are included) | [optional] 
 **limit_in_app_purchases_v2** | **int**| maximum number of related inAppPurchasesV2 returned (when they are included) | [optional] 
 **limit_promoted_purchases** | **int**| maximum number of related promotedPurchases returned (when they are included) | [optional] 
 **limit_app_events** | **int**| maximum number of related appEvents returned (when they are included) | [optional] 
 **limit_review_submissions** | **int**| maximum number of related reviewSubmissions returned (when they are included) | [optional] 
 **limit_app_store_version_experiments_v2** | **int**| maximum number of related appStoreVersionExperimentsV2 returned (when they are included) | [optional] 

### Return type

[**AppResponse**](AppResponse.md)

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
**200** | Single App |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_products_app_get_to_one_relationship**
> CiProductAppLinkageResponse ci_products_app_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_product_app_linkage_response import CiProductAppLinkageResponse
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
    api_instance = openapi_client.CiProductsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.ci_products_app_get_to_one_relationship(id)
        print("The response of CiProductsApi->ci_products_app_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiProductsApi->ci_products_app_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**CiProductAppLinkageResponse**](CiProductAppLinkageResponse.md)

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

# **ci_products_build_runs_get_to_many_related**
> CiBuildRunsResponse ci_products_build_runs_get_to_many_related(id, filter_builds=filter_builds, sort=sort, fields_ci_build_runs=fields_ci_build_runs, fields_builds=fields_builds, fields_ci_workflows=fields_ci_workflows, fields_ci_products=fields_ci_products, fields_scm_git_references=fields_scm_git_references, fields_scm_pull_requests=fields_scm_pull_requests, limit=limit, include=include, limit_builds=limit_builds)

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
    api_instance = openapi_client.CiProductsApi(api_client)
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
        api_response = api_instance.ci_products_build_runs_get_to_many_related(id, filter_builds=filter_builds, sort=sort, fields_ci_build_runs=fields_ci_build_runs, fields_builds=fields_builds, fields_ci_workflows=fields_ci_workflows, fields_ci_products=fields_ci_products, fields_scm_git_references=fields_scm_git_references, fields_scm_pull_requests=fields_scm_pull_requests, limit=limit, include=include, limit_builds=limit_builds)
        print("The response of CiProductsApi->ci_products_build_runs_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiProductsApi->ci_products_build_runs_get_to_many_related: %s\n" % e)
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

# **ci_products_build_runs_get_to_many_relationship**
> CiProductBuildRunsLinkagesResponse ci_products_build_runs_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_product_build_runs_linkages_response import CiProductBuildRunsLinkagesResponse
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
    api_instance = openapi_client.CiProductsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.ci_products_build_runs_get_to_many_relationship(id, limit=limit)
        print("The response of CiProductsApi->ci_products_build_runs_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiProductsApi->ci_products_build_runs_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**CiProductBuildRunsLinkagesResponse**](CiProductBuildRunsLinkagesResponse.md)

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

# **ci_products_delete_instance**
> ci_products_delete_instance(id)

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
    api_instance = openapi_client.CiProductsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.ci_products_delete_instance(id)
    except Exception as e:
        print("Exception when calling CiProductsApi->ci_products_delete_instance: %s\n" % e)
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

# **ci_products_get_collection**
> CiProductsResponse ci_products_get_collection(filter_product_type=filter_product_type, filter_app=filter_app, fields_ci_products=fields_ci_products, fields_apps=fields_apps, fields_scm_repositories=fields_scm_repositories, limit=limit, include=include, limit_primary_repositories=limit_primary_repositories)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_products_response import CiProductsResponse
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
    api_instance = openapi_client.CiProductsApi(api_client)
    filter_product_type = ['filter_product_type_example'] # List[str] | filter by attribute 'productType' (optional)
    filter_app = ['filter_app_example'] # List[str] | filter by id(s) of related 'app' (optional)
    fields_ci_products = ['fields_ci_products_example'] # List[str] | the fields to include for returned resources of type ciProducts (optional)
    fields_apps = ['fields_apps_example'] # List[str] | the fields to include for returned resources of type apps (optional)
    fields_scm_repositories = ['fields_scm_repositories_example'] # List[str] | the fields to include for returned resources of type scmRepositories (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_primary_repositories = 56 # int | maximum number of related primaryRepositories returned (when they are included) (optional)

    try:
        api_response = api_instance.ci_products_get_collection(filter_product_type=filter_product_type, filter_app=filter_app, fields_ci_products=fields_ci_products, fields_apps=fields_apps, fields_scm_repositories=fields_scm_repositories, limit=limit, include=include, limit_primary_repositories=limit_primary_repositories)
        print("The response of CiProductsApi->ci_products_get_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiProductsApi->ci_products_get_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter_product_type** | [**List[str]**](str.md)| filter by attribute &#39;productType&#39; | [optional] 
 **filter_app** | [**List[str]**](str.md)| filter by id(s) of related &#39;app&#39; | [optional] 
 **fields_ci_products** | [**List[str]**](str.md)| the fields to include for returned resources of type ciProducts | [optional] 
 **fields_apps** | [**List[str]**](str.md)| the fields to include for returned resources of type apps | [optional] 
 **fields_scm_repositories** | [**List[str]**](str.md)| the fields to include for returned resources of type scmRepositories | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_primary_repositories** | **int**| maximum number of related primaryRepositories returned (when they are included) | [optional] 

### Return type

[**CiProductsResponse**](CiProductsResponse.md)

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
**200** | List of CiProducts |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_products_get_instance**
> CiProductResponse ci_products_get_instance(id, fields_ci_products=fields_ci_products, fields_apps=fields_apps, fields_scm_repositories=fields_scm_repositories, include=include, limit_primary_repositories=limit_primary_repositories)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_product_response import CiProductResponse
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
    api_instance = openapi_client.CiProductsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_ci_products = ['fields_ci_products_example'] # List[str] | the fields to include for returned resources of type ciProducts (optional)
    fields_apps = ['fields_apps_example'] # List[str] | the fields to include for returned resources of type apps (optional)
    fields_scm_repositories = ['fields_scm_repositories_example'] # List[str] | the fields to include for returned resources of type scmRepositories (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_primary_repositories = 56 # int | maximum number of related primaryRepositories returned (when they are included) (optional)

    try:
        api_response = api_instance.ci_products_get_instance(id, fields_ci_products=fields_ci_products, fields_apps=fields_apps, fields_scm_repositories=fields_scm_repositories, include=include, limit_primary_repositories=limit_primary_repositories)
        print("The response of CiProductsApi->ci_products_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiProductsApi->ci_products_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_ci_products** | [**List[str]**](str.md)| the fields to include for returned resources of type ciProducts | [optional] 
 **fields_apps** | [**List[str]**](str.md)| the fields to include for returned resources of type apps | [optional] 
 **fields_scm_repositories** | [**List[str]**](str.md)| the fields to include for returned resources of type scmRepositories | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_primary_repositories** | **int**| maximum number of related primaryRepositories returned (when they are included) | [optional] 

### Return type

[**CiProductResponse**](CiProductResponse.md)

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
**200** | Single CiProduct |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_products_primary_repositories_get_to_many_related**
> ScmRepositoriesResponse ci_products_primary_repositories_get_to_many_related(id, filter_id=filter_id, fields_scm_repositories=fields_scm_repositories, fields_scm_providers=fields_scm_providers, fields_scm_git_references=fields_scm_git_references, limit=limit, include=include)

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
    api_instance = openapi_client.CiProductsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_id = ['filter_id_example'] # List[str] | filter by id(s) (optional)
    fields_scm_repositories = ['fields_scm_repositories_example'] # List[str] | the fields to include for returned resources of type scmRepositories (optional)
    fields_scm_providers = ['fields_scm_providers_example'] # List[str] | the fields to include for returned resources of type scmProviders (optional)
    fields_scm_git_references = ['fields_scm_git_references_example'] # List[str] | the fields to include for returned resources of type scmGitReferences (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.ci_products_primary_repositories_get_to_many_related(id, filter_id=filter_id, fields_scm_repositories=fields_scm_repositories, fields_scm_providers=fields_scm_providers, fields_scm_git_references=fields_scm_git_references, limit=limit, include=include)
        print("The response of CiProductsApi->ci_products_primary_repositories_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiProductsApi->ci_products_primary_repositories_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_id** | [**List[str]**](str.md)| filter by id(s) | [optional] 
 **fields_scm_repositories** | [**List[str]**](str.md)| the fields to include for returned resources of type scmRepositories | [optional] 
 **fields_scm_providers** | [**List[str]**](str.md)| the fields to include for returned resources of type scmProviders | [optional] 
 **fields_scm_git_references** | [**List[str]**](str.md)| the fields to include for returned resources of type scmGitReferences | [optional] 
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
**404** | Not found error |  -  |
**200** | List of ScmRepositories |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_products_primary_repositories_get_to_many_relationship**
> CiProductPrimaryRepositoriesLinkagesResponse ci_products_primary_repositories_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_product_primary_repositories_linkages_response import CiProductPrimaryRepositoriesLinkagesResponse
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
    api_instance = openapi_client.CiProductsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.ci_products_primary_repositories_get_to_many_relationship(id, limit=limit)
        print("The response of CiProductsApi->ci_products_primary_repositories_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiProductsApi->ci_products_primary_repositories_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**CiProductPrimaryRepositoriesLinkagesResponse**](CiProductPrimaryRepositoriesLinkagesResponse.md)

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

# **ci_products_workflows_get_to_many_related**
> CiWorkflowsResponse ci_products_workflows_get_to_many_related(id, fields_ci_workflows=fields_ci_workflows, fields_ci_products=fields_ci_products, fields_scm_repositories=fields_scm_repositories, fields_ci_xcode_versions=fields_ci_xcode_versions, fields_ci_mac_os_versions=fields_ci_mac_os_versions, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_workflows_response import CiWorkflowsResponse
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
    api_instance = openapi_client.CiProductsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_ci_workflows = ['fields_ci_workflows_example'] # List[str] | the fields to include for returned resources of type ciWorkflows (optional)
    fields_ci_products = ['fields_ci_products_example'] # List[str] | the fields to include for returned resources of type ciProducts (optional)
    fields_scm_repositories = ['fields_scm_repositories_example'] # List[str] | the fields to include for returned resources of type scmRepositories (optional)
    fields_ci_xcode_versions = ['fields_ci_xcode_versions_example'] # List[str] | the fields to include for returned resources of type ciXcodeVersions (optional)
    fields_ci_mac_os_versions = ['fields_ci_mac_os_versions_example'] # List[str] | the fields to include for returned resources of type ciMacOsVersions (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.ci_products_workflows_get_to_many_related(id, fields_ci_workflows=fields_ci_workflows, fields_ci_products=fields_ci_products, fields_scm_repositories=fields_scm_repositories, fields_ci_xcode_versions=fields_ci_xcode_versions, fields_ci_mac_os_versions=fields_ci_mac_os_versions, limit=limit, include=include)
        print("The response of CiProductsApi->ci_products_workflows_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiProductsApi->ci_products_workflows_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_ci_workflows** | [**List[str]**](str.md)| the fields to include for returned resources of type ciWorkflows | [optional] 
 **fields_ci_products** | [**List[str]**](str.md)| the fields to include for returned resources of type ciProducts | [optional] 
 **fields_scm_repositories** | [**List[str]**](str.md)| the fields to include for returned resources of type scmRepositories | [optional] 
 **fields_ci_xcode_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type ciXcodeVersions | [optional] 
 **fields_ci_mac_os_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type ciMacOsVersions | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**CiWorkflowsResponse**](CiWorkflowsResponse.md)

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
**200** | List of CiWorkflows |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ci_products_workflows_get_to_many_relationship**
> CiProductWorkflowsLinkagesResponse ci_products_workflows_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.ci_product_workflows_linkages_response import CiProductWorkflowsLinkagesResponse
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
    api_instance = openapi_client.CiProductsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.ci_products_workflows_get_to_many_relationship(id, limit=limit)
        print("The response of CiProductsApi->ci_products_workflows_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CiProductsApi->ci_products_workflows_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**CiProductWorkflowsLinkagesResponse**](CiProductWorkflowsLinkagesResponse.md)

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

