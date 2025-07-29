# openapi_client.GameCenterAppVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**game_center_app_versions_app_store_version_get_to_one_related**](GameCenterAppVersionsApi.md#game_center_app_versions_app_store_version_get_to_one_related) | **GET** /v1/gameCenterAppVersions/{id}/appStoreVersion | 
[**game_center_app_versions_app_store_version_get_to_one_relationship**](GameCenterAppVersionsApi.md#game_center_app_versions_app_store_version_get_to_one_relationship) | **GET** /v1/gameCenterAppVersions/{id}/relationships/appStoreVersion | 
[**game_center_app_versions_compatibility_versions_create_to_many_relationship**](GameCenterAppVersionsApi.md#game_center_app_versions_compatibility_versions_create_to_many_relationship) | **POST** /v1/gameCenterAppVersions/{id}/relationships/compatibilityVersions | 
[**game_center_app_versions_compatibility_versions_delete_to_many_relationship**](GameCenterAppVersionsApi.md#game_center_app_versions_compatibility_versions_delete_to_many_relationship) | **DELETE** /v1/gameCenterAppVersions/{id}/relationships/compatibilityVersions | 
[**game_center_app_versions_compatibility_versions_get_to_many_related**](GameCenterAppVersionsApi.md#game_center_app_versions_compatibility_versions_get_to_many_related) | **GET** /v1/gameCenterAppVersions/{id}/compatibilityVersions | 
[**game_center_app_versions_compatibility_versions_get_to_many_relationship**](GameCenterAppVersionsApi.md#game_center_app_versions_compatibility_versions_get_to_many_relationship) | **GET** /v1/gameCenterAppVersions/{id}/relationships/compatibilityVersions | 
[**game_center_app_versions_create_instance**](GameCenterAppVersionsApi.md#game_center_app_versions_create_instance) | **POST** /v1/gameCenterAppVersions | 
[**game_center_app_versions_get_instance**](GameCenterAppVersionsApi.md#game_center_app_versions_get_instance) | **GET** /v1/gameCenterAppVersions/{id} | 
[**game_center_app_versions_update_instance**](GameCenterAppVersionsApi.md#game_center_app_versions_update_instance) | **PATCH** /v1/gameCenterAppVersions/{id} | 


# **game_center_app_versions_app_store_version_get_to_one_related**
> AppStoreVersionResponse game_center_app_versions_app_store_version_get_to_one_related(id, fields_app_store_versions=fields_app_store_versions, fields_apps=fields_apps, fields_age_rating_declarations=fields_age_rating_declarations, fields_app_store_version_localizations=fields_app_store_version_localizations, fields_builds=fields_builds, fields_app_store_version_phased_releases=fields_app_store_version_phased_releases, fields_game_center_app_versions=fields_game_center_app_versions, fields_routing_app_coverages=fields_routing_app_coverages, fields_app_store_review_details=fields_app_store_review_details, fields_app_store_version_submissions=fields_app_store_version_submissions, fields_app_clip_default_experiences=fields_app_clip_default_experiences, fields_app_store_version_experiments=fields_app_store_version_experiments, fields_alternative_distribution_packages=fields_alternative_distribution_packages, include=include, limit_app_store_version_localizations=limit_app_store_version_localizations, limit_app_store_version_experiments=limit_app_store_version_experiments, limit_app_store_version_experiments_v2=limit_app_store_version_experiments_v2)

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
    api_instance = openapi_client.GameCenterAppVersionsApi(api_client)
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
        api_response = api_instance.game_center_app_versions_app_store_version_get_to_one_related(id, fields_app_store_versions=fields_app_store_versions, fields_apps=fields_apps, fields_age_rating_declarations=fields_age_rating_declarations, fields_app_store_version_localizations=fields_app_store_version_localizations, fields_builds=fields_builds, fields_app_store_version_phased_releases=fields_app_store_version_phased_releases, fields_game_center_app_versions=fields_game_center_app_versions, fields_routing_app_coverages=fields_routing_app_coverages, fields_app_store_review_details=fields_app_store_review_details, fields_app_store_version_submissions=fields_app_store_version_submissions, fields_app_clip_default_experiences=fields_app_clip_default_experiences, fields_app_store_version_experiments=fields_app_store_version_experiments, fields_alternative_distribution_packages=fields_alternative_distribution_packages, include=include, limit_app_store_version_localizations=limit_app_store_version_localizations, limit_app_store_version_experiments=limit_app_store_version_experiments, limit_app_store_version_experiments_v2=limit_app_store_version_experiments_v2)
        print("The response of GameCenterAppVersionsApi->game_center_app_versions_app_store_version_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAppVersionsApi->game_center_app_versions_app_store_version_get_to_one_related: %s\n" % e)
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

# **game_center_app_versions_app_store_version_get_to_one_relationship**
> GameCenterAppVersionAppStoreVersionLinkageResponse game_center_app_versions_app_store_version_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_app_version_app_store_version_linkage_response import GameCenterAppVersionAppStoreVersionLinkageResponse
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
    api_instance = openapi_client.GameCenterAppVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.game_center_app_versions_app_store_version_get_to_one_relationship(id)
        print("The response of GameCenterAppVersionsApi->game_center_app_versions_app_store_version_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAppVersionsApi->game_center_app_versions_app_store_version_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**GameCenterAppVersionAppStoreVersionLinkageResponse**](GameCenterAppVersionAppStoreVersionLinkageResponse.md)

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

# **game_center_app_versions_compatibility_versions_create_to_many_relationship**
> game_center_app_versions_compatibility_versions_create_to_many_relationship(id, game_center_app_version_compatibility_versions_linkages_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_app_version_compatibility_versions_linkages_request import GameCenterAppVersionCompatibilityVersionsLinkagesRequest
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
    api_instance = openapi_client.GameCenterAppVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_app_version_compatibility_versions_linkages_request = openapi_client.GameCenterAppVersionCompatibilityVersionsLinkagesRequest() # GameCenterAppVersionCompatibilityVersionsLinkagesRequest | List of related linkages

    try:
        api_instance.game_center_app_versions_compatibility_versions_create_to_many_relationship(id, game_center_app_version_compatibility_versions_linkages_request)
    except Exception as e:
        print("Exception when calling GameCenterAppVersionsApi->game_center_app_versions_compatibility_versions_create_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_app_version_compatibility_versions_linkages_request** | [**GameCenterAppVersionCompatibilityVersionsLinkagesRequest**](GameCenterAppVersionCompatibilityVersionsLinkagesRequest.md)| List of related linkages | 

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

# **game_center_app_versions_compatibility_versions_delete_to_many_relationship**
> game_center_app_versions_compatibility_versions_delete_to_many_relationship(id, game_center_app_version_compatibility_versions_linkages_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_app_version_compatibility_versions_linkages_request import GameCenterAppVersionCompatibilityVersionsLinkagesRequest
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
    api_instance = openapi_client.GameCenterAppVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_app_version_compatibility_versions_linkages_request = openapi_client.GameCenterAppVersionCompatibilityVersionsLinkagesRequest() # GameCenterAppVersionCompatibilityVersionsLinkagesRequest | List of related linkages

    try:
        api_instance.game_center_app_versions_compatibility_versions_delete_to_many_relationship(id, game_center_app_version_compatibility_versions_linkages_request)
    except Exception as e:
        print("Exception when calling GameCenterAppVersionsApi->game_center_app_versions_compatibility_versions_delete_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_app_version_compatibility_versions_linkages_request** | [**GameCenterAppVersionCompatibilityVersionsLinkagesRequest**](GameCenterAppVersionCompatibilityVersionsLinkagesRequest.md)| List of related linkages | 

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

# **game_center_app_versions_compatibility_versions_get_to_many_related**
> GameCenterAppVersionsResponse game_center_app_versions_compatibility_versions_get_to_many_related(id, filter_enabled=filter_enabled, fields_game_center_app_versions=fields_game_center_app_versions, fields_app_store_versions=fields_app_store_versions, limit=limit, include=include, limit_compatibility_versions=limit_compatibility_versions)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_app_versions_response import GameCenterAppVersionsResponse
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
    api_instance = openapi_client.GameCenterAppVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_enabled = ['filter_enabled_example'] # List[str] | filter by attribute 'enabled' (optional)
    fields_game_center_app_versions = ['fields_game_center_app_versions_example'] # List[str] | the fields to include for returned resources of type gameCenterAppVersions (optional)
    fields_app_store_versions = ['fields_app_store_versions_example'] # List[str] | the fields to include for returned resources of type appStoreVersions (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_compatibility_versions = 56 # int | maximum number of related compatibilityVersions returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_app_versions_compatibility_versions_get_to_many_related(id, filter_enabled=filter_enabled, fields_game_center_app_versions=fields_game_center_app_versions, fields_app_store_versions=fields_app_store_versions, limit=limit, include=include, limit_compatibility_versions=limit_compatibility_versions)
        print("The response of GameCenterAppVersionsApi->game_center_app_versions_compatibility_versions_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAppVersionsApi->game_center_app_versions_compatibility_versions_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_enabled** | [**List[str]**](str.md)| filter by attribute &#39;enabled&#39; | [optional] 
 **fields_game_center_app_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAppVersions | [optional] 
 **fields_app_store_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersions | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_compatibility_versions** | **int**| maximum number of related compatibilityVersions returned (when they are included) | [optional] 

### Return type

[**GameCenterAppVersionsResponse**](GameCenterAppVersionsResponse.md)

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
**200** | List of GameCenterAppVersions |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_app_versions_compatibility_versions_get_to_many_relationship**
> GameCenterAppVersionCompatibilityVersionsLinkagesResponse game_center_app_versions_compatibility_versions_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_app_version_compatibility_versions_linkages_response import GameCenterAppVersionCompatibilityVersionsLinkagesResponse
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
    api_instance = openapi_client.GameCenterAppVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_app_versions_compatibility_versions_get_to_many_relationship(id, limit=limit)
        print("The response of GameCenterAppVersionsApi->game_center_app_versions_compatibility_versions_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAppVersionsApi->game_center_app_versions_compatibility_versions_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterAppVersionCompatibilityVersionsLinkagesResponse**](GameCenterAppVersionCompatibilityVersionsLinkagesResponse.md)

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

# **game_center_app_versions_create_instance**
> GameCenterAppVersionResponse game_center_app_versions_create_instance(game_center_app_version_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_app_version_create_request import GameCenterAppVersionCreateRequest
from openapi_client.models.game_center_app_version_response import GameCenterAppVersionResponse
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
    api_instance = openapi_client.GameCenterAppVersionsApi(api_client)
    game_center_app_version_create_request = openapi_client.GameCenterAppVersionCreateRequest() # GameCenterAppVersionCreateRequest | GameCenterAppVersion representation

    try:
        api_response = api_instance.game_center_app_versions_create_instance(game_center_app_version_create_request)
        print("The response of GameCenterAppVersionsApi->game_center_app_versions_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAppVersionsApi->game_center_app_versions_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **game_center_app_version_create_request** | [**GameCenterAppVersionCreateRequest**](GameCenterAppVersionCreateRequest.md)| GameCenterAppVersion representation | 

### Return type

[**GameCenterAppVersionResponse**](GameCenterAppVersionResponse.md)

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
**201** | Single GameCenterAppVersion |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_app_versions_get_instance**
> GameCenterAppVersionResponse game_center_app_versions_get_instance(id, fields_game_center_app_versions=fields_game_center_app_versions, fields_app_store_versions=fields_app_store_versions, include=include, limit_compatibility_versions=limit_compatibility_versions)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_app_version_response import GameCenterAppVersionResponse
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
    api_instance = openapi_client.GameCenterAppVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_app_versions = ['fields_game_center_app_versions_example'] # List[str] | the fields to include for returned resources of type gameCenterAppVersions (optional)
    fields_app_store_versions = ['fields_app_store_versions_example'] # List[str] | the fields to include for returned resources of type appStoreVersions (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_compatibility_versions = 56 # int | maximum number of related compatibilityVersions returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_app_versions_get_instance(id, fields_game_center_app_versions=fields_game_center_app_versions, fields_app_store_versions=fields_app_store_versions, include=include, limit_compatibility_versions=limit_compatibility_versions)
        print("The response of GameCenterAppVersionsApi->game_center_app_versions_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAppVersionsApi->game_center_app_versions_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_app_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAppVersions | [optional] 
 **fields_app_store_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersions | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_compatibility_versions** | **int**| maximum number of related compatibilityVersions returned (when they are included) | [optional] 

### Return type

[**GameCenterAppVersionResponse**](GameCenterAppVersionResponse.md)

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
**200** | Single GameCenterAppVersion |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_app_versions_update_instance**
> GameCenterAppVersionResponse game_center_app_versions_update_instance(id, game_center_app_version_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_app_version_response import GameCenterAppVersionResponse
from openapi_client.models.game_center_app_version_update_request import GameCenterAppVersionUpdateRequest
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
    api_instance = openapi_client.GameCenterAppVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_app_version_update_request = openapi_client.GameCenterAppVersionUpdateRequest() # GameCenterAppVersionUpdateRequest | GameCenterAppVersion representation

    try:
        api_response = api_instance.game_center_app_versions_update_instance(id, game_center_app_version_update_request)
        print("The response of GameCenterAppVersionsApi->game_center_app_versions_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAppVersionsApi->game_center_app_versions_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_app_version_update_request** | [**GameCenterAppVersionUpdateRequest**](GameCenterAppVersionUpdateRequest.md)| GameCenterAppVersion representation | 

### Return type

[**GameCenterAppVersionResponse**](GameCenterAppVersionResponse.md)

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
**200** | Single GameCenterAppVersion |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

