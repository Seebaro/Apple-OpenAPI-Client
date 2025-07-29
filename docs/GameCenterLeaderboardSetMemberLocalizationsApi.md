# openapi_client.GameCenterLeaderboardSetMemberLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**game_center_leaderboard_set_member_localizations_create_instance**](GameCenterLeaderboardSetMemberLocalizationsApi.md#game_center_leaderboard_set_member_localizations_create_instance) | **POST** /v1/gameCenterLeaderboardSetMemberLocalizations | 
[**game_center_leaderboard_set_member_localizations_delete_instance**](GameCenterLeaderboardSetMemberLocalizationsApi.md#game_center_leaderboard_set_member_localizations_delete_instance) | **DELETE** /v1/gameCenterLeaderboardSetMemberLocalizations/{id} | 
[**game_center_leaderboard_set_member_localizations_game_center_leaderboard_get_to_one_related**](GameCenterLeaderboardSetMemberLocalizationsApi.md#game_center_leaderboard_set_member_localizations_game_center_leaderboard_get_to_one_related) | **GET** /v1/gameCenterLeaderboardSetMemberLocalizations/{id}/gameCenterLeaderboard | 
[**game_center_leaderboard_set_member_localizations_game_center_leaderboard_get_to_one_relationship**](GameCenterLeaderboardSetMemberLocalizationsApi.md#game_center_leaderboard_set_member_localizations_game_center_leaderboard_get_to_one_relationship) | **GET** /v1/gameCenterLeaderboardSetMemberLocalizations/{id}/relationships/gameCenterLeaderboard | 
[**game_center_leaderboard_set_member_localizations_game_center_leaderboard_set_get_to_one_related**](GameCenterLeaderboardSetMemberLocalizationsApi.md#game_center_leaderboard_set_member_localizations_game_center_leaderboard_set_get_to_one_related) | **GET** /v1/gameCenterLeaderboardSetMemberLocalizations/{id}/gameCenterLeaderboardSet | 
[**game_center_leaderboard_set_member_localizations_game_center_leaderboard_set_get_to_one_relationship**](GameCenterLeaderboardSetMemberLocalizationsApi.md#game_center_leaderboard_set_member_localizations_game_center_leaderboard_set_get_to_one_relationship) | **GET** /v1/gameCenterLeaderboardSetMemberLocalizations/{id}/relationships/gameCenterLeaderboardSet | 
[**game_center_leaderboard_set_member_localizations_get_collection**](GameCenterLeaderboardSetMemberLocalizationsApi.md#game_center_leaderboard_set_member_localizations_get_collection) | **GET** /v1/gameCenterLeaderboardSetMemberLocalizations | 
[**game_center_leaderboard_set_member_localizations_update_instance**](GameCenterLeaderboardSetMemberLocalizationsApi.md#game_center_leaderboard_set_member_localizations_update_instance) | **PATCH** /v1/gameCenterLeaderboardSetMemberLocalizations/{id} | 


# **game_center_leaderboard_set_member_localizations_create_instance**
> GameCenterLeaderboardSetMemberLocalizationResponse game_center_leaderboard_set_member_localizations_create_instance(game_center_leaderboard_set_member_localization_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_member_localization_create_request import GameCenterLeaderboardSetMemberLocalizationCreateRequest
from openapi_client.models.game_center_leaderboard_set_member_localization_response import GameCenterLeaderboardSetMemberLocalizationResponse
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
    api_instance = openapi_client.GameCenterLeaderboardSetMemberLocalizationsApi(api_client)
    game_center_leaderboard_set_member_localization_create_request = openapi_client.GameCenterLeaderboardSetMemberLocalizationCreateRequest() # GameCenterLeaderboardSetMemberLocalizationCreateRequest | GameCenterLeaderboardSetMemberLocalization representation

    try:
        api_response = api_instance.game_center_leaderboard_set_member_localizations_create_instance(game_center_leaderboard_set_member_localization_create_request)
        print("The response of GameCenterLeaderboardSetMemberLocalizationsApi->game_center_leaderboard_set_member_localizations_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi->game_center_leaderboard_set_member_localizations_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **game_center_leaderboard_set_member_localization_create_request** | [**GameCenterLeaderboardSetMemberLocalizationCreateRequest**](GameCenterLeaderboardSetMemberLocalizationCreateRequest.md)| GameCenterLeaderboardSetMemberLocalization representation | 

### Return type

[**GameCenterLeaderboardSetMemberLocalizationResponse**](GameCenterLeaderboardSetMemberLocalizationResponse.md)

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
**201** | Single GameCenterLeaderboardSetMemberLocalization |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_leaderboard_set_member_localizations_delete_instance**
> game_center_leaderboard_set_member_localizations_delete_instance(id)

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
    api_instance = openapi_client.GameCenterLeaderboardSetMemberLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.game_center_leaderboard_set_member_localizations_delete_instance(id)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi->game_center_leaderboard_set_member_localizations_delete_instance: %s\n" % e)
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

# **game_center_leaderboard_set_member_localizations_game_center_leaderboard_get_to_one_related**
> GameCenterLeaderboardResponse game_center_leaderboard_set_member_localizations_game_center_leaderboard_get_to_one_related(id, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_leaderboard_localizations=fields_game_center_leaderboard_localizations, fields_game_center_leaderboard_releases=fields_game_center_leaderboard_releases, fields_game_center_activities=fields_game_center_activities, fields_game_center_challenges=fields_game_center_challenges, include=include, limit_game_center_leaderboard_sets=limit_game_center_leaderboard_sets, limit_localizations=limit_localizations, limit_releases=limit_releases)

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
    api_instance = openapi_client.GameCenterLeaderboardSetMemberLocalizationsApi(api_client)
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
        api_response = api_instance.game_center_leaderboard_set_member_localizations_game_center_leaderboard_get_to_one_related(id, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_leaderboard_localizations=fields_game_center_leaderboard_localizations, fields_game_center_leaderboard_releases=fields_game_center_leaderboard_releases, fields_game_center_activities=fields_game_center_activities, fields_game_center_challenges=fields_game_center_challenges, include=include, limit_game_center_leaderboard_sets=limit_game_center_leaderboard_sets, limit_localizations=limit_localizations, limit_releases=limit_releases)
        print("The response of GameCenterLeaderboardSetMemberLocalizationsApi->game_center_leaderboard_set_member_localizations_game_center_leaderboard_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi->game_center_leaderboard_set_member_localizations_game_center_leaderboard_get_to_one_related: %s\n" % e)
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

# **game_center_leaderboard_set_member_localizations_game_center_leaderboard_get_to_one_relationship**
> GameCenterLeaderboardSetMemberLocalizationGameCenterLeaderboardLinkageResponse game_center_leaderboard_set_member_localizations_game_center_leaderboard_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_member_localization_game_center_leaderboard_linkage_response import GameCenterLeaderboardSetMemberLocalizationGameCenterLeaderboardLinkageResponse
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
    api_instance = openapi_client.GameCenterLeaderboardSetMemberLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.game_center_leaderboard_set_member_localizations_game_center_leaderboard_get_to_one_relationship(id)
        print("The response of GameCenterLeaderboardSetMemberLocalizationsApi->game_center_leaderboard_set_member_localizations_game_center_leaderboard_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi->game_center_leaderboard_set_member_localizations_game_center_leaderboard_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**GameCenterLeaderboardSetMemberLocalizationGameCenterLeaderboardLinkageResponse**](GameCenterLeaderboardSetMemberLocalizationGameCenterLeaderboardLinkageResponse.md)

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

# **game_center_leaderboard_set_member_localizations_game_center_leaderboard_set_get_to_one_related**
> GameCenterLeaderboardSetResponse game_center_leaderboard_set_member_localizations_game_center_leaderboard_set_get_to_one_related(id, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_leaderboard_set_localizations=fields_game_center_leaderboard_set_localizations, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_leaderboard_set_releases=fields_game_center_leaderboard_set_releases, include=include, limit_localizations=limit_localizations, limit_game_center_leaderboards=limit_game_center_leaderboards, limit_releases=limit_releases)

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
    api_instance = openapi_client.GameCenterLeaderboardSetMemberLocalizationsApi(api_client)
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
        api_response = api_instance.game_center_leaderboard_set_member_localizations_game_center_leaderboard_set_get_to_one_related(id, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_leaderboard_set_localizations=fields_game_center_leaderboard_set_localizations, fields_game_center_leaderboards=fields_game_center_leaderboards, fields_game_center_leaderboard_set_releases=fields_game_center_leaderboard_set_releases, include=include, limit_localizations=limit_localizations, limit_game_center_leaderboards=limit_game_center_leaderboards, limit_releases=limit_releases)
        print("The response of GameCenterLeaderboardSetMemberLocalizationsApi->game_center_leaderboard_set_member_localizations_game_center_leaderboard_set_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi->game_center_leaderboard_set_member_localizations_game_center_leaderboard_set_get_to_one_related: %s\n" % e)
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

# **game_center_leaderboard_set_member_localizations_game_center_leaderboard_set_get_to_one_relationship**
> GameCenterLeaderboardSetMemberLocalizationGameCenterLeaderboardSetLinkageResponse game_center_leaderboard_set_member_localizations_game_center_leaderboard_set_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_member_localization_game_center_leaderboard_set_linkage_response import GameCenterLeaderboardSetMemberLocalizationGameCenterLeaderboardSetLinkageResponse
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
    api_instance = openapi_client.GameCenterLeaderboardSetMemberLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.game_center_leaderboard_set_member_localizations_game_center_leaderboard_set_get_to_one_relationship(id)
        print("The response of GameCenterLeaderboardSetMemberLocalizationsApi->game_center_leaderboard_set_member_localizations_game_center_leaderboard_set_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi->game_center_leaderboard_set_member_localizations_game_center_leaderboard_set_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**GameCenterLeaderboardSetMemberLocalizationGameCenterLeaderboardSetLinkageResponse**](GameCenterLeaderboardSetMemberLocalizationGameCenterLeaderboardSetLinkageResponse.md)

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

# **game_center_leaderboard_set_member_localizations_get_collection**
> GameCenterLeaderboardSetMemberLocalizationsResponse game_center_leaderboard_set_member_localizations_get_collection(filter_game_center_leaderboard_set, filter_game_center_leaderboard, fields_game_center_leaderboard_set_member_localizations=fields_game_center_leaderboard_set_member_localizations, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_leaderboards=fields_game_center_leaderboards, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_member_localizations_response import GameCenterLeaderboardSetMemberLocalizationsResponse
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
    api_instance = openapi_client.GameCenterLeaderboardSetMemberLocalizationsApi(api_client)
    filter_game_center_leaderboard_set = ['filter_game_center_leaderboard_set_example'] # List[str] | filter by id(s) of related 'gameCenterLeaderboardSet'
    filter_game_center_leaderboard = ['filter_game_center_leaderboard_example'] # List[str] | filter by id(s) of related 'gameCenterLeaderboard'
    fields_game_center_leaderboard_set_member_localizations = ['fields_game_center_leaderboard_set_member_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSetMemberLocalizations (optional)
    fields_game_center_leaderboard_sets = ['fields_game_center_leaderboard_sets_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSets (optional)
    fields_game_center_leaderboards = ['fields_game_center_leaderboards_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboards (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.game_center_leaderboard_set_member_localizations_get_collection(filter_game_center_leaderboard_set, filter_game_center_leaderboard, fields_game_center_leaderboard_set_member_localizations=fields_game_center_leaderboard_set_member_localizations, fields_game_center_leaderboard_sets=fields_game_center_leaderboard_sets, fields_game_center_leaderboards=fields_game_center_leaderboards, limit=limit, include=include)
        print("The response of GameCenterLeaderboardSetMemberLocalizationsApi->game_center_leaderboard_set_member_localizations_get_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi->game_center_leaderboard_set_member_localizations_get_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter_game_center_leaderboard_set** | [**List[str]**](str.md)| filter by id(s) of related &#39;gameCenterLeaderboardSet&#39; | 
 **filter_game_center_leaderboard** | [**List[str]**](str.md)| filter by id(s) of related &#39;gameCenterLeaderboard&#39; | 
 **fields_game_center_leaderboard_set_member_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSetMemberLocalizations | [optional] 
 **fields_game_center_leaderboard_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSets | [optional] 
 **fields_game_center_leaderboards** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboards | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**GameCenterLeaderboardSetMemberLocalizationsResponse**](GameCenterLeaderboardSetMemberLocalizationsResponse.md)

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
**200** | List of GameCenterLeaderboardSetMemberLocalizations |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_leaderboard_set_member_localizations_update_instance**
> GameCenterLeaderboardSetMemberLocalizationResponse game_center_leaderboard_set_member_localizations_update_instance(id, game_center_leaderboard_set_member_localization_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_member_localization_response import GameCenterLeaderboardSetMemberLocalizationResponse
from openapi_client.models.game_center_leaderboard_set_member_localization_update_request import GameCenterLeaderboardSetMemberLocalizationUpdateRequest
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
    api_instance = openapi_client.GameCenterLeaderboardSetMemberLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_leaderboard_set_member_localization_update_request = openapi_client.GameCenterLeaderboardSetMemberLocalizationUpdateRequest() # GameCenterLeaderboardSetMemberLocalizationUpdateRequest | GameCenterLeaderboardSetMemberLocalization representation

    try:
        api_response = api_instance.game_center_leaderboard_set_member_localizations_update_instance(id, game_center_leaderboard_set_member_localization_update_request)
        print("The response of GameCenterLeaderboardSetMemberLocalizationsApi->game_center_leaderboard_set_member_localizations_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetMemberLocalizationsApi->game_center_leaderboard_set_member_localizations_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_leaderboard_set_member_localization_update_request** | [**GameCenterLeaderboardSetMemberLocalizationUpdateRequest**](GameCenterLeaderboardSetMemberLocalizationUpdateRequest.md)| GameCenterLeaderboardSetMemberLocalization representation | 

### Return type

[**GameCenterLeaderboardSetMemberLocalizationResponse**](GameCenterLeaderboardSetMemberLocalizationResponse.md)

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
**200** | Single GameCenterLeaderboardSetMemberLocalization |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

