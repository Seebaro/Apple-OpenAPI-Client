# openapi_client.GameCenterLeaderboardsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**game_center_leaderboards_activity_update_to_one_relationship**](GameCenterLeaderboardsApi.md#game_center_leaderboards_activity_update_to_one_relationship) | **PATCH** /v1/gameCenterLeaderboards/{id}/relationships/activity | 
[**game_center_leaderboards_challenge_update_to_one_relationship**](GameCenterLeaderboardsApi.md#game_center_leaderboards_challenge_update_to_one_relationship) | **PATCH** /v1/gameCenterLeaderboards/{id}/relationships/challenge | 
[**game_center_leaderboards_create_instance**](GameCenterLeaderboardsApi.md#game_center_leaderboards_create_instance) | **POST** /v1/gameCenterLeaderboards | 
[**game_center_leaderboards_delete_instance**](GameCenterLeaderboardsApi.md#game_center_leaderboards_delete_instance) | **DELETE** /v1/gameCenterLeaderboards/{id} | 
[**game_center_leaderboards_get_instance**](GameCenterLeaderboardsApi.md#game_center_leaderboards_get_instance) | **GET** /v1/gameCenterLeaderboards/{id} | 
[**game_center_leaderboards_group_leaderboard_get_to_one_related**](GameCenterLeaderboardsApi.md#game_center_leaderboards_group_leaderboard_get_to_one_related) | **GET** /v1/gameCenterLeaderboards/{id}/groupLeaderboard | 
[**game_center_leaderboards_group_leaderboard_get_to_one_relationship**](GameCenterLeaderboardsApi.md#game_center_leaderboards_group_leaderboard_get_to_one_relationship) | **GET** /v1/gameCenterLeaderboards/{id}/relationships/groupLeaderboard | 
[**game_center_leaderboards_group_leaderboard_update_to_one_relationship**](GameCenterLeaderboardsApi.md#game_center_leaderboards_group_leaderboard_update_to_one_relationship) | **PATCH** /v1/gameCenterLeaderboards/{id}/relationships/groupLeaderboard | 
[**game_center_leaderboards_localizations_get_to_many_related**](GameCenterLeaderboardsApi.md#game_center_leaderboards_localizations_get_to_many_related) | **GET** /v1/gameCenterLeaderboards/{id}/localizations | 
[**game_center_leaderboards_localizations_get_to_many_relationship**](GameCenterLeaderboardsApi.md#game_center_leaderboards_localizations_get_to_many_relationship) | **GET** /v1/gameCenterLeaderboards/{id}/relationships/localizations | 
[**game_center_leaderboards_releases_get_to_many_related**](GameCenterLeaderboardsApi.md#game_center_leaderboards_releases_get_to_many_related) | **GET** /v1/gameCenterLeaderboards/{id}/releases | 
[**game_center_leaderboards_releases_get_to_many_relationship**](GameCenterLeaderboardsApi.md#game_center_leaderboards_releases_get_to_many_relationship) | **GET** /v1/gameCenterLeaderboards/{id}/relationships/releases | 
[**game_center_leaderboards_update_instance**](GameCenterLeaderboardsApi.md#game_center_leaderboards_update_instance) | **PATCH** /v1/gameCenterLeaderboards/{id} | 


# **game_center_leaderboards_activity_update_to_one_relationship**
> game_center_leaderboards_activity_update_to_one_relationship(id, game_center_leaderboard_activity_linkage_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_activity_linkage_request import GameCenterLeaderboardActivityLinkageRequest
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
    api_instance = openapi_client.GameCenterLeaderboardsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_leaderboard_activity_linkage_request = openapi_client.GameCenterLeaderboardActivityLinkageRequest() # GameCenterLeaderboardActivityLinkageRequest | Related linkage

    try:
        api_instance.game_center_leaderboards_activity_update_to_one_relationship(id, game_center_leaderboard_activity_linkage_request)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardsApi->game_center_leaderboards_activity_update_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_leaderboard_activity_linkage_request** | [**GameCenterLeaderboardActivityLinkageRequest**](GameCenterLeaderboardActivityLinkageRequest.md)| Related linkage | 

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

# **game_center_leaderboards_challenge_update_to_one_relationship**
> game_center_leaderboards_challenge_update_to_one_relationship(id, game_center_leaderboard_challenge_linkage_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_challenge_linkage_request import GameCenterLeaderboardChallengeLinkageRequest
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
    api_instance = openapi_client.GameCenterLeaderboardsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_leaderboard_challenge_linkage_request = openapi_client.GameCenterLeaderboardChallengeLinkageRequest() # GameCenterLeaderboardChallengeLinkageRequest | Related linkage

    try:
        api_instance.game_center_leaderboards_challenge_update_to_one_relationship(id, game_center_leaderboard_challenge_linkage_request)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardsApi->game_center_leaderboards_challenge_update_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_leaderboard_challenge_linkage_request** | [**GameCenterLeaderboardChallengeLinkageRequest**](GameCenterLeaderboardChallengeLinkageRequest.md)| Related linkage | 

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

# **game_center_leaderboards_create_instance**
> GameCenterLeaderboardResponse game_center_leaderboards_create_instance(game_center_leaderboard_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_create_request import GameCenterLeaderboardCreateRequest
from openapi_client.models.game_center_leaderboard_response import GameCenterLeaderboardResponse
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
    api_instance = openapi_client.GameCenterLeaderboardsApi(api_client)
    game_center_leaderboard_create_request = openapi_client.GameCenterLeaderboardCreateRequest() # GameCenterLeaderboardCreateRequest | GameCenterLeaderboard representation

    try:
        api_response = api_instance.game_center_leaderboards_create_instance(game_center_leaderboard_create_request)
        print("The response of GameCenterLeaderboardsApi->game_center_leaderboards_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardsApi->game_center_leaderboards_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **game_center_leaderboard_create_request** | [**GameCenterLeaderboardCreateRequest**](GameCenterLeaderboardCreateRequest.md)| GameCenterLeaderboard representation | 

### Return type

[**GameCenterLeaderboardResponse**](GameCenterLeaderboardResponse.md)

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
**201** | Single GameCenterLeaderboard |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_leaderboards_delete_instance**
> game_center_leaderboards_delete_instance(id)

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
    api_instance = openapi_client.GameCenterLeaderboardsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.game_center_leaderboards_delete_instance(id)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardsApi->game_center_leaderboards_delete_instance: %s\n" % e)
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

# **game_center_leaderboards_get_instance**
> GameCenterLeaderboardResponse game_center_leaderboards_get_instance(id, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_leaderboard_localizations=fields_game_center_leaderboard_localizations, fields_game_center_leaderboard_releases=fields_game_center_leaderboard_releases, include=include, limit_game_center_leaderboard_sets=limit_game_center_leaderboard_sets, limit_localizations=limit_localizations, limit_releases=limit_releases)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_response import GameCenterLeaderboardResponse
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
    api_instance = openapi_client.GameCenterLeaderboardsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_leaderboards = ['fields_game_center_leaderboards_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboards (optional)
    fields_game_center_leaderboard_localizations = ['fields_game_center_leaderboard_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardLocalizations (optional)
    fields_game_center_leaderboard_releases = ['fields_game_center_leaderboard_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardReleases (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_game_center_leaderboard_sets = 56 # int | maximum number of related gameCenterLeaderboardSets returned (when they are included) (optional)
    limit_localizations = 56 # int | maximum number of related localizations returned (when they are included) (optional)
    limit_releases = 56 # int | maximum number of related releases returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_leaderboards_get_instance(id, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_leaderboard_localizations=fields_game_center_leaderboard_localizations, fields_game_center_leaderboard_releases=fields_game_center_leaderboard_releases, include=include, limit_game_center_leaderboard_sets=limit_game_center_leaderboard_sets, limit_localizations=limit_localizations, limit_releases=limit_releases)
        print("The response of GameCenterLeaderboardsApi->game_center_leaderboards_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardsApi->game_center_leaderboards_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_leaderboards** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboards | [optional] 
 **fields_game_center_leaderboard_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional] 
 **fields_game_center_leaderboard_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardReleases | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_game_center_leaderboard_sets** | **int**| maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional] 
 **limit_localizations** | **int**| maximum number of related localizations returned (when they are included) | [optional] 
 **limit_releases** | **int**| maximum number of related releases returned (when they are included) | [optional] 

### Return type

[**GameCenterLeaderboardResponse**](GameCenterLeaderboardResponse.md)

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
**200** | Single GameCenterLeaderboard |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_leaderboards_group_leaderboard_get_to_one_related**
> GameCenterLeaderboardResponse game_center_leaderboards_group_leaderboard_get_to_one_related(id, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_leaderboard_localizations=fields_game_center_leaderboard_localizations, fields_game_center_leaderboard_releases=fields_game_center_leaderboard_releases, fields_game_center_activities=fields_game_center_activities, fields_game_center_challenges=fields_game_center_challenges, include=include, limit_game_center_leaderboard_sets=limit_game_center_leaderboard_sets, limit_localizations=limit_localizations, limit_releases=limit_releases)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_response import GameCenterLeaderboardResponse
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
    api_instance = openapi_client.GameCenterLeaderboardsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_leaderboards = ['fields_game_center_leaderboards_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboards (optional)
    fields_game_center_details = ['fields_game_center_details_example'] # List[str] | the fields to include for returned resources of type gameCenterDetails (optional)
    fields_game_center_groups = ['fields_game_center_groups_example'] # List[str] | the fields to include for returned resources of type gameCenterGroups (optional)
    fields_game_center_leaderboard_sets = ['fields_game_center_leaderboard_sets_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSets (optional)
    fields_game_center_leaderboard_localizations = ['fields_game_center_leaderboard_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardLocalizations (optional)
    fields_game_center_leaderboard_releases = ['fields_game_center_leaderboard_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardReleases (optional)
    fields_game_center_activities = ['fields_game_center_activities_example'] # List[str] | the fields to include for returned resources of type gameCenterActivities (optional)
    fields_game_center_challenges = ['fields_game_center_challenges_example'] # List[str] | the fields to include for returned resources of type gameCenterChallenges (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_game_center_leaderboard_sets = 56 # int | maximum number of related gameCenterLeaderboardSets returned (when they are included) (optional)
    limit_localizations = 56 # int | maximum number of related localizations returned (when they are included) (optional)
    limit_releases = 56 # int | maximum number of related releases returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_leaderboards_group_leaderboard_get_to_one_related(id, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_leaderboard_localizations=fields_game_center_leaderboard_localizations, fields_game_center_leaderboard_releases=fields_game_center_leaderboard_releases, fields_game_center_activities=fields_game_center_activities, fields_game_center_challenges=fields_game_center_challenges, include=include, limit_game_center_leaderboard_sets=limit_game_center_leaderboard_sets, limit_localizations=limit_localizations, limit_releases=limit_releases)
        print("The response of GameCenterLeaderboardsApi->game_center_leaderboards_group_leaderboard_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardsApi->game_center_leaderboards_group_leaderboard_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_leaderboards** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboards | [optional] 
 **fields_game_center_details** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterDetails | [optional] 
 **fields_game_center_groups** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterGroups | [optional] 
 **fields_game_center_leaderboard_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSets | [optional] 
 **fields_game_center_leaderboard_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional] 
 **fields_game_center_leaderboard_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardReleases | [optional] 
 **fields_game_center_activities** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivities | [optional] 
 **fields_game_center_challenges** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallenges | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_game_center_leaderboard_sets** | **int**| maximum number of related gameCenterLeaderboardSets returned (when they are included) | [optional] 
 **limit_localizations** | **int**| maximum number of related localizations returned (when they are included) | [optional] 
 **limit_releases** | **int**| maximum number of related releases returned (when they are included) | [optional] 

### Return type

[**GameCenterLeaderboardResponse**](GameCenterLeaderboardResponse.md)

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
**200** | Single GameCenterLeaderboard |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_leaderboards_group_leaderboard_get_to_one_relationship**
> GameCenterLeaderboardGroupLeaderboardLinkageResponse game_center_leaderboards_group_leaderboard_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_group_leaderboard_linkage_response import GameCenterLeaderboardGroupLeaderboardLinkageResponse
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
    api_instance = openapi_client.GameCenterLeaderboardsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.game_center_leaderboards_group_leaderboard_get_to_one_relationship(id)
        print("The response of GameCenterLeaderboardsApi->game_center_leaderboards_group_leaderboard_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardsApi->game_center_leaderboards_group_leaderboard_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**GameCenterLeaderboardGroupLeaderboardLinkageResponse**](GameCenterLeaderboardGroupLeaderboardLinkageResponse.md)

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

# **game_center_leaderboards_group_leaderboard_update_to_one_relationship**
> game_center_leaderboards_group_leaderboard_update_to_one_relationship(id, game_center_leaderboard_group_leaderboard_linkage_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_group_leaderboard_linkage_request import GameCenterLeaderboardGroupLeaderboardLinkageRequest
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
    api_instance = openapi_client.GameCenterLeaderboardsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_leaderboard_group_leaderboard_linkage_request = openapi_client.GameCenterLeaderboardGroupLeaderboardLinkageRequest() # GameCenterLeaderboardGroupLeaderboardLinkageRequest | Related linkage

    try:
        api_instance.game_center_leaderboards_group_leaderboard_update_to_one_relationship(id, game_center_leaderboard_group_leaderboard_linkage_request)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardsApi->game_center_leaderboards_group_leaderboard_update_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_leaderboard_group_leaderboard_linkage_request** | [**GameCenterLeaderboardGroupLeaderboardLinkageRequest**](GameCenterLeaderboardGroupLeaderboardLinkageRequest.md)| Related linkage | 

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

# **game_center_leaderboards_localizations_get_to_many_related**
> GameCenterLeaderboardLocalizationsResponse game_center_leaderboards_localizations_get_to_many_related(id, fields_game_center_leaderboard_localizations=fields_game_center_leaderboard_localizations, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_leaderboard_images=fields_game_center_leaderboard_images, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_localizations_response import GameCenterLeaderboardLocalizationsResponse
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
    api_instance = openapi_client.GameCenterLeaderboardsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_leaderboard_localizations = ['fields_game_center_leaderboard_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardLocalizations (optional)
    fields_game_center_leaderboards = ['fields_game_center_leaderboards_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboards (optional)
    fields_game_center_leaderboard_images = ['fields_game_center_leaderboard_images_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardImages (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.game_center_leaderboards_localizations_get_to_many_related(id, fields_game_center_leaderboard_localizations=fields_game_center_leaderboard_localizations, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_leaderboard_images=fields_game_center_leaderboard_images, limit=limit, include=include)
        print("The response of GameCenterLeaderboardsApi->game_center_leaderboards_localizations_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardsApi->game_center_leaderboards_localizations_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_leaderboard_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional] 
 **fields_game_center_leaderboards** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboards | [optional] 
 **fields_game_center_leaderboard_images** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardImages | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**GameCenterLeaderboardLocalizationsResponse**](GameCenterLeaderboardLocalizationsResponse.md)

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
**200** | List of GameCenterLeaderboardLocalizations |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_leaderboards_localizations_get_to_many_relationship**
> GameCenterLeaderboardLocalizationsLinkagesResponse game_center_leaderboards_localizations_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_localizations_linkages_response import GameCenterLeaderboardLocalizationsLinkagesResponse
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
    api_instance = openapi_client.GameCenterLeaderboardsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_leaderboards_localizations_get_to_many_relationship(id, limit=limit)
        print("The response of GameCenterLeaderboardsApi->game_center_leaderboards_localizations_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardsApi->game_center_leaderboards_localizations_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterLeaderboardLocalizationsLinkagesResponse**](GameCenterLeaderboardLocalizationsLinkagesResponse.md)

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

# **game_center_leaderboards_releases_get_to_many_related**
> GameCenterLeaderboardReleasesResponse game_center_leaderboards_releases_get_to_many_related(id, filter_live=filter_live, filter_game_center_detail=filter_game_center_detail, fields_game_center_leaderboard_releases=fields_game_center_leaderboard_releases, fields_game_center_details=fields_game_center_details, fields_game_center_leaderboards=fields_game_center_leaderboards, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_releases_response import GameCenterLeaderboardReleasesResponse
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
    api_instance = openapi_client.GameCenterLeaderboardsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_live = ['filter_live_example'] # List[str] | filter by attribute 'live' (optional)
    filter_game_center_detail = ['filter_game_center_detail_example'] # List[str] | filter by id(s) of related 'gameCenterDetail' (optional)
    fields_game_center_leaderboard_releases = ['fields_game_center_leaderboard_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardReleases (optional)
    fields_game_center_details = ['fields_game_center_details_example'] # List[str] | the fields to include for returned resources of type gameCenterDetails (optional)
    fields_game_center_leaderboards = ['fields_game_center_leaderboards_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboards (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.game_center_leaderboards_releases_get_to_many_related(id, filter_live=filter_live, filter_game_center_detail=filter_game_center_detail, fields_game_center_leaderboard_releases=fields_game_center_leaderboard_releases, fields_game_center_details=fields_game_center_details, fields_game_center_leaderboards=fields_game_center_leaderboards, limit=limit, include=include)
        print("The response of GameCenterLeaderboardsApi->game_center_leaderboards_releases_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardsApi->game_center_leaderboards_releases_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_live** | [**List[str]**](str.md)| filter by attribute &#39;live&#39; | [optional] 
 **filter_game_center_detail** | [**List[str]**](str.md)| filter by id(s) of related &#39;gameCenterDetail&#39; | [optional] 
 **fields_game_center_leaderboard_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardReleases | [optional] 
 **fields_game_center_details** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterDetails | [optional] 
 **fields_game_center_leaderboards** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboards | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**GameCenterLeaderboardReleasesResponse**](GameCenterLeaderboardReleasesResponse.md)

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
**200** | List of GameCenterLeaderboardReleases |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_leaderboards_releases_get_to_many_relationship**
> GameCenterLeaderboardReleasesLinkagesResponse game_center_leaderboards_releases_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_releases_linkages_response import GameCenterLeaderboardReleasesLinkagesResponse
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
    api_instance = openapi_client.GameCenterLeaderboardsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_leaderboards_releases_get_to_many_relationship(id, limit=limit)
        print("The response of GameCenterLeaderboardsApi->game_center_leaderboards_releases_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardsApi->game_center_leaderboards_releases_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterLeaderboardReleasesLinkagesResponse**](GameCenterLeaderboardReleasesLinkagesResponse.md)

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

# **game_center_leaderboards_update_instance**
> GameCenterLeaderboardResponse game_center_leaderboards_update_instance(id, game_center_leaderboard_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_response import GameCenterLeaderboardResponse
from openapi_client.models.game_center_leaderboard_update_request import GameCenterLeaderboardUpdateRequest
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
    api_instance = openapi_client.GameCenterLeaderboardsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_leaderboard_update_request = openapi_client.GameCenterLeaderboardUpdateRequest() # GameCenterLeaderboardUpdateRequest | GameCenterLeaderboard representation

    try:
        api_response = api_instance.game_center_leaderboards_update_instance(id, game_center_leaderboard_update_request)
        print("The response of GameCenterLeaderboardsApi->game_center_leaderboards_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardsApi->game_center_leaderboards_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_leaderboard_update_request** | [**GameCenterLeaderboardUpdateRequest**](GameCenterLeaderboardUpdateRequest.md)| GameCenterLeaderboard representation | 

### Return type

[**GameCenterLeaderboardResponse**](GameCenterLeaderboardResponse.md)

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
**200** | Single GameCenterLeaderboard |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

