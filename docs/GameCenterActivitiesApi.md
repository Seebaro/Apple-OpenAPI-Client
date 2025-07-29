# openapi_client.GameCenterActivitiesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**game_center_activities_achievements_create_to_many_relationship**](GameCenterActivitiesApi.md#game_center_activities_achievements_create_to_many_relationship) | **POST** /v1/gameCenterActivities/{id}/relationships/achievements | 
[**game_center_activities_achievements_delete_to_many_relationship**](GameCenterActivitiesApi.md#game_center_activities_achievements_delete_to_many_relationship) | **DELETE** /v1/gameCenterActivities/{id}/relationships/achievements | 
[**game_center_activities_create_instance**](GameCenterActivitiesApi.md#game_center_activities_create_instance) | **POST** /v1/gameCenterActivities | 
[**game_center_activities_delete_instance**](GameCenterActivitiesApi.md#game_center_activities_delete_instance) | **DELETE** /v1/gameCenterActivities/{id} | 
[**game_center_activities_get_instance**](GameCenterActivitiesApi.md#game_center_activities_get_instance) | **GET** /v1/gameCenterActivities/{id} | 
[**game_center_activities_leaderboards_create_to_many_relationship**](GameCenterActivitiesApi.md#game_center_activities_leaderboards_create_to_many_relationship) | **POST** /v1/gameCenterActivities/{id}/relationships/leaderboards | 
[**game_center_activities_leaderboards_delete_to_many_relationship**](GameCenterActivitiesApi.md#game_center_activities_leaderboards_delete_to_many_relationship) | **DELETE** /v1/gameCenterActivities/{id}/relationships/leaderboards | 
[**game_center_activities_update_instance**](GameCenterActivitiesApi.md#game_center_activities_update_instance) | **PATCH** /v1/gameCenterActivities/{id} | 
[**game_center_activities_versions_get_to_many_related**](GameCenterActivitiesApi.md#game_center_activities_versions_get_to_many_related) | **GET** /v1/gameCenterActivities/{id}/versions | 
[**game_center_activities_versions_get_to_many_relationship**](GameCenterActivitiesApi.md#game_center_activities_versions_get_to_many_relationship) | **GET** /v1/gameCenterActivities/{id}/relationships/versions | 


# **game_center_activities_achievements_create_to_many_relationship**
> game_center_activities_achievements_create_to_many_relationship(id, game_center_activity_achievements_linkages_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_activity_achievements_linkages_request import GameCenterActivityAchievementsLinkagesRequest
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
    api_instance = openapi_client.GameCenterActivitiesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_activity_achievements_linkages_request = openapi_client.GameCenterActivityAchievementsLinkagesRequest() # GameCenterActivityAchievementsLinkagesRequest | List of related linkages

    try:
        api_instance.game_center_activities_achievements_create_to_many_relationship(id, game_center_activity_achievements_linkages_request)
    except Exception as e:
        print("Exception when calling GameCenterActivitiesApi->game_center_activities_achievements_create_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_activity_achievements_linkages_request** | [**GameCenterActivityAchievementsLinkagesRequest**](GameCenterActivityAchievementsLinkagesRequest.md)| List of related linkages | 

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

# **game_center_activities_achievements_delete_to_many_relationship**
> game_center_activities_achievements_delete_to_many_relationship(id, game_center_activity_achievements_linkages_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_activity_achievements_linkages_request import GameCenterActivityAchievementsLinkagesRequest
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
    api_instance = openapi_client.GameCenterActivitiesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_activity_achievements_linkages_request = openapi_client.GameCenterActivityAchievementsLinkagesRequest() # GameCenterActivityAchievementsLinkagesRequest | List of related linkages

    try:
        api_instance.game_center_activities_achievements_delete_to_many_relationship(id, game_center_activity_achievements_linkages_request)
    except Exception as e:
        print("Exception when calling GameCenterActivitiesApi->game_center_activities_achievements_delete_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_activity_achievements_linkages_request** | [**GameCenterActivityAchievementsLinkagesRequest**](GameCenterActivityAchievementsLinkagesRequest.md)| List of related linkages | 

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

# **game_center_activities_create_instance**
> GameCenterActivityResponse game_center_activities_create_instance(game_center_activity_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_activity_create_request import GameCenterActivityCreateRequest
from openapi_client.models.game_center_activity_response import GameCenterActivityResponse
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
    api_instance = openapi_client.GameCenterActivitiesApi(api_client)
    game_center_activity_create_request = openapi_client.GameCenterActivityCreateRequest() # GameCenterActivityCreateRequest | GameCenterActivity representation

    try:
        api_response = api_instance.game_center_activities_create_instance(game_center_activity_create_request)
        print("The response of GameCenterActivitiesApi->game_center_activities_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterActivitiesApi->game_center_activities_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **game_center_activity_create_request** | [**GameCenterActivityCreateRequest**](GameCenterActivityCreateRequest.md)| GameCenterActivity representation | 

### Return type

[**GameCenterActivityResponse**](GameCenterActivityResponse.md)

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
**201** | Single GameCenterActivity |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_activities_delete_instance**
> game_center_activities_delete_instance(id)

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
    api_instance = openapi_client.GameCenterActivitiesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.game_center_activities_delete_instance(id)
    except Exception as e:
        print("Exception when calling GameCenterActivitiesApi->game_center_activities_delete_instance: %s\n" % e)
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

# **game_center_activities_get_instance**
> GameCenterActivityResponse game_center_activities_get_instance(id, fields_game_center_activities=fields_game_center_activities, fields_game_center_activity_versions=fields_game_center_activity_versions, include=include, limit_achievements=limit_achievements, limit_leaderboards=limit_leaderboards, limit_versions=limit_versions)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_activity_response import GameCenterActivityResponse
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
    api_instance = openapi_client.GameCenterActivitiesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_activities = ['fields_game_center_activities_example'] # List[str] | the fields to include for returned resources of type gameCenterActivities (optional)
    fields_game_center_activity_versions = ['fields_game_center_activity_versions_example'] # List[str] | the fields to include for returned resources of type gameCenterActivityVersions (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_achievements = 56 # int | maximum number of related achievements returned (when they are included) (optional)
    limit_leaderboards = 56 # int | maximum number of related leaderboards returned (when they are included) (optional)
    limit_versions = 56 # int | maximum number of related versions returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_activities_get_instance(id, fields_game_center_activities=fields_game_center_activities, fields_game_center_activity_versions=fields_game_center_activity_versions, include=include, limit_achievements=limit_achievements, limit_leaderboards=limit_leaderboards, limit_versions=limit_versions)
        print("The response of GameCenterActivitiesApi->game_center_activities_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterActivitiesApi->game_center_activities_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_activities** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivities | [optional] 
 **fields_game_center_activity_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivityVersions | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_achievements** | **int**| maximum number of related achievements returned (when they are included) | [optional] 
 **limit_leaderboards** | **int**| maximum number of related leaderboards returned (when they are included) | [optional] 
 **limit_versions** | **int**| maximum number of related versions returned (when they are included) | [optional] 

### Return type

[**GameCenterActivityResponse**](GameCenterActivityResponse.md)

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
**200** | Single GameCenterActivity |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_activities_leaderboards_create_to_many_relationship**
> game_center_activities_leaderboards_create_to_many_relationship(id, game_center_activity_leaderboards_linkages_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_activity_leaderboards_linkages_request import GameCenterActivityLeaderboardsLinkagesRequest
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
    api_instance = openapi_client.GameCenterActivitiesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_activity_leaderboards_linkages_request = openapi_client.GameCenterActivityLeaderboardsLinkagesRequest() # GameCenterActivityLeaderboardsLinkagesRequest | List of related linkages

    try:
        api_instance.game_center_activities_leaderboards_create_to_many_relationship(id, game_center_activity_leaderboards_linkages_request)
    except Exception as e:
        print("Exception when calling GameCenterActivitiesApi->game_center_activities_leaderboards_create_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_activity_leaderboards_linkages_request** | [**GameCenterActivityLeaderboardsLinkagesRequest**](GameCenterActivityLeaderboardsLinkagesRequest.md)| List of related linkages | 

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

# **game_center_activities_leaderboards_delete_to_many_relationship**
> game_center_activities_leaderboards_delete_to_many_relationship(id, game_center_activity_leaderboards_linkages_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_activity_leaderboards_linkages_request import GameCenterActivityLeaderboardsLinkagesRequest
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
    api_instance = openapi_client.GameCenterActivitiesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_activity_leaderboards_linkages_request = openapi_client.GameCenterActivityLeaderboardsLinkagesRequest() # GameCenterActivityLeaderboardsLinkagesRequest | List of related linkages

    try:
        api_instance.game_center_activities_leaderboards_delete_to_many_relationship(id, game_center_activity_leaderboards_linkages_request)
    except Exception as e:
        print("Exception when calling GameCenterActivitiesApi->game_center_activities_leaderboards_delete_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_activity_leaderboards_linkages_request** | [**GameCenterActivityLeaderboardsLinkagesRequest**](GameCenterActivityLeaderboardsLinkagesRequest.md)| List of related linkages | 

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

# **game_center_activities_update_instance**
> GameCenterActivityResponse game_center_activities_update_instance(id, game_center_activity_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_activity_response import GameCenterActivityResponse
from openapi_client.models.game_center_activity_update_request import GameCenterActivityUpdateRequest
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
    api_instance = openapi_client.GameCenterActivitiesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_activity_update_request = openapi_client.GameCenterActivityUpdateRequest() # GameCenterActivityUpdateRequest | GameCenterActivity representation

    try:
        api_response = api_instance.game_center_activities_update_instance(id, game_center_activity_update_request)
        print("The response of GameCenterActivitiesApi->game_center_activities_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterActivitiesApi->game_center_activities_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_activity_update_request** | [**GameCenterActivityUpdateRequest**](GameCenterActivityUpdateRequest.md)| GameCenterActivity representation | 

### Return type

[**GameCenterActivityResponse**](GameCenterActivityResponse.md)

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
**200** | Single GameCenterActivity |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_activities_versions_get_to_many_related**
> GameCenterActivityVersionsResponse game_center_activities_versions_get_to_many_related(id, fields_game_center_activity_versions=fields_game_center_activity_versions, fields_game_center_activities=fields_game_center_activities, fields_game_center_activity_localizations=fields_game_center_activity_localizations, fields_game_center_activity_images=fields_game_center_activity_images, fields_game_center_activity_version_releases=fields_game_center_activity_version_releases, limit=limit, include=include, limit_localizations=limit_localizations, limit_releases=limit_releases)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_activity_versions_response import GameCenterActivityVersionsResponse
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
    api_instance = openapi_client.GameCenterActivitiesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_activity_versions = ['fields_game_center_activity_versions_example'] # List[str] | the fields to include for returned resources of type gameCenterActivityVersions (optional)
    fields_game_center_activities = ['fields_game_center_activities_example'] # List[str] | the fields to include for returned resources of type gameCenterActivities (optional)
    fields_game_center_activity_localizations = ['fields_game_center_activity_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterActivityLocalizations (optional)
    fields_game_center_activity_images = ['fields_game_center_activity_images_example'] # List[str] | the fields to include for returned resources of type gameCenterActivityImages (optional)
    fields_game_center_activity_version_releases = ['fields_game_center_activity_version_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterActivityVersionReleases (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_localizations = 56 # int | maximum number of related localizations returned (when they are included) (optional)
    limit_releases = 56 # int | maximum number of related releases returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_activities_versions_get_to_many_related(id, fields_game_center_activity_versions=fields_game_center_activity_versions, fields_game_center_activities=fields_game_center_activities, fields_game_center_activity_localizations=fields_game_center_activity_localizations, fields_game_center_activity_images=fields_game_center_activity_images, fields_game_center_activity_version_releases=fields_game_center_activity_version_releases, limit=limit, include=include, limit_localizations=limit_localizations, limit_releases=limit_releases)
        print("The response of GameCenterActivitiesApi->game_center_activities_versions_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterActivitiesApi->game_center_activities_versions_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_activity_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivityVersions | [optional] 
 **fields_game_center_activities** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivities | [optional] 
 **fields_game_center_activity_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivityLocalizations | [optional] 
 **fields_game_center_activity_images** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivityImages | [optional] 
 **fields_game_center_activity_version_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivityVersionReleases | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_localizations** | **int**| maximum number of related localizations returned (when they are included) | [optional] 
 **limit_releases** | **int**| maximum number of related releases returned (when they are included) | [optional] 

### Return type

[**GameCenterActivityVersionsResponse**](GameCenterActivityVersionsResponse.md)

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
**200** | List of GameCenterActivityVersions |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_activities_versions_get_to_many_relationship**
> GameCenterActivityVersionsLinkagesResponse game_center_activities_versions_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_activity_versions_linkages_response import GameCenterActivityVersionsLinkagesResponse
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
    api_instance = openapi_client.GameCenterActivitiesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_activities_versions_get_to_many_relationship(id, limit=limit)
        print("The response of GameCenterActivitiesApi->game_center_activities_versions_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterActivitiesApi->game_center_activities_versions_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterActivityVersionsLinkagesResponse**](GameCenterActivityVersionsLinkagesResponse.md)

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

