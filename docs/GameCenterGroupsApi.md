# openapi_client.GameCenterGroupsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**game_center_groups_create_instance**](GameCenterGroupsApi.md#game_center_groups_create_instance) | **POST** /v1/gameCenterGroups | 
[**game_center_groups_delete_instance**](GameCenterGroupsApi.md#game_center_groups_delete_instance) | **DELETE** /v1/gameCenterGroups/{id} | 
[**game_center_groups_game_center_achievements_get_to_many_related**](GameCenterGroupsApi.md#game_center_groups_game_center_achievements_get_to_many_related) | **GET** /v1/gameCenterGroups/{id}/gameCenterAchievements | 
[**game_center_groups_game_center_achievements_get_to_many_relationship**](GameCenterGroupsApi.md#game_center_groups_game_center_achievements_get_to_many_relationship) | **GET** /v1/gameCenterGroups/{id}/relationships/gameCenterAchievements | 
[**game_center_groups_game_center_achievements_replace_to_many_relationship**](GameCenterGroupsApi.md#game_center_groups_game_center_achievements_replace_to_many_relationship) | **PATCH** /v1/gameCenterGroups/{id}/relationships/gameCenterAchievements | 
[**game_center_groups_game_center_activities_get_to_many_related**](GameCenterGroupsApi.md#game_center_groups_game_center_activities_get_to_many_related) | **GET** /v1/gameCenterGroups/{id}/gameCenterActivities | 
[**game_center_groups_game_center_activities_get_to_many_relationship**](GameCenterGroupsApi.md#game_center_groups_game_center_activities_get_to_many_relationship) | **GET** /v1/gameCenterGroups/{id}/relationships/gameCenterActivities | 
[**game_center_groups_game_center_challenges_get_to_many_related**](GameCenterGroupsApi.md#game_center_groups_game_center_challenges_get_to_many_related) | **GET** /v1/gameCenterGroups/{id}/gameCenterChallenges | 
[**game_center_groups_game_center_challenges_get_to_many_relationship**](GameCenterGroupsApi.md#game_center_groups_game_center_challenges_get_to_many_relationship) | **GET** /v1/gameCenterGroups/{id}/relationships/gameCenterChallenges | 
[**game_center_groups_game_center_details_get_to_many_related**](GameCenterGroupsApi.md#game_center_groups_game_center_details_get_to_many_related) | **GET** /v1/gameCenterGroups/{id}/gameCenterDetails | 
[**game_center_groups_game_center_details_get_to_many_relationship**](GameCenterGroupsApi.md#game_center_groups_game_center_details_get_to_many_relationship) | **GET** /v1/gameCenterGroups/{id}/relationships/gameCenterDetails | 
[**game_center_groups_game_center_leaderboard_sets_get_to_many_related**](GameCenterGroupsApi.md#game_center_groups_game_center_leaderboard_sets_get_to_many_related) | **GET** /v1/gameCenterGroups/{id}/gameCenterLeaderboardSets | 
[**game_center_groups_game_center_leaderboard_sets_get_to_many_relationship**](GameCenterGroupsApi.md#game_center_groups_game_center_leaderboard_sets_get_to_many_relationship) | **GET** /v1/gameCenterGroups/{id}/relationships/gameCenterLeaderboardSets | 
[**game_center_groups_game_center_leaderboard_sets_replace_to_many_relationship**](GameCenterGroupsApi.md#game_center_groups_game_center_leaderboard_sets_replace_to_many_relationship) | **PATCH** /v1/gameCenterGroups/{id}/relationships/gameCenterLeaderboardSets | 
[**game_center_groups_game_center_leaderboards_get_to_many_related**](GameCenterGroupsApi.md#game_center_groups_game_center_leaderboards_get_to_many_related) | **GET** /v1/gameCenterGroups/{id}/gameCenterLeaderboards | 
[**game_center_groups_game_center_leaderboards_get_to_many_relationship**](GameCenterGroupsApi.md#game_center_groups_game_center_leaderboards_get_to_many_relationship) | **GET** /v1/gameCenterGroups/{id}/relationships/gameCenterLeaderboards | 
[**game_center_groups_game_center_leaderboards_replace_to_many_relationship**](GameCenterGroupsApi.md#game_center_groups_game_center_leaderboards_replace_to_many_relationship) | **PATCH** /v1/gameCenterGroups/{id}/relationships/gameCenterLeaderboards | 
[**game_center_groups_get_collection**](GameCenterGroupsApi.md#game_center_groups_get_collection) | **GET** /v1/gameCenterGroups | 
[**game_center_groups_get_instance**](GameCenterGroupsApi.md#game_center_groups_get_instance) | **GET** /v1/gameCenterGroups/{id} | 
[**game_center_groups_update_instance**](GameCenterGroupsApi.md#game_center_groups_update_instance) | **PATCH** /v1/gameCenterGroups/{id} | 


# **game_center_groups_create_instance**
> GameCenterGroupResponse game_center_groups_create_instance(game_center_group_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_group_create_request import GameCenterGroupCreateRequest
from openapi_client.models.game_center_group_response import GameCenterGroupResponse
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
    api_instance = openapi_client.GameCenterGroupsApi(api_client)
    game_center_group_create_request = openapi_client.GameCenterGroupCreateRequest() # GameCenterGroupCreateRequest | GameCenterGroup representation

    try:
        api_response = api_instance.game_center_groups_create_instance(game_center_group_create_request)
        print("The response of GameCenterGroupsApi->game_center_groups_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterGroupsApi->game_center_groups_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **game_center_group_create_request** | [**GameCenterGroupCreateRequest**](GameCenterGroupCreateRequest.md)| GameCenterGroup representation | 

### Return type

[**GameCenterGroupResponse**](GameCenterGroupResponse.md)

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
**201** | Single GameCenterGroup |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_groups_delete_instance**
> game_center_groups_delete_instance(id)

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
    api_instance = openapi_client.GameCenterGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.game_center_groups_delete_instance(id)
    except Exception as e:
        print("Exception when calling GameCenterGroupsApi->game_center_groups_delete_instance: %s\n" % e)
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

# **game_center_groups_game_center_achievements_get_to_many_related**
> GameCenterAchievementsResponse game_center_groups_game_center_achievements_get_to_many_related(id, filter_reference_name=filter_reference_name, filter_archived=filter_archived, filter_id=filter_id, fields_game_center_achievements=fields_game_center_achievements, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_achievement_localizations=fields_game_center_achievement_localizations, fields_game_center_achievement_releases=fields_game_center_achievement_releases, fields_game_center_activities=fields_game_center_activities, limit=limit, include=include, limit_localizations=limit_localizations, limit_releases=limit_releases)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_achievements_response import GameCenterAchievementsResponse
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
    api_instance = openapi_client.GameCenterGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_reference_name = ['filter_reference_name_example'] # List[str] | filter by attribute 'referenceName' (optional)
    filter_archived = ['filter_archived_example'] # List[str] | filter by attribute 'archived' (optional)
    filter_id = ['filter_id_example'] # List[str] | filter by id(s) (optional)
    fields_game_center_achievements = ['fields_game_center_achievements_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievements (optional)
    fields_game_center_details = ['fields_game_center_details_example'] # List[str] | the fields to include for returned resources of type gameCenterDetails (optional)
    fields_game_center_groups = ['fields_game_center_groups_example'] # List[str] | the fields to include for returned resources of type gameCenterGroups (optional)
    fields_game_center_achievement_localizations = ['fields_game_center_achievement_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievementLocalizations (optional)
    fields_game_center_achievement_releases = ['fields_game_center_achievement_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievementReleases (optional)
    fields_game_center_activities = ['fields_game_center_activities_example'] # List[str] | the fields to include for returned resources of type gameCenterActivities (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_localizations = 56 # int | maximum number of related localizations returned (when they are included) (optional)
    limit_releases = 56 # int | maximum number of related releases returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_groups_game_center_achievements_get_to_many_related(id, filter_reference_name=filter_reference_name, filter_archived=filter_archived, filter_id=filter_id, fields_game_center_achievements=fields_game_center_achievements, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_achievement_localizations=fields_game_center_achievement_localizations, fields_game_center_achievement_releases=fields_game_center_achievement_releases, fields_game_center_activities=fields_game_center_activities, limit=limit, include=include, limit_localizations=limit_localizations, limit_releases=limit_releases)
        print("The response of GameCenterGroupsApi->game_center_groups_game_center_achievements_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterGroupsApi->game_center_groups_game_center_achievements_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_reference_name** | [**List[str]**](str.md)| filter by attribute &#39;referenceName&#39; | [optional] 
 **filter_archived** | [**List[str]**](str.md)| filter by attribute &#39;archived&#39; | [optional] 
 **filter_id** | [**List[str]**](str.md)| filter by id(s) | [optional] 
 **fields_game_center_achievements** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievements | [optional] 
 **fields_game_center_details** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterDetails | [optional] 
 **fields_game_center_groups** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterGroups | [optional] 
 **fields_game_center_achievement_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional] 
 **fields_game_center_achievement_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievementReleases | [optional] 
 **fields_game_center_activities** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivities | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_localizations** | **int**| maximum number of related localizations returned (when they are included) | [optional] 
 **limit_releases** | **int**| maximum number of related releases returned (when they are included) | [optional] 

### Return type

[**GameCenterAchievementsResponse**](GameCenterAchievementsResponse.md)

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
**200** | List of GameCenterAchievements |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_groups_game_center_achievements_get_to_many_relationship**
> GameCenterGroupGameCenterAchievementsLinkagesResponse game_center_groups_game_center_achievements_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_group_game_center_achievements_linkages_response import GameCenterGroupGameCenterAchievementsLinkagesResponse
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
    api_instance = openapi_client.GameCenterGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_groups_game_center_achievements_get_to_many_relationship(id, limit=limit)
        print("The response of GameCenterGroupsApi->game_center_groups_game_center_achievements_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterGroupsApi->game_center_groups_game_center_achievements_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterGroupGameCenterAchievementsLinkagesResponse**](GameCenterGroupGameCenterAchievementsLinkagesResponse.md)

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

# **game_center_groups_game_center_achievements_replace_to_many_relationship**
> game_center_groups_game_center_achievements_replace_to_many_relationship(id, game_center_group_game_center_achievements_linkages_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_group_game_center_achievements_linkages_request import GameCenterGroupGameCenterAchievementsLinkagesRequest
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
    api_instance = openapi_client.GameCenterGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_group_game_center_achievements_linkages_request = openapi_client.GameCenterGroupGameCenterAchievementsLinkagesRequest() # GameCenterGroupGameCenterAchievementsLinkagesRequest | List of related linkages

    try:
        api_instance.game_center_groups_game_center_achievements_replace_to_many_relationship(id, game_center_group_game_center_achievements_linkages_request)
    except Exception as e:
        print("Exception when calling GameCenterGroupsApi->game_center_groups_game_center_achievements_replace_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_group_game_center_achievements_linkages_request** | [**GameCenterGroupGameCenterAchievementsLinkagesRequest**](GameCenterGroupGameCenterAchievementsLinkagesRequest.md)| List of related linkages | 

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

# **game_center_groups_game_center_activities_get_to_many_related**
> GameCenterActivitiesResponse game_center_groups_game_center_activities_get_to_many_related(id, fields_game_center_activities=fields_game_center_activities, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_achievements=fields_game_center_achievements, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_activity_versions=fields_game_center_activity_versions, limit=limit, include=include, limit_achievements=limit_achievements, limit_leaderboards=limit_leaderboards, limit_versions=limit_versions)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_activities_response import GameCenterActivitiesResponse
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
    api_instance = openapi_client.GameCenterGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_activities = ['fields_game_center_activities_example'] # List[str] | the fields to include for returned resources of type gameCenterActivities (optional)
    fields_game_center_details = ['fields_game_center_details_example'] # List[str] | the fields to include for returned resources of type gameCenterDetails (optional)
    fields_game_center_groups = ['fields_game_center_groups_example'] # List[str] | the fields to include for returned resources of type gameCenterGroups (optional)
    fields_game_center_achievements = ['fields_game_center_achievements_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievements (optional)
    fields_game_center_leaderboards = ['fields_game_center_leaderboards_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboards (optional)
    fields_game_center_activity_versions = ['fields_game_center_activity_versions_example'] # List[str] | the fields to include for returned resources of type gameCenterActivityVersions (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_achievements = 56 # int | maximum number of related achievements returned (when they are included) (optional)
    limit_leaderboards = 56 # int | maximum number of related leaderboards returned (when they are included) (optional)
    limit_versions = 56 # int | maximum number of related versions returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_groups_game_center_activities_get_to_many_related(id, fields_game_center_activities=fields_game_center_activities, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_achievements=fields_game_center_achievements, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_activity_versions=fields_game_center_activity_versions, limit=limit, include=include, limit_achievements=limit_achievements, limit_leaderboards=limit_leaderboards, limit_versions=limit_versions)
        print("The response of GameCenterGroupsApi->game_center_groups_game_center_activities_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterGroupsApi->game_center_groups_game_center_activities_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_activities** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivities | [optional] 
 **fields_game_center_details** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterDetails | [optional] 
 **fields_game_center_groups** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterGroups | [optional] 
 **fields_game_center_achievements** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievements | [optional] 
 **fields_game_center_leaderboards** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboards | [optional] 
 **fields_game_center_activity_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivityVersions | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_achievements** | **int**| maximum number of related achievements returned (when they are included) | [optional] 
 **limit_leaderboards** | **int**| maximum number of related leaderboards returned (when they are included) | [optional] 
 **limit_versions** | **int**| maximum number of related versions returned (when they are included) | [optional] 

### Return type

[**GameCenterActivitiesResponse**](GameCenterActivitiesResponse.md)

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
**200** | List of GameCenterActivities |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_groups_game_center_activities_get_to_many_relationship**
> GameCenterGroupGameCenterActivitiesLinkagesResponse game_center_groups_game_center_activities_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_group_game_center_activities_linkages_response import GameCenterGroupGameCenterActivitiesLinkagesResponse
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
    api_instance = openapi_client.GameCenterGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_groups_game_center_activities_get_to_many_relationship(id, limit=limit)
        print("The response of GameCenterGroupsApi->game_center_groups_game_center_activities_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterGroupsApi->game_center_groups_game_center_activities_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterGroupGameCenterActivitiesLinkagesResponse**](GameCenterGroupGameCenterActivitiesLinkagesResponse.md)

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

# **game_center_groups_game_center_challenges_get_to_many_related**
> GameCenterChallengesResponse game_center_groups_game_center_challenges_get_to_many_related(id, filter_reference_name=filter_reference_name, filter_archived=filter_archived, filter_id=filter_id, fields_game_center_challenges=fields_game_center_challenges, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_challenge_versions=fields_game_center_challenge_versions, fields_game_center_leaderboards=fields_game_center_leaderboards, limit=limit, include=include, limit_versions=limit_versions)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_challenges_response import GameCenterChallengesResponse
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
    api_instance = openapi_client.GameCenterGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_reference_name = ['filter_reference_name_example'] # List[str] | filter by attribute 'referenceName' (optional)
    filter_archived = ['filter_archived_example'] # List[str] | filter by attribute 'archived' (optional)
    filter_id = ['filter_id_example'] # List[str] | filter by id(s) (optional)
    fields_game_center_challenges = ['fields_game_center_challenges_example'] # List[str] | the fields to include for returned resources of type gameCenterChallenges (optional)
    fields_game_center_details = ['fields_game_center_details_example'] # List[str] | the fields to include for returned resources of type gameCenterDetails (optional)
    fields_game_center_groups = ['fields_game_center_groups_example'] # List[str] | the fields to include for returned resources of type gameCenterGroups (optional)
    fields_game_center_challenge_versions = ['fields_game_center_challenge_versions_example'] # List[str] | the fields to include for returned resources of type gameCenterChallengeVersions (optional)
    fields_game_center_leaderboards = ['fields_game_center_leaderboards_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboards (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_versions = 56 # int | maximum number of related versions returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_groups_game_center_challenges_get_to_many_related(id, filter_reference_name=filter_reference_name, filter_archived=filter_archived, filter_id=filter_id, fields_game_center_challenges=fields_game_center_challenges, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_challenge_versions=fields_game_center_challenge_versions, fields_game_center_leaderboards=fields_game_center_leaderboards, limit=limit, include=include, limit_versions=limit_versions)
        print("The response of GameCenterGroupsApi->game_center_groups_game_center_challenges_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterGroupsApi->game_center_groups_game_center_challenges_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_reference_name** | [**List[str]**](str.md)| filter by attribute &#39;referenceName&#39; | [optional] 
 **filter_archived** | [**List[str]**](str.md)| filter by attribute &#39;archived&#39; | [optional] 
 **filter_id** | [**List[str]**](str.md)| filter by id(s) | [optional] 
 **fields_game_center_challenges** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallenges | [optional] 
 **fields_game_center_details** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterDetails | [optional] 
 **fields_game_center_groups** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterGroups | [optional] 
 **fields_game_center_challenge_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallengeVersions | [optional] 
 **fields_game_center_leaderboards** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboards | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_versions** | **int**| maximum number of related versions returned (when they are included) | [optional] 

### Return type

[**GameCenterChallengesResponse**](GameCenterChallengesResponse.md)

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
**200** | List of GameCenterChallenges |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_groups_game_center_challenges_get_to_many_relationship**
> GameCenterGroupGameCenterChallengesLinkagesResponse game_center_groups_game_center_challenges_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_group_game_center_challenges_linkages_response import GameCenterGroupGameCenterChallengesLinkagesResponse
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
    api_instance = openapi_client.GameCenterGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_groups_game_center_challenges_get_to_many_relationship(id, limit=limit)
        print("The response of GameCenterGroupsApi->game_center_groups_game_center_challenges_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterGroupsApi->game_center_groups_game_center_challenges_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterGroupGameCenterChallengesLinkagesResponse**](GameCenterGroupGameCenterChallengesLinkagesResponse.md)

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

# **game_center_groups_game_center_details_get_to_many_related**
> GameCenterDetailsResponse game_center_groups_game_center_details_get_to_many_related(id, filter_game_center_app_versions_enabled=filter_game_center_app_versions_enabled, fields_game_center_details=fields_game_center_details, fields_apps=fields_apps, fields_game_center_app_versions=fields_game_center_app_versions, fields_game_center_groups=fields_game_center_groups, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_achievements=fields_game_center_achievements, fields_game_center_activities=fields_game_center_activities, fields_game_center_challenges=fields_game_center_challenges, fields_game_center_achievement_releases=fields_game_center_achievement_releases, fields_game_center_activity_version_releases=fields_game_center_activity_version_releases, fields_game_center_challenge_version_releases=fields_game_center_challenge_version_releases, fields_game_center_leaderboard_releases=fields_game_center_leaderboard_releases, fields_game_center_leaderboard_set_releases=fields_game_center_leaderboard_set_releases, fields_app_store_versions=fields_app_store_versions, limit=limit, include=include, limit_game_center_app_versions=limit_game_center_app_versions, limit_game_center_leaderboards=limit_game_center_leaderboards, limit_game_center_leaderboard_sets=limit_game_center_leaderboard_sets, limit_game_center_achievements=limit_game_center_achievements, limit_game_center_activities=limit_game_center_activities, limit_game_center_challenges=limit_game_center_challenges, limit_achievement_releases=limit_achievement_releases, limit_activity_releases=limit_activity_releases, limit_challenge_releases=limit_challenge_releases, limit_leaderboard_releases=limit_leaderboard_releases, limit_leaderboard_set_releases=limit_leaderboard_set_releases, limit_challenges_minimum_platform_versions=limit_challenges_minimum_platform_versions)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_details_response import GameCenterDetailsResponse
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
    api_instance = openapi_client.GameCenterGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_game_center_app_versions_enabled = ['filter_game_center_app_versions_enabled_example'] # List[str] | filter by attribute 'gameCenterAppVersions.enabled' (optional)
    fields_game_center_details = ['fields_game_center_details_example'] # List[str] | the fields to include for returned resources of type gameCenterDetails (optional)
    fields_apps = ['fields_apps_example'] # List[str] | the fields to include for returned resources of type apps (optional)
    fields_game_center_app_versions = ['fields_game_center_app_versions_example'] # List[str] | the fields to include for returned resources of type gameCenterAppVersions (optional)
    fields_game_center_groups = ['fields_game_center_groups_example'] # List[str] | the fields to include for returned resources of type gameCenterGroups (optional)
    fields_game_center_leaderboards = ['fields_game_center_leaderboards_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboards (optional)
    fields_game_center_leaderboard_sets = ['fields_game_center_leaderboard_sets_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSets (optional)
    fields_game_center_achievements = ['fields_game_center_achievements_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievements (optional)
    fields_game_center_activities = ['fields_game_center_activities_example'] # List[str] | the fields to include for returned resources of type gameCenterActivities (optional)
    fields_game_center_challenges = ['fields_game_center_challenges_example'] # List[str] | the fields to include for returned resources of type gameCenterChallenges (optional)
    fields_game_center_achievement_releases = ['fields_game_center_achievement_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievementReleases (optional)
    fields_game_center_activity_version_releases = ['fields_game_center_activity_version_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterActivityVersionReleases (optional)
    fields_game_center_challenge_version_releases = ['fields_game_center_challenge_version_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterChallengeVersionReleases (optional)
    fields_game_center_leaderboard_releases = ['fields_game_center_leaderboard_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardReleases (optional)
    fields_game_center_leaderboard_set_releases = ['fields_game_center_leaderboard_set_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSetReleases (optional)
    fields_app_store_versions = ['fields_app_store_versions_example'] # List[str] | the fields to include for returned resources of type appStoreVersions (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_game_center_app_versions = 56 # int | maximum number of related gameCenterAppVersions returned (when they are included) (optional)
    limit_game_center_leaderboards = 56 # int | maximum number of related gameCenterLeaderboards returned (when they are included) (optional)
    limit_game_center_leaderboard_sets = 56 # int | maximum number of related gameCenterLeaderboardSets returned (when they are included) (optional)
    limit_game_center_achievements = 56 # int | maximum number of related gameCenterAchievements returned (when they are included) (optional)
    limit_game_center_activities = 56 # int | maximum number of related gameCenterActivities returned (when they are included) (optional)
    limit_game_center_challenges = 56 # int | maximum number of related gameCenterChallenges returned (when they are included) (optional)
    limit_achievement_releases = 56 # int | maximum number of related achievementReleases returned (when they are included) (optional)
    limit_activity_releases = 56 # int | maximum number of related activityReleases returned (when they are included) (optional)
    limit_challenge_releases = 56 # int | maximum number of related challengeReleases returned (when they are included) (optional)
    limit_leaderboard_releases = 56 # int | maximum number of related leaderboardReleases returned (when they are included) (optional)
    limit_leaderboard_set_releases = 56 # int | maximum number of related leaderboardSetReleases returned (when they are included) (optional)
    limit_challenges_minimum_platform_versions = 56 # int | maximum number of related challengesMinimumPlatformVersions returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_groups_game_center_details_get_to_many_related(id, filter_game_center_app_versions_enabled=filter_game_center_app_versions_enabled, fields_game_center_details=fields_game_center_details, fields_apps=fields_apps, fields_game_center_app_versions=fields_game_center_app_versions, fields_game_center_groups=fields_game_center_groups, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_achievements=fields_game_center_achievements, fields_game_center_activities=fields_game_center_activities, fields_game_center_challenges=fields_game_center_challenges, fields_game_center_achievement_releases=fields_game_center_achievement_releases, fields_game_center_activity_version_releases=fields_game_center_activity_version_releases, fields_game_center_challenge_version_releases=fields_game_center_challenge_version_releases, fields_game_center_leaderboard_releases=fields_game_center_leaderboard_releases, fields_game_center_leaderboard_set_releases=fields_game_center_leaderboard_set_releases, fields_app_store_versions=fields_app_store_versions, limit=limit, include=include, limit_game_center_app_versions=limit_game_center_app_versions, limit_game_center_leaderboards=limit_game_center_leaderboards, limit_game_center_leaderboard_sets=limit_game_center_leaderboard_sets, limit_game_center_achievements=limit_game_center_achievements, limit_game_center_activities=limit_game_center_activities, limit_game_center_challenges=limit_game_center_challenges, limit_achievement_releases=limit_achievement_releases, limit_activity_releases=limit_activity_releases, limit_challenge_releases=limit_challenge_releases, limit_leaderboard_releases=limit_leaderboard_releases, limit_leaderboard_set_releases=limit_leaderboard_set_releases, limit_challenges_minimum_platform_versions=limit_challenges_minimum_platform_versions)
        print("The response of GameCenterGroupsApi->game_center_groups_game_center_details_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterGroupsApi->game_center_groups_game_center_details_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_game_center_app_versions_enabled** | [**List[str]**](str.md)| filter by attribute &#39;gameCenterAppVersions.enabled&#39; | [optional] 
 **fields_game_center_details** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterDetails | [optional] 
 **fields_apps** | [**List[str]**](str.md)| the fields to include for returned resources of type apps | [optional] 
 **fields_game_center_app_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAppVersions | [optional] 
 **fields_game_center_groups** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterGroups | [optional] 
 **fields_game_center_leaderboards** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboards | [optional] 
 **fields_game_center_leaderboard_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSets | [optional] 
 **fields_game_center_achievements** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievements | [optional] 
 **fields_game_center_activities** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivities | [optional] 
 **fields_game_center_challenges** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallenges | [optional] 
 **fields_game_center_achievement_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievementReleases | [optional] 
 **fields_game_center_activity_version_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivityVersionReleases | [optional] 
 **fields_game_center_challenge_version_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallengeVersionReleases | [optional] 
 **fields_game_center_leaderboard_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardReleases | [optional] 
 **fields_game_center_leaderboard_set_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSetReleases | [optional] 
 **fields_app_store_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersions | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_game_center_app_versions** | **int**| maximum number of related gameCenterAppVersions returned (when they are included) | [optional] 
 **limit_game_center_leaderboards** | **int**| maximum number of related gameCenterLeaderboards returned (when they are included) | [optional] 
 **limit_game_center_leaderboard_sets** | **int**| maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional] 
 **limit_game_center_achievements** | **int**| maximum number of related gameCenterAchievements returned (when they are included) | [optional] 
 **limit_game_center_activities** | **int**| maximum number of related gameCenterActivities returned (when they are included) | [optional] 
 **limit_game_center_challenges** | **int**| maximum number of related gameCenterChallenges returned (when they are included) | [optional] 
 **limit_achievement_releases** | **int**| maximum number of related achievementReleases returned (when they are included) | [optional] 
 **limit_activity_releases** | **int**| maximum number of related activityReleases returned (when they are included) | [optional] 
 **limit_challenge_releases** | **int**| maximum number of related challengeReleases returned (when they are included) | [optional] 
 **limit_leaderboard_releases** | **int**| maximum number of related leaderboardReleases returned (when they are included) | [optional] 
 **limit_leaderboard_set_releases** | **int**| maximum number of related leaderboardSetReleases returned (when they are included) | [optional] 
 **limit_challenges_minimum_platform_versions** | **int**| maximum number of related challengesMinimumPlatformVersions returned (when they are included) | [optional] 

### Return type

[**GameCenterDetailsResponse**](GameCenterDetailsResponse.md)

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
**200** | List of GameCenterDetails |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_groups_game_center_details_get_to_many_relationship**
> GameCenterGroupGameCenterDetailsLinkagesResponse game_center_groups_game_center_details_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_group_game_center_details_linkages_response import GameCenterGroupGameCenterDetailsLinkagesResponse
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
    api_instance = openapi_client.GameCenterGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_groups_game_center_details_get_to_many_relationship(id, limit=limit)
        print("The response of GameCenterGroupsApi->game_center_groups_game_center_details_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterGroupsApi->game_center_groups_game_center_details_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterGroupGameCenterDetailsLinkagesResponse**](GameCenterGroupGameCenterDetailsLinkagesResponse.md)

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

# **game_center_groups_game_center_leaderboard_sets_get_to_many_related**
> GameCenterLeaderboardSetsResponse game_center_groups_game_center_leaderboard_sets_get_to_many_related(id, filter_reference_name=filter_reference_name, filter_id=filter_id, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_leaderboard_set_localizations=fields_game_center_leaderboard_set_localizations, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_leaderboard_set_releases=fields_game_center_leaderboard_set_releases, limit=limit, include=include, limit_localizations=limit_localizations, limit_game_center_leaderboards=limit_game_center_leaderboards, limit_releases=limit_releases)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_sets_response import GameCenterLeaderboardSetsResponse
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
    api_instance = openapi_client.GameCenterGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_reference_name = ['filter_reference_name_example'] # List[str] | filter by attribute 'referenceName' (optional)
    filter_id = ['filter_id_example'] # List[str] | filter by id(s) (optional)
    fields_game_center_leaderboard_sets = ['fields_game_center_leaderboard_sets_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSets (optional)
    fields_game_center_details = ['fields_game_center_details_example'] # List[str] | the fields to include for returned resources of type gameCenterDetails (optional)
    fields_game_center_groups = ['fields_game_center_groups_example'] # List[str] | the fields to include for returned resources of type gameCenterGroups (optional)
    fields_game_center_leaderboard_set_localizations = ['fields_game_center_leaderboard_set_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations (optional)
    fields_game_center_leaderboards = ['fields_game_center_leaderboards_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboards (optional)
    fields_game_center_leaderboard_set_releases = ['fields_game_center_leaderboard_set_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSetReleases (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_localizations = 56 # int | maximum number of related localizations returned (when they are included) (optional)
    limit_game_center_leaderboards = 56 # int | maximum number of related gameCenterLeaderboards returned (when they are included) (optional)
    limit_releases = 56 # int | maximum number of related releases returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_groups_game_center_leaderboard_sets_get_to_many_related(id, filter_reference_name=filter_reference_name, filter_id=filter_id, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_leaderboard_set_localizations=fields_game_center_leaderboard_set_localizations, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_leaderboard_set_releases=fields_game_center_leaderboard_set_releases, limit=limit, include=include, limit_localizations=limit_localizations, limit_game_center_leaderboards=limit_game_center_leaderboards, limit_releases=limit_releases)
        print("The response of GameCenterGroupsApi->game_center_groups_game_center_leaderboard_sets_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterGroupsApi->game_center_groups_game_center_leaderboard_sets_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_reference_name** | [**List[str]**](str.md)| filter by attribute &#39;referenceName&#39; | [optional] 
 **filter_id** | [**List[str]**](str.md)| filter by id(s) | [optional] 
 **fields_game_center_leaderboard_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSets | [optional] 
 **fields_game_center_details** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterDetails | [optional] 
 **fields_game_center_groups** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterGroups | [optional] 
 **fields_game_center_leaderboard_set_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional] 
 **fields_game_center_leaderboards** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboards | [optional] 
 **fields_game_center_leaderboard_set_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSetReleases | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_localizations** | **int**| maximum number of related localizations returned (when they are included) | [optional] 
 **limit_game_center_leaderboards** | **int**| maximum number of related gameCenterLeaderboards returned (when they are included) | [optional] 
 **limit_releases** | **int**| maximum number of related releases returned (when they are included) | [optional] 

### Return type

[**GameCenterLeaderboardSetsResponse**](GameCenterLeaderboardSetsResponse.md)

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
**200** | List of GameCenterLeaderboardSets |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_groups_game_center_leaderboard_sets_get_to_many_relationship**
> GameCenterGroupGameCenterLeaderboardSetsLinkagesResponse game_center_groups_game_center_leaderboard_sets_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_group_game_center_leaderboard_sets_linkages_response import GameCenterGroupGameCenterLeaderboardSetsLinkagesResponse
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
    api_instance = openapi_client.GameCenterGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_groups_game_center_leaderboard_sets_get_to_many_relationship(id, limit=limit)
        print("The response of GameCenterGroupsApi->game_center_groups_game_center_leaderboard_sets_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterGroupsApi->game_center_groups_game_center_leaderboard_sets_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterGroupGameCenterLeaderboardSetsLinkagesResponse**](GameCenterGroupGameCenterLeaderboardSetsLinkagesResponse.md)

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

# **game_center_groups_game_center_leaderboard_sets_replace_to_many_relationship**
> game_center_groups_game_center_leaderboard_sets_replace_to_many_relationship(id, game_center_group_game_center_leaderboard_sets_linkages_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_group_game_center_leaderboard_sets_linkages_request import GameCenterGroupGameCenterLeaderboardSetsLinkagesRequest
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
    api_instance = openapi_client.GameCenterGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_group_game_center_leaderboard_sets_linkages_request = openapi_client.GameCenterGroupGameCenterLeaderboardSetsLinkagesRequest() # GameCenterGroupGameCenterLeaderboardSetsLinkagesRequest | List of related linkages

    try:
        api_instance.game_center_groups_game_center_leaderboard_sets_replace_to_many_relationship(id, game_center_group_game_center_leaderboard_sets_linkages_request)
    except Exception as e:
        print("Exception when calling GameCenterGroupsApi->game_center_groups_game_center_leaderboard_sets_replace_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_group_game_center_leaderboard_sets_linkages_request** | [**GameCenterGroupGameCenterLeaderboardSetsLinkagesRequest**](GameCenterGroupGameCenterLeaderboardSetsLinkagesRequest.md)| List of related linkages | 

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

# **game_center_groups_game_center_leaderboards_get_to_many_related**
> GameCenterLeaderboardsResponse game_center_groups_game_center_leaderboards_get_to_many_related(id, filter_reference_name=filter_reference_name, filter_archived=filter_archived, filter_id=filter_id, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_leaderboard_localizations=fields_game_center_leaderboard_localizations, fields_game_center_leaderboard_releases=fields_game_center_leaderboard_releases, fields_game_center_activities=fields_game_center_activities, fields_game_center_challenges=fields_game_center_challenges, limit=limit, include=include, limit_game_center_leaderboard_sets=limit_game_center_leaderboard_sets, limit_localizations=limit_localizations, limit_releases=limit_releases)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboards_response import GameCenterLeaderboardsResponse
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
    api_instance = openapi_client.GameCenterGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_reference_name = ['filter_reference_name_example'] # List[str] | filter by attribute 'referenceName' (optional)
    filter_archived = ['filter_archived_example'] # List[str] | filter by attribute 'archived' (optional)
    filter_id = ['filter_id_example'] # List[str] | filter by id(s) (optional)
    fields_game_center_leaderboards = ['fields_game_center_leaderboards_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboards (optional)
    fields_game_center_details = ['fields_game_center_details_example'] # List[str] | the fields to include for returned resources of type gameCenterDetails (optional)
    fields_game_center_groups = ['fields_game_center_groups_example'] # List[str] | the fields to include for returned resources of type gameCenterGroups (optional)
    fields_game_center_leaderboard_sets = ['fields_game_center_leaderboard_sets_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSets (optional)
    fields_game_center_leaderboard_localizations = ['fields_game_center_leaderboard_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardLocalizations (optional)
    fields_game_center_leaderboard_releases = ['fields_game_center_leaderboard_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardReleases (optional)
    fields_game_center_activities = ['fields_game_center_activities_example'] # List[str] | the fields to include for returned resources of type gameCenterActivities (optional)
    fields_game_center_challenges = ['fields_game_center_challenges_example'] # List[str] | the fields to include for returned resources of type gameCenterChallenges (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_game_center_leaderboard_sets = 56 # int | maximum number of related gameCenterLeaderboardSets returned (when they are included) (optional)
    limit_localizations = 56 # int | maximum number of related localizations returned (when they are included) (optional)
    limit_releases = 56 # int | maximum number of related releases returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_groups_game_center_leaderboards_get_to_many_related(id, filter_reference_name=filter_reference_name, filter_archived=filter_archived, filter_id=filter_id, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_leaderboard_localizations=fields_game_center_leaderboard_localizations, fields_game_center_leaderboard_releases=fields_game_center_leaderboard_releases, fields_game_center_activities=fields_game_center_activities, fields_game_center_challenges=fields_game_center_challenges, limit=limit, include=include, limit_game_center_leaderboard_sets=limit_game_center_leaderboard_sets, limit_localizations=limit_localizations, limit_releases=limit_releases)
        print("The response of GameCenterGroupsApi->game_center_groups_game_center_leaderboards_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterGroupsApi->game_center_groups_game_center_leaderboards_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_reference_name** | [**List[str]**](str.md)| filter by attribute &#39;referenceName&#39; | [optional] 
 **filter_archived** | [**List[str]**](str.md)| filter by attribute &#39;archived&#39; | [optional] 
 **filter_id** | [**List[str]**](str.md)| filter by id(s) | [optional] 
 **fields_game_center_leaderboards** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboards | [optional] 
 **fields_game_center_details** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterDetails | [optional] 
 **fields_game_center_groups** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterGroups | [optional] 
 **fields_game_center_leaderboard_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSets | [optional] 
 **fields_game_center_leaderboard_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional] 
 **fields_game_center_leaderboard_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardReleases | [optional] 
 **fields_game_center_activities** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivities | [optional] 
 **fields_game_center_challenges** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallenges | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_game_center_leaderboard_sets** | **int**| maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional] 
 **limit_localizations** | **int**| maximum number of related localizations returned (when they are included) | [optional] 
 **limit_releases** | **int**| maximum number of related releases returned (when they are included) | [optional] 

### Return type

[**GameCenterLeaderboardsResponse**](GameCenterLeaderboardsResponse.md)

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
**200** | List of GameCenterLeaderboards |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_groups_game_center_leaderboards_get_to_many_relationship**
> GameCenterGroupGameCenterLeaderboardsLinkagesResponse game_center_groups_game_center_leaderboards_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_group_game_center_leaderboards_linkages_response import GameCenterGroupGameCenterLeaderboardsLinkagesResponse
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
    api_instance = openapi_client.GameCenterGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_groups_game_center_leaderboards_get_to_many_relationship(id, limit=limit)
        print("The response of GameCenterGroupsApi->game_center_groups_game_center_leaderboards_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterGroupsApi->game_center_groups_game_center_leaderboards_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterGroupGameCenterLeaderboardsLinkagesResponse**](GameCenterGroupGameCenterLeaderboardsLinkagesResponse.md)

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

# **game_center_groups_game_center_leaderboards_replace_to_many_relationship**
> game_center_groups_game_center_leaderboards_replace_to_many_relationship(id, game_center_group_game_center_leaderboards_linkages_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_group_game_center_leaderboards_linkages_request import GameCenterGroupGameCenterLeaderboardsLinkagesRequest
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
    api_instance = openapi_client.GameCenterGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_group_game_center_leaderboards_linkages_request = openapi_client.GameCenterGroupGameCenterLeaderboardsLinkagesRequest() # GameCenterGroupGameCenterLeaderboardsLinkagesRequest | List of related linkages

    try:
        api_instance.game_center_groups_game_center_leaderboards_replace_to_many_relationship(id, game_center_group_game_center_leaderboards_linkages_request)
    except Exception as e:
        print("Exception when calling GameCenterGroupsApi->game_center_groups_game_center_leaderboards_replace_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_group_game_center_leaderboards_linkages_request** | [**GameCenterGroupGameCenterLeaderboardsLinkagesRequest**](GameCenterGroupGameCenterLeaderboardsLinkagesRequest.md)| List of related linkages | 

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

# **game_center_groups_get_collection**
> GameCenterGroupsResponse game_center_groups_get_collection(filter_game_center_details=filter_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_details=fields_game_center_details, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_achievements=fields_game_center_achievements, fields_game_center_activities=fields_game_center_activities, fields_game_center_challenges=fields_game_center_challenges, limit=limit, include=include, limit_game_center_achievements=limit_game_center_achievements, limit_game_center_activities=limit_game_center_activities, limit_game_center_challenges=limit_game_center_challenges, limit_game_center_details=limit_game_center_details, limit_game_center_leaderboard_sets=limit_game_center_leaderboard_sets, limit_game_center_leaderboards=limit_game_center_leaderboards)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_groups_response import GameCenterGroupsResponse
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
    api_instance = openapi_client.GameCenterGroupsApi(api_client)
    filter_game_center_details = ['filter_game_center_details_example'] # List[str] | filter by id(s) of related 'gameCenterDetails' (optional)
    fields_game_center_groups = ['fields_game_center_groups_example'] # List[str] | the fields to include for returned resources of type gameCenterGroups (optional)
    fields_game_center_details = ['fields_game_center_details_example'] # List[str] | the fields to include for returned resources of type gameCenterDetails (optional)
    fields_game_center_leaderboards = ['fields_game_center_leaderboards_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboards (optional)
    fields_game_center_leaderboard_sets = ['fields_game_center_leaderboard_sets_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSets (optional)
    fields_game_center_achievements = ['fields_game_center_achievements_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievements (optional)
    fields_game_center_activities = ['fields_game_center_activities_example'] # List[str] | the fields to include for returned resources of type gameCenterActivities (optional)
    fields_game_center_challenges = ['fields_game_center_challenges_example'] # List[str] | the fields to include for returned resources of type gameCenterChallenges (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_game_center_achievements = 56 # int | maximum number of related gameCenterAchievements returned (when they are included) (optional)
    limit_game_center_activities = 56 # int | maximum number of related gameCenterActivities returned (when they are included) (optional)
    limit_game_center_challenges = 56 # int | maximum number of related gameCenterChallenges returned (when they are included) (optional)
    limit_game_center_details = 56 # int | maximum number of related gameCenterDetails returned (when they are included) (optional)
    limit_game_center_leaderboard_sets = 56 # int | maximum number of related gameCenterLeaderboardSets returned (when they are included) (optional)
    limit_game_center_leaderboards = 56 # int | maximum number of related gameCenterLeaderboards returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_groups_get_collection(filter_game_center_details=filter_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_details=fields_game_center_details, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_achievements=fields_game_center_achievements, fields_game_center_activities=fields_game_center_activities, fields_game_center_challenges=fields_game_center_challenges, limit=limit, include=include, limit_game_center_achievements=limit_game_center_achievements, limit_game_center_activities=limit_game_center_activities, limit_game_center_challenges=limit_game_center_challenges, limit_game_center_details=limit_game_center_details, limit_game_center_leaderboard_sets=limit_game_center_leaderboard_sets, limit_game_center_leaderboards=limit_game_center_leaderboards)
        print("The response of GameCenterGroupsApi->game_center_groups_get_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterGroupsApi->game_center_groups_get_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter_game_center_details** | [**List[str]**](str.md)| filter by id(s) of related &#39;gameCenterDetails&#39; | [optional] 
 **fields_game_center_groups** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterGroups | [optional] 
 **fields_game_center_details** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterDetails | [optional] 
 **fields_game_center_leaderboards** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboards | [optional] 
 **fields_game_center_leaderboard_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSets | [optional] 
 **fields_game_center_achievements** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievements | [optional] 
 **fields_game_center_activities** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivities | [optional] 
 **fields_game_center_challenges** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallenges | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_game_center_achievements** | **int**| maximum number of related gameCenterAchievements returned (when they are included) | [optional] 
 **limit_game_center_activities** | **int**| maximum number of related gameCenterActivities returned (when they are included) | [optional] 
 **limit_game_center_challenges** | **int**| maximum number of related gameCenterChallenges returned (when they are included) | [optional] 
 **limit_game_center_details** | **int**| maximum number of related gameCenterDetails returned (when they are included) | [optional] 
 **limit_game_center_leaderboard_sets** | **int**| maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional] 
 **limit_game_center_leaderboards** | **int**| maximum number of related gameCenterLeaderboards returned (when they are included) | [optional] 

### Return type

[**GameCenterGroupsResponse**](GameCenterGroupsResponse.md)

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
**200** | List of GameCenterGroups |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_groups_get_instance**
> GameCenterGroupResponse game_center_groups_get_instance(id, fields_game_center_groups=fields_game_center_groups, fields_game_center_details=fields_game_center_details, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_achievements=fields_game_center_achievements, fields_game_center_activities=fields_game_center_activities, fields_game_center_challenges=fields_game_center_challenges, include=include, limit_game_center_achievements=limit_game_center_achievements, limit_game_center_activities=limit_game_center_activities, limit_game_center_challenges=limit_game_center_challenges, limit_game_center_details=limit_game_center_details, limit_game_center_leaderboard_sets=limit_game_center_leaderboard_sets, limit_game_center_leaderboards=limit_game_center_leaderboards)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_group_response import GameCenterGroupResponse
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
    api_instance = openapi_client.GameCenterGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_groups = ['fields_game_center_groups_example'] # List[str] | the fields to include for returned resources of type gameCenterGroups (optional)
    fields_game_center_details = ['fields_game_center_details_example'] # List[str] | the fields to include for returned resources of type gameCenterDetails (optional)
    fields_game_center_leaderboards = ['fields_game_center_leaderboards_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboards (optional)
    fields_game_center_leaderboard_sets = ['fields_game_center_leaderboard_sets_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSets (optional)
    fields_game_center_achievements = ['fields_game_center_achievements_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievements (optional)
    fields_game_center_activities = ['fields_game_center_activities_example'] # List[str] | the fields to include for returned resources of type gameCenterActivities (optional)
    fields_game_center_challenges = ['fields_game_center_challenges_example'] # List[str] | the fields to include for returned resources of type gameCenterChallenges (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_game_center_achievements = 56 # int | maximum number of related gameCenterAchievements returned (when they are included) (optional)
    limit_game_center_activities = 56 # int | maximum number of related gameCenterActivities returned (when they are included) (optional)
    limit_game_center_challenges = 56 # int | maximum number of related gameCenterChallenges returned (when they are included) (optional)
    limit_game_center_details = 56 # int | maximum number of related gameCenterDetails returned (when they are included) (optional)
    limit_game_center_leaderboard_sets = 56 # int | maximum number of related gameCenterLeaderboardSets returned (when they are included) (optional)
    limit_game_center_leaderboards = 56 # int | maximum number of related gameCenterLeaderboards returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_groups_get_instance(id, fields_game_center_groups=fields_game_center_groups, fields_game_center_details=fields_game_center_details, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_achievements=fields_game_center_achievements, fields_game_center_activities=fields_game_center_activities, fields_game_center_challenges=fields_game_center_challenges, include=include, limit_game_center_achievements=limit_game_center_achievements, limit_game_center_activities=limit_game_center_activities, limit_game_center_challenges=limit_game_center_challenges, limit_game_center_details=limit_game_center_details, limit_game_center_leaderboard_sets=limit_game_center_leaderboard_sets, limit_game_center_leaderboards=limit_game_center_leaderboards)
        print("The response of GameCenterGroupsApi->game_center_groups_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterGroupsApi->game_center_groups_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_groups** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterGroups | [optional] 
 **fields_game_center_details** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterDetails | [optional] 
 **fields_game_center_leaderboards** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboards | [optional] 
 **fields_game_center_leaderboard_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSets | [optional] 
 **fields_game_center_achievements** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievements | [optional] 
 **fields_game_center_activities** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivities | [optional] 
 **fields_game_center_challenges** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallenges | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_game_center_achievements** | **int**| maximum number of related gameCenterAchievements returned (when they are included) | [optional] 
 **limit_game_center_activities** | **int**| maximum number of related gameCenterActivities returned (when they are included) | [optional] 
 **limit_game_center_challenges** | **int**| maximum number of related gameCenterChallenges returned (when they are included) | [optional] 
 **limit_game_center_details** | **int**| maximum number of related gameCenterDetails returned (when they are included) | [optional] 
 **limit_game_center_leaderboard_sets** | **int**| maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional] 
 **limit_game_center_leaderboards** | **int**| maximum number of related gameCenterLeaderboards returned (when they are included) | [optional] 

### Return type

[**GameCenterGroupResponse**](GameCenterGroupResponse.md)

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
**200** | Single GameCenterGroup |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_groups_update_instance**
> GameCenterGroupResponse game_center_groups_update_instance(id, game_center_group_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_group_response import GameCenterGroupResponse
from openapi_client.models.game_center_group_update_request import GameCenterGroupUpdateRequest
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
    api_instance = openapi_client.GameCenterGroupsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_group_update_request = openapi_client.GameCenterGroupUpdateRequest() # GameCenterGroupUpdateRequest | GameCenterGroup representation

    try:
        api_response = api_instance.game_center_groups_update_instance(id, game_center_group_update_request)
        print("The response of GameCenterGroupsApi->game_center_groups_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterGroupsApi->game_center_groups_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_group_update_request** | [**GameCenterGroupUpdateRequest**](GameCenterGroupUpdateRequest.md)| GameCenterGroup representation | 

### Return type

[**GameCenterGroupResponse**](GameCenterGroupResponse.md)

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
**200** | Single GameCenterGroup |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

