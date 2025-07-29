# openapi_client.GameCenterAchievementsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**game_center_achievements_activity_update_to_one_relationship**](GameCenterAchievementsApi.md#game_center_achievements_activity_update_to_one_relationship) | **PATCH** /v1/gameCenterAchievements/{id}/relationships/activity | 
[**game_center_achievements_create_instance**](GameCenterAchievementsApi.md#game_center_achievements_create_instance) | **POST** /v1/gameCenterAchievements | 
[**game_center_achievements_delete_instance**](GameCenterAchievementsApi.md#game_center_achievements_delete_instance) | **DELETE** /v1/gameCenterAchievements/{id} | 
[**game_center_achievements_get_instance**](GameCenterAchievementsApi.md#game_center_achievements_get_instance) | **GET** /v1/gameCenterAchievements/{id} | 
[**game_center_achievements_group_achievement_get_to_one_related**](GameCenterAchievementsApi.md#game_center_achievements_group_achievement_get_to_one_related) | **GET** /v1/gameCenterAchievements/{id}/groupAchievement | 
[**game_center_achievements_group_achievement_get_to_one_relationship**](GameCenterAchievementsApi.md#game_center_achievements_group_achievement_get_to_one_relationship) | **GET** /v1/gameCenterAchievements/{id}/relationships/groupAchievement | 
[**game_center_achievements_group_achievement_update_to_one_relationship**](GameCenterAchievementsApi.md#game_center_achievements_group_achievement_update_to_one_relationship) | **PATCH** /v1/gameCenterAchievements/{id}/relationships/groupAchievement | 
[**game_center_achievements_localizations_get_to_many_related**](GameCenterAchievementsApi.md#game_center_achievements_localizations_get_to_many_related) | **GET** /v1/gameCenterAchievements/{id}/localizations | 
[**game_center_achievements_localizations_get_to_many_relationship**](GameCenterAchievementsApi.md#game_center_achievements_localizations_get_to_many_relationship) | **GET** /v1/gameCenterAchievements/{id}/relationships/localizations | 
[**game_center_achievements_releases_get_to_many_related**](GameCenterAchievementsApi.md#game_center_achievements_releases_get_to_many_related) | **GET** /v1/gameCenterAchievements/{id}/releases | 
[**game_center_achievements_releases_get_to_many_relationship**](GameCenterAchievementsApi.md#game_center_achievements_releases_get_to_many_relationship) | **GET** /v1/gameCenterAchievements/{id}/relationships/releases | 
[**game_center_achievements_update_instance**](GameCenterAchievementsApi.md#game_center_achievements_update_instance) | **PATCH** /v1/gameCenterAchievements/{id} | 


# **game_center_achievements_activity_update_to_one_relationship**
> game_center_achievements_activity_update_to_one_relationship(id, game_center_achievement_activity_linkage_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_achievement_activity_linkage_request import GameCenterAchievementActivityLinkageRequest
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
    api_instance = openapi_client.GameCenterAchievementsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_achievement_activity_linkage_request = openapi_client.GameCenterAchievementActivityLinkageRequest() # GameCenterAchievementActivityLinkageRequest | Related linkage

    try:
        api_instance.game_center_achievements_activity_update_to_one_relationship(id, game_center_achievement_activity_linkage_request)
    except Exception as e:
        print("Exception when calling GameCenterAchievementsApi->game_center_achievements_activity_update_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_achievement_activity_linkage_request** | [**GameCenterAchievementActivityLinkageRequest**](GameCenterAchievementActivityLinkageRequest.md)| Related linkage | 

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

# **game_center_achievements_create_instance**
> GameCenterAchievementResponse game_center_achievements_create_instance(game_center_achievement_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_achievement_create_request import GameCenterAchievementCreateRequest
from openapi_client.models.game_center_achievement_response import GameCenterAchievementResponse
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
    api_instance = openapi_client.GameCenterAchievementsApi(api_client)
    game_center_achievement_create_request = openapi_client.GameCenterAchievementCreateRequest() # GameCenterAchievementCreateRequest | GameCenterAchievement representation

    try:
        api_response = api_instance.game_center_achievements_create_instance(game_center_achievement_create_request)
        print("The response of GameCenterAchievementsApi->game_center_achievements_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAchievementsApi->game_center_achievements_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **game_center_achievement_create_request** | [**GameCenterAchievementCreateRequest**](GameCenterAchievementCreateRequest.md)| GameCenterAchievement representation | 

### Return type

[**GameCenterAchievementResponse**](GameCenterAchievementResponse.md)

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
**201** | Single GameCenterAchievement |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_achievements_delete_instance**
> game_center_achievements_delete_instance(id)

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
    api_instance = openapi_client.GameCenterAchievementsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.game_center_achievements_delete_instance(id)
    except Exception as e:
        print("Exception when calling GameCenterAchievementsApi->game_center_achievements_delete_instance: %s\n" % e)
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

# **game_center_achievements_get_instance**
> GameCenterAchievementResponse game_center_achievements_get_instance(id, fields_game_center_achievements=fields_game_center_achievements, fields_game_center_achievement_localizations=fields_game_center_achievement_localizations, fields_game_center_achievement_releases=fields_game_center_achievement_releases, include=include, limit_localizations=limit_localizations, limit_releases=limit_releases)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_achievement_response import GameCenterAchievementResponse
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
    api_instance = openapi_client.GameCenterAchievementsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_achievements = ['fields_game_center_achievements_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievements (optional)
    fields_game_center_achievement_localizations = ['fields_game_center_achievement_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievementLocalizations (optional)
    fields_game_center_achievement_releases = ['fields_game_center_achievement_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievementReleases (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_localizations = 56 # int | maximum number of related localizations returned (when they are included) (optional)
    limit_releases = 56 # int | maximum number of related releases returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_achievements_get_instance(id, fields_game_center_achievements=fields_game_center_achievements, fields_game_center_achievement_localizations=fields_game_center_achievement_localizations, fields_game_center_achievement_releases=fields_game_center_achievement_releases, include=include, limit_localizations=limit_localizations, limit_releases=limit_releases)
        print("The response of GameCenterAchievementsApi->game_center_achievements_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAchievementsApi->game_center_achievements_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_achievements** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievements | [optional] 
 **fields_game_center_achievement_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional] 
 **fields_game_center_achievement_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievementReleases | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_localizations** | **int**| maximum number of related localizations returned (when they are included) | [optional] 
 **limit_releases** | **int**| maximum number of related releases returned (when they are included) | [optional] 

### Return type

[**GameCenterAchievementResponse**](GameCenterAchievementResponse.md)

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
**200** | Single GameCenterAchievement |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_achievements_group_achievement_get_to_one_related**
> GameCenterAchievementResponse game_center_achievements_group_achievement_get_to_one_related(id, fields_game_center_achievements=fields_game_center_achievements, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_achievement_localizations=fields_game_center_achievement_localizations, fields_game_center_achievement_releases=fields_game_center_achievement_releases, fields_game_center_activities=fields_game_center_activities, include=include, limit_localizations=limit_localizations, limit_releases=limit_releases)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_achievement_response import GameCenterAchievementResponse
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
    api_instance = openapi_client.GameCenterAchievementsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_achievements = ['fields_game_center_achievements_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievements (optional)
    fields_game_center_details = ['fields_game_center_details_example'] # List[str] | the fields to include for returned resources of type gameCenterDetails (optional)
    fields_game_center_groups = ['fields_game_center_groups_example'] # List[str] | the fields to include for returned resources of type gameCenterGroups (optional)
    fields_game_center_achievement_localizations = ['fields_game_center_achievement_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievementLocalizations (optional)
    fields_game_center_achievement_releases = ['fields_game_center_achievement_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievementReleases (optional)
    fields_game_center_activities = ['fields_game_center_activities_example'] # List[str] | the fields to include for returned resources of type gameCenterActivities (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_localizations = 56 # int | maximum number of related localizations returned (when they are included) (optional)
    limit_releases = 56 # int | maximum number of related releases returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_achievements_group_achievement_get_to_one_related(id, fields_game_center_achievements=fields_game_center_achievements, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_achievement_localizations=fields_game_center_achievement_localizations, fields_game_center_achievement_releases=fields_game_center_achievement_releases, fields_game_center_activities=fields_game_center_activities, include=include, limit_localizations=limit_localizations, limit_releases=limit_releases)
        print("The response of GameCenterAchievementsApi->game_center_achievements_group_achievement_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAchievementsApi->game_center_achievements_group_achievement_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_achievements** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievements | [optional] 
 **fields_game_center_details** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterDetails | [optional] 
 **fields_game_center_groups** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterGroups | [optional] 
 **fields_game_center_achievement_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional] 
 **fields_game_center_achievement_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievementReleases | [optional] 
 **fields_game_center_activities** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivities | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_localizations** | **int**| maximum number of related localizations returned (when they are included) | [optional] 
 **limit_releases** | **int**| maximum number of related releases returned (when they are included) | [optional] 

### Return type

[**GameCenterAchievementResponse**](GameCenterAchievementResponse.md)

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
**200** | Single GameCenterAchievement |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_achievements_group_achievement_get_to_one_relationship**
> GameCenterAchievementGroupAchievementLinkageResponse game_center_achievements_group_achievement_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_achievement_group_achievement_linkage_response import GameCenterAchievementGroupAchievementLinkageResponse
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
    api_instance = openapi_client.GameCenterAchievementsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.game_center_achievements_group_achievement_get_to_one_relationship(id)
        print("The response of GameCenterAchievementsApi->game_center_achievements_group_achievement_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAchievementsApi->game_center_achievements_group_achievement_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**GameCenterAchievementGroupAchievementLinkageResponse**](GameCenterAchievementGroupAchievementLinkageResponse.md)

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

# **game_center_achievements_group_achievement_update_to_one_relationship**
> game_center_achievements_group_achievement_update_to_one_relationship(id, game_center_achievement_group_achievement_linkage_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_achievement_group_achievement_linkage_request import GameCenterAchievementGroupAchievementLinkageRequest
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
    api_instance = openapi_client.GameCenterAchievementsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_achievement_group_achievement_linkage_request = openapi_client.GameCenterAchievementGroupAchievementLinkageRequest() # GameCenterAchievementGroupAchievementLinkageRequest | Related linkage

    try:
        api_instance.game_center_achievements_group_achievement_update_to_one_relationship(id, game_center_achievement_group_achievement_linkage_request)
    except Exception as e:
        print("Exception when calling GameCenterAchievementsApi->game_center_achievements_group_achievement_update_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_achievement_group_achievement_linkage_request** | [**GameCenterAchievementGroupAchievementLinkageRequest**](GameCenterAchievementGroupAchievementLinkageRequest.md)| Related linkage | 

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

# **game_center_achievements_localizations_get_to_many_related**
> GameCenterAchievementLocalizationsResponse game_center_achievements_localizations_get_to_many_related(id, fields_game_center_achievement_localizations=fields_game_center_achievement_localizations, fields_game_center_achievements=fields_game_center_achievements, fields_game_center_achievement_images=fields_game_center_achievement_images, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_achievement_localizations_response import GameCenterAchievementLocalizationsResponse
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
    api_instance = openapi_client.GameCenterAchievementsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_achievement_localizations = ['fields_game_center_achievement_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievementLocalizations (optional)
    fields_game_center_achievements = ['fields_game_center_achievements_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievements (optional)
    fields_game_center_achievement_images = ['fields_game_center_achievement_images_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievementImages (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.game_center_achievements_localizations_get_to_many_related(id, fields_game_center_achievement_localizations=fields_game_center_achievement_localizations, fields_game_center_achievements=fields_game_center_achievements, fields_game_center_achievement_images=fields_game_center_achievement_images, limit=limit, include=include)
        print("The response of GameCenterAchievementsApi->game_center_achievements_localizations_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAchievementsApi->game_center_achievements_localizations_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_achievement_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional] 
 **fields_game_center_achievements** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievements | [optional] 
 **fields_game_center_achievement_images** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievementImages | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**GameCenterAchievementLocalizationsResponse**](GameCenterAchievementLocalizationsResponse.md)

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
**200** | List of GameCenterAchievementLocalizations |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_achievements_localizations_get_to_many_relationship**
> GameCenterAchievementLocalizationsLinkagesResponse game_center_achievements_localizations_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_achievement_localizations_linkages_response import GameCenterAchievementLocalizationsLinkagesResponse
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
    api_instance = openapi_client.GameCenterAchievementsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_achievements_localizations_get_to_many_relationship(id, limit=limit)
        print("The response of GameCenterAchievementsApi->game_center_achievements_localizations_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAchievementsApi->game_center_achievements_localizations_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterAchievementLocalizationsLinkagesResponse**](GameCenterAchievementLocalizationsLinkagesResponse.md)

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

# **game_center_achievements_releases_get_to_many_related**
> GameCenterAchievementReleasesResponse game_center_achievements_releases_get_to_many_related(id, filter_live=filter_live, filter_game_center_detail=filter_game_center_detail, fields_game_center_achievement_releases=fields_game_center_achievement_releases, fields_game_center_details=fields_game_center_details, fields_game_center_achievements=fields_game_center_achievements, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_achievement_releases_response import GameCenterAchievementReleasesResponse
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
    api_instance = openapi_client.GameCenterAchievementsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_live = ['filter_live_example'] # List[str] | filter by attribute 'live' (optional)
    filter_game_center_detail = ['filter_game_center_detail_example'] # List[str] | filter by id(s) of related 'gameCenterDetail' (optional)
    fields_game_center_achievement_releases = ['fields_game_center_achievement_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievementReleases (optional)
    fields_game_center_details = ['fields_game_center_details_example'] # List[str] | the fields to include for returned resources of type gameCenterDetails (optional)
    fields_game_center_achievements = ['fields_game_center_achievements_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievements (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.game_center_achievements_releases_get_to_many_related(id, filter_live=filter_live, filter_game_center_detail=filter_game_center_detail, fields_game_center_achievement_releases=fields_game_center_achievement_releases, fields_game_center_details=fields_game_center_details, fields_game_center_achievements=fields_game_center_achievements, limit=limit, include=include)
        print("The response of GameCenterAchievementsApi->game_center_achievements_releases_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAchievementsApi->game_center_achievements_releases_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_live** | [**List[str]**](str.md)| filter by attribute &#39;live&#39; | [optional] 
 **filter_game_center_detail** | [**List[str]**](str.md)| filter by id(s) of related &#39;gameCenterDetail&#39; | [optional] 
 **fields_game_center_achievement_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievementReleases | [optional] 
 **fields_game_center_details** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterDetails | [optional] 
 **fields_game_center_achievements** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievements | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**GameCenterAchievementReleasesResponse**](GameCenterAchievementReleasesResponse.md)

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
**200** | List of GameCenterAchievementReleases |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_achievements_releases_get_to_many_relationship**
> GameCenterAchievementReleasesLinkagesResponse game_center_achievements_releases_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_achievement_releases_linkages_response import GameCenterAchievementReleasesLinkagesResponse
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
    api_instance = openapi_client.GameCenterAchievementsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_achievements_releases_get_to_many_relationship(id, limit=limit)
        print("The response of GameCenterAchievementsApi->game_center_achievements_releases_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAchievementsApi->game_center_achievements_releases_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterAchievementReleasesLinkagesResponse**](GameCenterAchievementReleasesLinkagesResponse.md)

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

# **game_center_achievements_update_instance**
> GameCenterAchievementResponse game_center_achievements_update_instance(id, game_center_achievement_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_achievement_response import GameCenterAchievementResponse
from openapi_client.models.game_center_achievement_update_request import GameCenterAchievementUpdateRequest
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
    api_instance = openapi_client.GameCenterAchievementsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_achievement_update_request = openapi_client.GameCenterAchievementUpdateRequest() # GameCenterAchievementUpdateRequest | GameCenterAchievement representation

    try:
        api_response = api_instance.game_center_achievements_update_instance(id, game_center_achievement_update_request)
        print("The response of GameCenterAchievementsApi->game_center_achievements_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAchievementsApi->game_center_achievements_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_achievement_update_request** | [**GameCenterAchievementUpdateRequest**](GameCenterAchievementUpdateRequest.md)| GameCenterAchievement representation | 

### Return type

[**GameCenterAchievementResponse**](GameCenterAchievementResponse.md)

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
**200** | Single GameCenterAchievement |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

