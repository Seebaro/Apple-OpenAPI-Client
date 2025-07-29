# openapi_client.GameCenterLeaderboardSetsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**game_center_leaderboard_sets_create_instance**](GameCenterLeaderboardSetsApi.md#game_center_leaderboard_sets_create_instance) | **POST** /v1/gameCenterLeaderboardSets | 
[**game_center_leaderboard_sets_delete_instance**](GameCenterLeaderboardSetsApi.md#game_center_leaderboard_sets_delete_instance) | **DELETE** /v1/gameCenterLeaderboardSets/{id} | 
[**game_center_leaderboard_sets_game_center_leaderboards_create_to_many_relationship**](GameCenterLeaderboardSetsApi.md#game_center_leaderboard_sets_game_center_leaderboards_create_to_many_relationship) | **POST** /v1/gameCenterLeaderboardSets/{id}/relationships/gameCenterLeaderboards | 
[**game_center_leaderboard_sets_game_center_leaderboards_delete_to_many_relationship**](GameCenterLeaderboardSetsApi.md#game_center_leaderboard_sets_game_center_leaderboards_delete_to_many_relationship) | **DELETE** /v1/gameCenterLeaderboardSets/{id}/relationships/gameCenterLeaderboards | 
[**game_center_leaderboard_sets_game_center_leaderboards_get_to_many_related**](GameCenterLeaderboardSetsApi.md#game_center_leaderboard_sets_game_center_leaderboards_get_to_many_related) | **GET** /v1/gameCenterLeaderboardSets/{id}/gameCenterLeaderboards | 
[**game_center_leaderboard_sets_game_center_leaderboards_get_to_many_relationship**](GameCenterLeaderboardSetsApi.md#game_center_leaderboard_sets_game_center_leaderboards_get_to_many_relationship) | **GET** /v1/gameCenterLeaderboardSets/{id}/relationships/gameCenterLeaderboards | 
[**game_center_leaderboard_sets_game_center_leaderboards_replace_to_many_relationship**](GameCenterLeaderboardSetsApi.md#game_center_leaderboard_sets_game_center_leaderboards_replace_to_many_relationship) | **PATCH** /v1/gameCenterLeaderboardSets/{id}/relationships/gameCenterLeaderboards | 
[**game_center_leaderboard_sets_get_instance**](GameCenterLeaderboardSetsApi.md#game_center_leaderboard_sets_get_instance) | **GET** /v1/gameCenterLeaderboardSets/{id} | 
[**game_center_leaderboard_sets_group_leaderboard_set_get_to_one_related**](GameCenterLeaderboardSetsApi.md#game_center_leaderboard_sets_group_leaderboard_set_get_to_one_related) | **GET** /v1/gameCenterLeaderboardSets/{id}/groupLeaderboardSet | 
[**game_center_leaderboard_sets_group_leaderboard_set_get_to_one_relationship**](GameCenterLeaderboardSetsApi.md#game_center_leaderboard_sets_group_leaderboard_set_get_to_one_relationship) | **GET** /v1/gameCenterLeaderboardSets/{id}/relationships/groupLeaderboardSet | 
[**game_center_leaderboard_sets_group_leaderboard_set_update_to_one_relationship**](GameCenterLeaderboardSetsApi.md#game_center_leaderboard_sets_group_leaderboard_set_update_to_one_relationship) | **PATCH** /v1/gameCenterLeaderboardSets/{id}/relationships/groupLeaderboardSet | 
[**game_center_leaderboard_sets_localizations_get_to_many_related**](GameCenterLeaderboardSetsApi.md#game_center_leaderboard_sets_localizations_get_to_many_related) | **GET** /v1/gameCenterLeaderboardSets/{id}/localizations | 
[**game_center_leaderboard_sets_localizations_get_to_many_relationship**](GameCenterLeaderboardSetsApi.md#game_center_leaderboard_sets_localizations_get_to_many_relationship) | **GET** /v1/gameCenterLeaderboardSets/{id}/relationships/localizations | 
[**game_center_leaderboard_sets_releases_get_to_many_related**](GameCenterLeaderboardSetsApi.md#game_center_leaderboard_sets_releases_get_to_many_related) | **GET** /v1/gameCenterLeaderboardSets/{id}/releases | 
[**game_center_leaderboard_sets_releases_get_to_many_relationship**](GameCenterLeaderboardSetsApi.md#game_center_leaderboard_sets_releases_get_to_many_relationship) | **GET** /v1/gameCenterLeaderboardSets/{id}/relationships/releases | 
[**game_center_leaderboard_sets_update_instance**](GameCenterLeaderboardSetsApi.md#game_center_leaderboard_sets_update_instance) | **PATCH** /v1/gameCenterLeaderboardSets/{id} | 


# **game_center_leaderboard_sets_create_instance**
> GameCenterLeaderboardSetResponse game_center_leaderboard_sets_create_instance(game_center_leaderboard_set_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_create_request import GameCenterLeaderboardSetCreateRequest
from openapi_client.models.game_center_leaderboard_set_response import GameCenterLeaderboardSetResponse
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
    api_instance = openapi_client.GameCenterLeaderboardSetsApi(api_client)
    game_center_leaderboard_set_create_request = openapi_client.GameCenterLeaderboardSetCreateRequest() # GameCenterLeaderboardSetCreateRequest | GameCenterLeaderboardSet representation

    try:
        api_response = api_instance.game_center_leaderboard_sets_create_instance(game_center_leaderboard_set_create_request)
        print("The response of GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **game_center_leaderboard_set_create_request** | [**GameCenterLeaderboardSetCreateRequest**](GameCenterLeaderboardSetCreateRequest.md)| GameCenterLeaderboardSet representation | 

### Return type

[**GameCenterLeaderboardSetResponse**](GameCenterLeaderboardSetResponse.md)

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
**201** | Single GameCenterLeaderboardSet |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_leaderboard_sets_delete_instance**
> game_center_leaderboard_sets_delete_instance(id)

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
    api_instance = openapi_client.GameCenterLeaderboardSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.game_center_leaderboard_sets_delete_instance(id)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_delete_instance: %s\n" % e)
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

# **game_center_leaderboard_sets_game_center_leaderboards_create_to_many_relationship**
> game_center_leaderboard_sets_game_center_leaderboards_create_to_many_relationship(id, game_center_leaderboard_set_game_center_leaderboards_linkages_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_game_center_leaderboards_linkages_request import GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest
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
    api_instance = openapi_client.GameCenterLeaderboardSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_leaderboard_set_game_center_leaderboards_linkages_request = openapi_client.GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest() # GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest | List of related linkages

    try:
        api_instance.game_center_leaderboard_sets_game_center_leaderboards_create_to_many_relationship(id, game_center_leaderboard_set_game_center_leaderboards_linkages_request)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_game_center_leaderboards_create_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_leaderboard_set_game_center_leaderboards_linkages_request** | [**GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest**](GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest.md)| List of related linkages | 

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

# **game_center_leaderboard_sets_game_center_leaderboards_delete_to_many_relationship**
> game_center_leaderboard_sets_game_center_leaderboards_delete_to_many_relationship(id, game_center_leaderboard_set_game_center_leaderboards_linkages_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_game_center_leaderboards_linkages_request import GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest
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
    api_instance = openapi_client.GameCenterLeaderboardSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_leaderboard_set_game_center_leaderboards_linkages_request = openapi_client.GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest() # GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest | List of related linkages

    try:
        api_instance.game_center_leaderboard_sets_game_center_leaderboards_delete_to_many_relationship(id, game_center_leaderboard_set_game_center_leaderboards_linkages_request)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_game_center_leaderboards_delete_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_leaderboard_set_game_center_leaderboards_linkages_request** | [**GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest**](GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest.md)| List of related linkages | 

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

# **game_center_leaderboard_sets_game_center_leaderboards_get_to_many_related**
> GameCenterLeaderboardsResponse game_center_leaderboard_sets_game_center_leaderboards_get_to_many_related(id, filter_reference_name=filter_reference_name, filter_archived=filter_archived, filter_id=filter_id, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_leaderboard_localizations=fields_game_center_leaderboard_localizations, fields_game_center_leaderboard_releases=fields_game_center_leaderboard_releases, fields_game_center_activities=fields_game_center_activities, fields_game_center_challenges=fields_game_center_challenges, limit=limit, include=include, limit_game_center_leaderboard_sets=limit_game_center_leaderboard_sets, limit_localizations=limit_localizations, limit_releases=limit_releases)

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
    api_instance = openapi_client.GameCenterLeaderboardSetsApi(api_client)
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
        api_response = api_instance.game_center_leaderboard_sets_game_center_leaderboards_get_to_many_related(id, filter_reference_name=filter_reference_name, filter_archived=filter_archived, filter_id=filter_id, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_leaderboard_localizations=fields_game_center_leaderboard_localizations, fields_game_center_leaderboard_releases=fields_game_center_leaderboard_releases, fields_game_center_activities=fields_game_center_activities, fields_game_center_challenges=fields_game_center_challenges, limit=limit, include=include, limit_game_center_leaderboard_sets=limit_game_center_leaderboard_sets, limit_localizations=limit_localizations, limit_releases=limit_releases)
        print("The response of GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_game_center_leaderboards_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_game_center_leaderboards_get_to_many_related: %s\n" % e)
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

# **game_center_leaderboard_sets_game_center_leaderboards_get_to_many_relationship**
> GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesResponse game_center_leaderboard_sets_game_center_leaderboards_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_game_center_leaderboards_linkages_response import GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesResponse
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
    api_instance = openapi_client.GameCenterLeaderboardSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_leaderboard_sets_game_center_leaderboards_get_to_many_relationship(id, limit=limit)
        print("The response of GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_game_center_leaderboards_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_game_center_leaderboards_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesResponse**](GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesResponse.md)

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

# **game_center_leaderboard_sets_game_center_leaderboards_replace_to_many_relationship**
> game_center_leaderboard_sets_game_center_leaderboards_replace_to_many_relationship(id, game_center_leaderboard_set_game_center_leaderboards_linkages_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_game_center_leaderboards_linkages_request import GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest
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
    api_instance = openapi_client.GameCenterLeaderboardSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_leaderboard_set_game_center_leaderboards_linkages_request = openapi_client.GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest() # GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest | List of related linkages

    try:
        api_instance.game_center_leaderboard_sets_game_center_leaderboards_replace_to_many_relationship(id, game_center_leaderboard_set_game_center_leaderboards_linkages_request)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_game_center_leaderboards_replace_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_leaderboard_set_game_center_leaderboards_linkages_request** | [**GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest**](GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest.md)| List of related linkages | 

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

# **game_center_leaderboard_sets_get_instance**
> GameCenterLeaderboardSetResponse game_center_leaderboard_sets_get_instance(id, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_leaderboard_set_localizations=fields_game_center_leaderboard_set_localizations, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_leaderboard_set_releases=fields_game_center_leaderboard_set_releases, include=include, limit_game_center_leaderboards=limit_game_center_leaderboards, limit_localizations=limit_localizations, limit_releases=limit_releases)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_response import GameCenterLeaderboardSetResponse
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
    api_instance = openapi_client.GameCenterLeaderboardSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_leaderboard_sets = ['fields_game_center_leaderboard_sets_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSets (optional)
    fields_game_center_leaderboard_set_localizations = ['fields_game_center_leaderboard_set_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations (optional)
    fields_game_center_leaderboards = ['fields_game_center_leaderboards_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboards (optional)
    fields_game_center_leaderboard_set_releases = ['fields_game_center_leaderboard_set_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSetReleases (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_game_center_leaderboards = 56 # int | maximum number of related gameCenterLeaderboards returned (when they are included) (optional)
    limit_localizations = 56 # int | maximum number of related localizations returned (when they are included) (optional)
    limit_releases = 56 # int | maximum number of related releases returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_leaderboard_sets_get_instance(id, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_leaderboard_set_localizations=fields_game_center_leaderboard_set_localizations, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_leaderboard_set_releases=fields_game_center_leaderboard_set_releases, include=include, limit_game_center_leaderboards=limit_game_center_leaderboards, limit_localizations=limit_localizations, limit_releases=limit_releases)
        print("The response of GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_leaderboard_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSets | [optional] 
 **fields_game_center_leaderboard_set_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional] 
 **fields_game_center_leaderboards** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboards | [optional] 
 **fields_game_center_leaderboard_set_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSetReleases | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_game_center_leaderboards** | **int**| maximum number of related gameCenterLeaderboards returned (when they are included) | [optional] 
 **limit_localizations** | **int**| maximum number of related localizations returned (when they are included) | [optional] 
 **limit_releases** | **int**| maximum number of related releases returned (when they are included) | [optional] 

### Return type

[**GameCenterLeaderboardSetResponse**](GameCenterLeaderboardSetResponse.md)

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
**200** | Single GameCenterLeaderboardSet |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_leaderboard_sets_group_leaderboard_set_get_to_one_related**
> GameCenterLeaderboardSetResponse game_center_leaderboard_sets_group_leaderboard_set_get_to_one_related(id, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_leaderboard_set_localizations=fields_game_center_leaderboard_set_localizations, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_leaderboard_set_releases=fields_game_center_leaderboard_set_releases, include=include, limit_localizations=limit_localizations, limit_game_center_leaderboards=limit_game_center_leaderboards, limit_releases=limit_releases)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_response import GameCenterLeaderboardSetResponse
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
    api_instance = openapi_client.GameCenterLeaderboardSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_leaderboard_sets = ['fields_game_center_leaderboard_sets_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSets (optional)
    fields_game_center_details = ['fields_game_center_details_example'] # List[str] | the fields to include for returned resources of type gameCenterDetails (optional)
    fields_game_center_groups = ['fields_game_center_groups_example'] # List[str] | the fields to include for returned resources of type gameCenterGroups (optional)
    fields_game_center_leaderboard_set_localizations = ['fields_game_center_leaderboard_set_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations (optional)
    fields_game_center_leaderboards = ['fields_game_center_leaderboards_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboards (optional)
    fields_game_center_leaderboard_set_releases = ['fields_game_center_leaderboard_set_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSetReleases (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_localizations = 56 # int | maximum number of related localizations returned (when they are included) (optional)
    limit_game_center_leaderboards = 56 # int | maximum number of related gameCenterLeaderboards returned (when they are included) (optional)
    limit_releases = 56 # int | maximum number of related releases returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_leaderboard_sets_group_leaderboard_set_get_to_one_related(id, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_leaderboard_set_localizations=fields_game_center_leaderboard_set_localizations, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_leaderboard_set_releases=fields_game_center_leaderboard_set_releases, include=include, limit_localizations=limit_localizations, limit_game_center_leaderboards=limit_game_center_leaderboards, limit_releases=limit_releases)
        print("The response of GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_group_leaderboard_set_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_group_leaderboard_set_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_leaderboard_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSets | [optional] 
 **fields_game_center_details** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterDetails | [optional] 
 **fields_game_center_groups** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterGroups | [optional] 
 **fields_game_center_leaderboard_set_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional] 
 **fields_game_center_leaderboards** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboards | [optional] 
 **fields_game_center_leaderboard_set_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSetReleases | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_localizations** | **int**| maximum number of related localizations returned (when they are included) | [optional] 
 **limit_game_center_leaderboards** | **int**| maximum number of related gameCenterLeaderboards returned (when they are included) | [optional] 
 **limit_releases** | **int**| maximum number of related releases returned (when they are included) | [optional] 

### Return type

[**GameCenterLeaderboardSetResponse**](GameCenterLeaderboardSetResponse.md)

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
**200** | Single GameCenterLeaderboardSet |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_leaderboard_sets_group_leaderboard_set_get_to_one_relationship**
> GameCenterLeaderboardSetGroupLeaderboardSetLinkageResponse game_center_leaderboard_sets_group_leaderboard_set_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_group_leaderboard_set_linkage_response import GameCenterLeaderboardSetGroupLeaderboardSetLinkageResponse
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
    api_instance = openapi_client.GameCenterLeaderboardSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.game_center_leaderboard_sets_group_leaderboard_set_get_to_one_relationship(id)
        print("The response of GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_group_leaderboard_set_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_group_leaderboard_set_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**GameCenterLeaderboardSetGroupLeaderboardSetLinkageResponse**](GameCenterLeaderboardSetGroupLeaderboardSetLinkageResponse.md)

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

# **game_center_leaderboard_sets_group_leaderboard_set_update_to_one_relationship**
> game_center_leaderboard_sets_group_leaderboard_set_update_to_one_relationship(id, game_center_leaderboard_set_group_leaderboard_set_linkage_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_group_leaderboard_set_linkage_request import GameCenterLeaderboardSetGroupLeaderboardSetLinkageRequest
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
    api_instance = openapi_client.GameCenterLeaderboardSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_leaderboard_set_group_leaderboard_set_linkage_request = openapi_client.GameCenterLeaderboardSetGroupLeaderboardSetLinkageRequest() # GameCenterLeaderboardSetGroupLeaderboardSetLinkageRequest | Related linkage

    try:
        api_instance.game_center_leaderboard_sets_group_leaderboard_set_update_to_one_relationship(id, game_center_leaderboard_set_group_leaderboard_set_linkage_request)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_group_leaderboard_set_update_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_leaderboard_set_group_leaderboard_set_linkage_request** | [**GameCenterLeaderboardSetGroupLeaderboardSetLinkageRequest**](GameCenterLeaderboardSetGroupLeaderboardSetLinkageRequest.md)| Related linkage | 

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

# **game_center_leaderboard_sets_localizations_get_to_many_related**
> GameCenterLeaderboardSetLocalizationsResponse game_center_leaderboard_sets_localizations_get_to_many_related(id, fields_game_center_leaderboard_set_localizations=fields_game_center_leaderboard_set_localizations, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_leaderboard_set_images=fields_game_center_leaderboard_set_images, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_localizations_response import GameCenterLeaderboardSetLocalizationsResponse
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
    api_instance = openapi_client.GameCenterLeaderboardSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_leaderboard_set_localizations = ['fields_game_center_leaderboard_set_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations (optional)
    fields_game_center_leaderboard_sets = ['fields_game_center_leaderboard_sets_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSets (optional)
    fields_game_center_leaderboard_set_images = ['fields_game_center_leaderboard_set_images_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSetImages (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.game_center_leaderboard_sets_localizations_get_to_many_related(id, fields_game_center_leaderboard_set_localizations=fields_game_center_leaderboard_set_localizations, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_leaderboard_set_images=fields_game_center_leaderboard_set_images, limit=limit, include=include)
        print("The response of GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_localizations_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_localizations_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_leaderboard_set_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSetLocalizations | [optional] 
 **fields_game_center_leaderboard_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSets | [optional] 
 **fields_game_center_leaderboard_set_images** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSetImages | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**GameCenterLeaderboardSetLocalizationsResponse**](GameCenterLeaderboardSetLocalizationsResponse.md)

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
**200** | List of GameCenterLeaderboardSetLocalizations |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_leaderboard_sets_localizations_get_to_many_relationship**
> GameCenterLeaderboardSetLocalizationsLinkagesResponse game_center_leaderboard_sets_localizations_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_localizations_linkages_response import GameCenterLeaderboardSetLocalizationsLinkagesResponse
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
    api_instance = openapi_client.GameCenterLeaderboardSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_leaderboard_sets_localizations_get_to_many_relationship(id, limit=limit)
        print("The response of GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_localizations_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_localizations_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterLeaderboardSetLocalizationsLinkagesResponse**](GameCenterLeaderboardSetLocalizationsLinkagesResponse.md)

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

# **game_center_leaderboard_sets_releases_get_to_many_related**
> GameCenterLeaderboardSetReleasesResponse game_center_leaderboard_sets_releases_get_to_many_related(id, filter_live=filter_live, filter_game_center_detail=filter_game_center_detail, fields_game_center_leaderboard_set_releases=fields_game_center_leaderboard_set_releases, fields_game_center_details=fields_game_center_details, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_releases_response import GameCenterLeaderboardSetReleasesResponse
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
    api_instance = openapi_client.GameCenterLeaderboardSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_live = ['filter_live_example'] # List[str] | filter by attribute 'live' (optional)
    filter_game_center_detail = ['filter_game_center_detail_example'] # List[str] | filter by id(s) of related 'gameCenterDetail' (optional)
    fields_game_center_leaderboard_set_releases = ['fields_game_center_leaderboard_set_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSetReleases (optional)
    fields_game_center_details = ['fields_game_center_details_example'] # List[str] | the fields to include for returned resources of type gameCenterDetails (optional)
    fields_game_center_leaderboard_sets = ['fields_game_center_leaderboard_sets_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSets (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.game_center_leaderboard_sets_releases_get_to_many_related(id, filter_live=filter_live, filter_game_center_detail=filter_game_center_detail, fields_game_center_leaderboard_set_releases=fields_game_center_leaderboard_set_releases, fields_game_center_details=fields_game_center_details, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, limit=limit, include=include)
        print("The response of GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_releases_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_releases_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_live** | [**List[str]**](str.md)| filter by attribute &#39;live&#39; | [optional] 
 **filter_game_center_detail** | [**List[str]**](str.md)| filter by id(s) of related &#39;gameCenterDetail&#39; | [optional] 
 **fields_game_center_leaderboard_set_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSetReleases | [optional] 
 **fields_game_center_details** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterDetails | [optional] 
 **fields_game_center_leaderboard_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSets | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**GameCenterLeaderboardSetReleasesResponse**](GameCenterLeaderboardSetReleasesResponse.md)

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
**200** | List of GameCenterLeaderboardSetReleases |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_leaderboard_sets_releases_get_to_many_relationship**
> GameCenterLeaderboardSetReleasesLinkagesResponse game_center_leaderboard_sets_releases_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_releases_linkages_response import GameCenterLeaderboardSetReleasesLinkagesResponse
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
    api_instance = openapi_client.GameCenterLeaderboardSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_leaderboard_sets_releases_get_to_many_relationship(id, limit=limit)
        print("The response of GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_releases_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_releases_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterLeaderboardSetReleasesLinkagesResponse**](GameCenterLeaderboardSetReleasesLinkagesResponse.md)

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

# **game_center_leaderboard_sets_update_instance**
> GameCenterLeaderboardSetResponse game_center_leaderboard_sets_update_instance(id, game_center_leaderboard_set_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_response import GameCenterLeaderboardSetResponse
from openapi_client.models.game_center_leaderboard_set_update_request import GameCenterLeaderboardSetUpdateRequest
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
    api_instance = openapi_client.GameCenterLeaderboardSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_leaderboard_set_update_request = openapi_client.GameCenterLeaderboardSetUpdateRequest() # GameCenterLeaderboardSetUpdateRequest | GameCenterLeaderboardSet representation

    try:
        api_response = api_instance.game_center_leaderboard_sets_update_instance(id, game_center_leaderboard_set_update_request)
        print("The response of GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetsApi->game_center_leaderboard_sets_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_leaderboard_set_update_request** | [**GameCenterLeaderboardSetUpdateRequest**](GameCenterLeaderboardSetUpdateRequest.md)| GameCenterLeaderboardSet representation | 

### Return type

[**GameCenterLeaderboardSetResponse**](GameCenterLeaderboardSetResponse.md)

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
**200** | Single GameCenterLeaderboardSet |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

