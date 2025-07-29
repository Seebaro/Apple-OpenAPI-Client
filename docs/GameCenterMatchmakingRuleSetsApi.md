# openapi_client.GameCenterMatchmakingRuleSetsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**game_center_matchmaking_rule_sets_create_instance**](GameCenterMatchmakingRuleSetsApi.md#game_center_matchmaking_rule_sets_create_instance) | **POST** /v1/gameCenterMatchmakingRuleSets | 
[**game_center_matchmaking_rule_sets_delete_instance**](GameCenterMatchmakingRuleSetsApi.md#game_center_matchmaking_rule_sets_delete_instance) | **DELETE** /v1/gameCenterMatchmakingRuleSets/{id} | 
[**game_center_matchmaking_rule_sets_get_collection**](GameCenterMatchmakingRuleSetsApi.md#game_center_matchmaking_rule_sets_get_collection) | **GET** /v1/gameCenterMatchmakingRuleSets | 
[**game_center_matchmaking_rule_sets_get_instance**](GameCenterMatchmakingRuleSetsApi.md#game_center_matchmaking_rule_sets_get_instance) | **GET** /v1/gameCenterMatchmakingRuleSets/{id} | 
[**game_center_matchmaking_rule_sets_matchmaking_queues_get_to_many_related**](GameCenterMatchmakingRuleSetsApi.md#game_center_matchmaking_rule_sets_matchmaking_queues_get_to_many_related) | **GET** /v1/gameCenterMatchmakingRuleSets/{id}/matchmakingQueues | 
[**game_center_matchmaking_rule_sets_matchmaking_queues_get_to_many_relationship**](GameCenterMatchmakingRuleSetsApi.md#game_center_matchmaking_rule_sets_matchmaking_queues_get_to_many_relationship) | **GET** /v1/gameCenterMatchmakingRuleSets/{id}/relationships/matchmakingQueues | 
[**game_center_matchmaking_rule_sets_rules_get_to_many_related**](GameCenterMatchmakingRuleSetsApi.md#game_center_matchmaking_rule_sets_rules_get_to_many_related) | **GET** /v1/gameCenterMatchmakingRuleSets/{id}/rules | 
[**game_center_matchmaking_rule_sets_rules_get_to_many_relationship**](GameCenterMatchmakingRuleSetsApi.md#game_center_matchmaking_rule_sets_rules_get_to_many_relationship) | **GET** /v1/gameCenterMatchmakingRuleSets/{id}/relationships/rules | 
[**game_center_matchmaking_rule_sets_teams_get_to_many_related**](GameCenterMatchmakingRuleSetsApi.md#game_center_matchmaking_rule_sets_teams_get_to_many_related) | **GET** /v1/gameCenterMatchmakingRuleSets/{id}/teams | 
[**game_center_matchmaking_rule_sets_teams_get_to_many_relationship**](GameCenterMatchmakingRuleSetsApi.md#game_center_matchmaking_rule_sets_teams_get_to_many_relationship) | **GET** /v1/gameCenterMatchmakingRuleSets/{id}/relationships/teams | 
[**game_center_matchmaking_rule_sets_update_instance**](GameCenterMatchmakingRuleSetsApi.md#game_center_matchmaking_rule_sets_update_instance) | **PATCH** /v1/gameCenterMatchmakingRuleSets/{id} | 


# **game_center_matchmaking_rule_sets_create_instance**
> GameCenterMatchmakingRuleSetResponse game_center_matchmaking_rule_sets_create_instance(game_center_matchmaking_rule_set_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_rule_set_create_request import GameCenterMatchmakingRuleSetCreateRequest
from openapi_client.models.game_center_matchmaking_rule_set_response import GameCenterMatchmakingRuleSetResponse
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
    api_instance = openapi_client.GameCenterMatchmakingRuleSetsApi(api_client)
    game_center_matchmaking_rule_set_create_request = openapi_client.GameCenterMatchmakingRuleSetCreateRequest() # GameCenterMatchmakingRuleSetCreateRequest | GameCenterMatchmakingRuleSet representation

    try:
        api_response = api_instance.game_center_matchmaking_rule_sets_create_instance(game_center_matchmaking_rule_set_create_request)
        print("The response of GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **game_center_matchmaking_rule_set_create_request** | [**GameCenterMatchmakingRuleSetCreateRequest**](GameCenterMatchmakingRuleSetCreateRequest.md)| GameCenterMatchmakingRuleSet representation | 

### Return type

[**GameCenterMatchmakingRuleSetResponse**](GameCenterMatchmakingRuleSetResponse.md)

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
**201** | Single GameCenterMatchmakingRuleSet |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_matchmaking_rule_sets_delete_instance**
> game_center_matchmaking_rule_sets_delete_instance(id)

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
    api_instance = openapi_client.GameCenterMatchmakingRuleSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.game_center_matchmaking_rule_sets_delete_instance(id)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_delete_instance: %s\n" % e)
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

# **game_center_matchmaking_rule_sets_get_collection**
> GameCenterMatchmakingRuleSetsResponse game_center_matchmaking_rule_sets_get_collection(fields_game_center_matchmaking_rule_sets=fields_game_center_matchmaking_rule_sets, fields_game_center_matchmaking_teams=fields_game_center_matchmaking_teams, fields_game_center_matchmaking_rules=fields_game_center_matchmaking_rules, fields_game_center_matchmaking_queues=fields_game_center_matchmaking_queues, limit=limit, include=include, limit_matchmaking_queues=limit_matchmaking_queues, limit_rules=limit_rules, limit_teams=limit_teams)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_rule_sets_response import GameCenterMatchmakingRuleSetsResponse
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
    api_instance = openapi_client.GameCenterMatchmakingRuleSetsApi(api_client)
    fields_game_center_matchmaking_rule_sets = ['fields_game_center_matchmaking_rule_sets_example'] # List[str] | the fields to include for returned resources of type gameCenterMatchmakingRuleSets (optional)
    fields_game_center_matchmaking_teams = ['fields_game_center_matchmaking_teams_example'] # List[str] | the fields to include for returned resources of type gameCenterMatchmakingTeams (optional)
    fields_game_center_matchmaking_rules = ['fields_game_center_matchmaking_rules_example'] # List[str] | the fields to include for returned resources of type gameCenterMatchmakingRules (optional)
    fields_game_center_matchmaking_queues = ['fields_game_center_matchmaking_queues_example'] # List[str] | the fields to include for returned resources of type gameCenterMatchmakingQueues (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_matchmaking_queues = 56 # int | maximum number of related matchmakingQueues returned (when they are included) (optional)
    limit_rules = 56 # int | maximum number of related rules returned (when they are included) (optional)
    limit_teams = 56 # int | maximum number of related teams returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_matchmaking_rule_sets_get_collection(fields_game_center_matchmaking_rule_sets=fields_game_center_matchmaking_rule_sets, fields_game_center_matchmaking_teams=fields_game_center_matchmaking_teams, fields_game_center_matchmaking_rules=fields_game_center_matchmaking_rules, fields_game_center_matchmaking_queues=fields_game_center_matchmaking_queues, limit=limit, include=include, limit_matchmaking_queues=limit_matchmaking_queues, limit_rules=limit_rules, limit_teams=limit_teams)
        print("The response of GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_get_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_get_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fields_game_center_matchmaking_rule_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterMatchmakingRuleSets | [optional] 
 **fields_game_center_matchmaking_teams** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterMatchmakingTeams | [optional] 
 **fields_game_center_matchmaking_rules** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterMatchmakingRules | [optional] 
 **fields_game_center_matchmaking_queues** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterMatchmakingQueues | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_matchmaking_queues** | **int**| maximum number of related matchmakingQueues returned (when they are included) | [optional] 
 **limit_rules** | **int**| maximum number of related rules returned (when they are included) | [optional] 
 **limit_teams** | **int**| maximum number of related teams returned (when they are included) | [optional] 

### Return type

[**GameCenterMatchmakingRuleSetsResponse**](GameCenterMatchmakingRuleSetsResponse.md)

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
**200** | List of GameCenterMatchmakingRuleSets |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_matchmaking_rule_sets_get_instance**
> GameCenterMatchmakingRuleSetResponse game_center_matchmaking_rule_sets_get_instance(id, fields_game_center_matchmaking_rule_sets=fields_game_center_matchmaking_rule_sets, fields_game_center_matchmaking_teams=fields_game_center_matchmaking_teams, fields_game_center_matchmaking_rules=fields_game_center_matchmaking_rules, fields_game_center_matchmaking_queues=fields_game_center_matchmaking_queues, include=include, limit_matchmaking_queues=limit_matchmaking_queues, limit_rules=limit_rules, limit_teams=limit_teams)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_rule_set_response import GameCenterMatchmakingRuleSetResponse
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
    api_instance = openapi_client.GameCenterMatchmakingRuleSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_matchmaking_rule_sets = ['fields_game_center_matchmaking_rule_sets_example'] # List[str] | the fields to include for returned resources of type gameCenterMatchmakingRuleSets (optional)
    fields_game_center_matchmaking_teams = ['fields_game_center_matchmaking_teams_example'] # List[str] | the fields to include for returned resources of type gameCenterMatchmakingTeams (optional)
    fields_game_center_matchmaking_rules = ['fields_game_center_matchmaking_rules_example'] # List[str] | the fields to include for returned resources of type gameCenterMatchmakingRules (optional)
    fields_game_center_matchmaking_queues = ['fields_game_center_matchmaking_queues_example'] # List[str] | the fields to include for returned resources of type gameCenterMatchmakingQueues (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_matchmaking_queues = 56 # int | maximum number of related matchmakingQueues returned (when they are included) (optional)
    limit_rules = 56 # int | maximum number of related rules returned (when they are included) (optional)
    limit_teams = 56 # int | maximum number of related teams returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_matchmaking_rule_sets_get_instance(id, fields_game_center_matchmaking_rule_sets=fields_game_center_matchmaking_rule_sets, fields_game_center_matchmaking_teams=fields_game_center_matchmaking_teams, fields_game_center_matchmaking_rules=fields_game_center_matchmaking_rules, fields_game_center_matchmaking_queues=fields_game_center_matchmaking_queues, include=include, limit_matchmaking_queues=limit_matchmaking_queues, limit_rules=limit_rules, limit_teams=limit_teams)
        print("The response of GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_matchmaking_rule_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterMatchmakingRuleSets | [optional] 
 **fields_game_center_matchmaking_teams** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterMatchmakingTeams | [optional] 
 **fields_game_center_matchmaking_rules** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterMatchmakingRules | [optional] 
 **fields_game_center_matchmaking_queues** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterMatchmakingQueues | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_matchmaking_queues** | **int**| maximum number of related matchmakingQueues returned (when they are included) | [optional] 
 **limit_rules** | **int**| maximum number of related rules returned (when they are included) | [optional] 
 **limit_teams** | **int**| maximum number of related teams returned (when they are included) | [optional] 

### Return type

[**GameCenterMatchmakingRuleSetResponse**](GameCenterMatchmakingRuleSetResponse.md)

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
**200** | Single GameCenterMatchmakingRuleSet |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_matchmaking_rule_sets_matchmaking_queues_get_to_many_related**
> GameCenterMatchmakingQueuesResponse game_center_matchmaking_rule_sets_matchmaking_queues_get_to_many_related(id, fields_game_center_matchmaking_queues=fields_game_center_matchmaking_queues, fields_game_center_matchmaking_rule_sets=fields_game_center_matchmaking_rule_sets, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_queues_response import GameCenterMatchmakingQueuesResponse
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
    api_instance = openapi_client.GameCenterMatchmakingRuleSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_matchmaking_queues = ['fields_game_center_matchmaking_queues_example'] # List[str] | the fields to include for returned resources of type gameCenterMatchmakingQueues (optional)
    fields_game_center_matchmaking_rule_sets = ['fields_game_center_matchmaking_rule_sets_example'] # List[str] | the fields to include for returned resources of type gameCenterMatchmakingRuleSets (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.game_center_matchmaking_rule_sets_matchmaking_queues_get_to_many_related(id, fields_game_center_matchmaking_queues=fields_game_center_matchmaking_queues, fields_game_center_matchmaking_rule_sets=fields_game_center_matchmaking_rule_sets, limit=limit, include=include)
        print("The response of GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_matchmaking_queues_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_matchmaking_queues_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_matchmaking_queues** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterMatchmakingQueues | [optional] 
 **fields_game_center_matchmaking_rule_sets** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterMatchmakingRuleSets | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**GameCenterMatchmakingQueuesResponse**](GameCenterMatchmakingQueuesResponse.md)

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
**200** | List of GameCenterMatchmakingQueues |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_matchmaking_rule_sets_matchmaking_queues_get_to_many_relationship**
> GameCenterMatchmakingRuleSetMatchmakingQueuesLinkagesResponse game_center_matchmaking_rule_sets_matchmaking_queues_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_rule_set_matchmaking_queues_linkages_response import GameCenterMatchmakingRuleSetMatchmakingQueuesLinkagesResponse
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
    api_instance = openapi_client.GameCenterMatchmakingRuleSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_rule_sets_matchmaking_queues_get_to_many_relationship(id, limit=limit)
        print("The response of GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_matchmaking_queues_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_matchmaking_queues_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterMatchmakingRuleSetMatchmakingQueuesLinkagesResponse**](GameCenterMatchmakingRuleSetMatchmakingQueuesLinkagesResponse.md)

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

# **game_center_matchmaking_rule_sets_rules_get_to_many_related**
> GameCenterMatchmakingRulesResponse game_center_matchmaking_rule_sets_rules_get_to_many_related(id, fields_game_center_matchmaking_rules=fields_game_center_matchmaking_rules, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_rules_response import GameCenterMatchmakingRulesResponse
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
    api_instance = openapi_client.GameCenterMatchmakingRuleSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_matchmaking_rules = ['fields_game_center_matchmaking_rules_example'] # List[str] | the fields to include for returned resources of type gameCenterMatchmakingRules (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_rule_sets_rules_get_to_many_related(id, fields_game_center_matchmaking_rules=fields_game_center_matchmaking_rules, limit=limit)
        print("The response of GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_rules_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_rules_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_matchmaking_rules** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterMatchmakingRules | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterMatchmakingRulesResponse**](GameCenterMatchmakingRulesResponse.md)

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
**200** | List of GameCenterMatchmakingRules |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_matchmaking_rule_sets_rules_get_to_many_relationship**
> GameCenterMatchmakingRuleSetRulesLinkagesResponse game_center_matchmaking_rule_sets_rules_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_rule_set_rules_linkages_response import GameCenterMatchmakingRuleSetRulesLinkagesResponse
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
    api_instance = openapi_client.GameCenterMatchmakingRuleSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_rule_sets_rules_get_to_many_relationship(id, limit=limit)
        print("The response of GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_rules_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_rules_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterMatchmakingRuleSetRulesLinkagesResponse**](GameCenterMatchmakingRuleSetRulesLinkagesResponse.md)

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

# **game_center_matchmaking_rule_sets_teams_get_to_many_related**
> GameCenterMatchmakingTeamsResponse game_center_matchmaking_rule_sets_teams_get_to_many_related(id, fields_game_center_matchmaking_teams=fields_game_center_matchmaking_teams, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_teams_response import GameCenterMatchmakingTeamsResponse
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
    api_instance = openapi_client.GameCenterMatchmakingRuleSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_matchmaking_teams = ['fields_game_center_matchmaking_teams_example'] # List[str] | the fields to include for returned resources of type gameCenterMatchmakingTeams (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_rule_sets_teams_get_to_many_related(id, fields_game_center_matchmaking_teams=fields_game_center_matchmaking_teams, limit=limit)
        print("The response of GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_teams_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_teams_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_matchmaking_teams** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterMatchmakingTeams | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterMatchmakingTeamsResponse**](GameCenterMatchmakingTeamsResponse.md)

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
**200** | List of GameCenterMatchmakingTeams |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_matchmaking_rule_sets_teams_get_to_many_relationship**
> GameCenterMatchmakingRuleSetTeamsLinkagesResponse game_center_matchmaking_rule_sets_teams_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_rule_set_teams_linkages_response import GameCenterMatchmakingRuleSetTeamsLinkagesResponse
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
    api_instance = openapi_client.GameCenterMatchmakingRuleSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_rule_sets_teams_get_to_many_relationship(id, limit=limit)
        print("The response of GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_teams_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_teams_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterMatchmakingRuleSetTeamsLinkagesResponse**](GameCenterMatchmakingRuleSetTeamsLinkagesResponse.md)

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

# **game_center_matchmaking_rule_sets_update_instance**
> GameCenterMatchmakingRuleSetResponse game_center_matchmaking_rule_sets_update_instance(id, game_center_matchmaking_rule_set_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_rule_set_response import GameCenterMatchmakingRuleSetResponse
from openapi_client.models.game_center_matchmaking_rule_set_update_request import GameCenterMatchmakingRuleSetUpdateRequest
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
    api_instance = openapi_client.GameCenterMatchmakingRuleSetsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_matchmaking_rule_set_update_request = openapi_client.GameCenterMatchmakingRuleSetUpdateRequest() # GameCenterMatchmakingRuleSetUpdateRequest | GameCenterMatchmakingRuleSet representation

    try:
        api_response = api_instance.game_center_matchmaking_rule_sets_update_instance(id, game_center_matchmaking_rule_set_update_request)
        print("The response of GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingRuleSetsApi->game_center_matchmaking_rule_sets_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_matchmaking_rule_set_update_request** | [**GameCenterMatchmakingRuleSetUpdateRequest**](GameCenterMatchmakingRuleSetUpdateRequest.md)| GameCenterMatchmakingRuleSet representation | 

### Return type

[**GameCenterMatchmakingRuleSetResponse**](GameCenterMatchmakingRuleSetResponse.md)

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
**200** | Single GameCenterMatchmakingRuleSet |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

