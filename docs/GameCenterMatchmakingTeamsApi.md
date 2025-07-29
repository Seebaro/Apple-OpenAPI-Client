# openapi_client.GameCenterMatchmakingTeamsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**game_center_matchmaking_teams_create_instance**](GameCenterMatchmakingTeamsApi.md#game_center_matchmaking_teams_create_instance) | **POST** /v1/gameCenterMatchmakingTeams | 
[**game_center_matchmaking_teams_delete_instance**](GameCenterMatchmakingTeamsApi.md#game_center_matchmaking_teams_delete_instance) | **DELETE** /v1/gameCenterMatchmakingTeams/{id} | 
[**game_center_matchmaking_teams_update_instance**](GameCenterMatchmakingTeamsApi.md#game_center_matchmaking_teams_update_instance) | **PATCH** /v1/gameCenterMatchmakingTeams/{id} | 


# **game_center_matchmaking_teams_create_instance**
> GameCenterMatchmakingTeamResponse game_center_matchmaking_teams_create_instance(game_center_matchmaking_team_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_team_create_request import GameCenterMatchmakingTeamCreateRequest
from openapi_client.models.game_center_matchmaking_team_response import GameCenterMatchmakingTeamResponse
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
    api_instance = openapi_client.GameCenterMatchmakingTeamsApi(api_client)
    game_center_matchmaking_team_create_request = openapi_client.GameCenterMatchmakingTeamCreateRequest() # GameCenterMatchmakingTeamCreateRequest | GameCenterMatchmakingTeam representation

    try:
        api_response = api_instance.game_center_matchmaking_teams_create_instance(game_center_matchmaking_team_create_request)
        print("The response of GameCenterMatchmakingTeamsApi->game_center_matchmaking_teams_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingTeamsApi->game_center_matchmaking_teams_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **game_center_matchmaking_team_create_request** | [**GameCenterMatchmakingTeamCreateRequest**](GameCenterMatchmakingTeamCreateRequest.md)| GameCenterMatchmakingTeam representation | 

### Return type

[**GameCenterMatchmakingTeamResponse**](GameCenterMatchmakingTeamResponse.md)

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
**201** | Single GameCenterMatchmakingTeam |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_matchmaking_teams_delete_instance**
> game_center_matchmaking_teams_delete_instance(id)

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
    api_instance = openapi_client.GameCenterMatchmakingTeamsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.game_center_matchmaking_teams_delete_instance(id)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingTeamsApi->game_center_matchmaking_teams_delete_instance: %s\n" % e)
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

# **game_center_matchmaking_teams_update_instance**
> GameCenterMatchmakingTeamResponse game_center_matchmaking_teams_update_instance(id, game_center_matchmaking_team_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_team_response import GameCenterMatchmakingTeamResponse
from openapi_client.models.game_center_matchmaking_team_update_request import GameCenterMatchmakingTeamUpdateRequest
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
    api_instance = openapi_client.GameCenterMatchmakingTeamsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_matchmaking_team_update_request = openapi_client.GameCenterMatchmakingTeamUpdateRequest() # GameCenterMatchmakingTeamUpdateRequest | GameCenterMatchmakingTeam representation

    try:
        api_response = api_instance.game_center_matchmaking_teams_update_instance(id, game_center_matchmaking_team_update_request)
        print("The response of GameCenterMatchmakingTeamsApi->game_center_matchmaking_teams_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingTeamsApi->game_center_matchmaking_teams_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_matchmaking_team_update_request** | [**GameCenterMatchmakingTeamUpdateRequest**](GameCenterMatchmakingTeamUpdateRequest.md)| GameCenterMatchmakingTeam representation | 

### Return type

[**GameCenterMatchmakingTeamResponse**](GameCenterMatchmakingTeamResponse.md)

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
**200** | Single GameCenterMatchmakingTeam |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

