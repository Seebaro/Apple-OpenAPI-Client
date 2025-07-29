# openapi_client.GameCenterMatchmakingRulesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**game_center_matchmaking_rules_create_instance**](GameCenterMatchmakingRulesApi.md#game_center_matchmaking_rules_create_instance) | **POST** /v1/gameCenterMatchmakingRules | 
[**game_center_matchmaking_rules_delete_instance**](GameCenterMatchmakingRulesApi.md#game_center_matchmaking_rules_delete_instance) | **DELETE** /v1/gameCenterMatchmakingRules/{id} | 
[**game_center_matchmaking_rules_matchmaking_boolean_rule_results_get_metrics**](GameCenterMatchmakingRulesApi.md#game_center_matchmaking_rules_matchmaking_boolean_rule_results_get_metrics) | **GET** /v1/gameCenterMatchmakingRules/{id}/metrics/matchmakingBooleanRuleResults | 
[**game_center_matchmaking_rules_matchmaking_number_rule_results_get_metrics**](GameCenterMatchmakingRulesApi.md#game_center_matchmaking_rules_matchmaking_number_rule_results_get_metrics) | **GET** /v1/gameCenterMatchmakingRules/{id}/metrics/matchmakingNumberRuleResults | 
[**game_center_matchmaking_rules_matchmaking_rule_errors_get_metrics**](GameCenterMatchmakingRulesApi.md#game_center_matchmaking_rules_matchmaking_rule_errors_get_metrics) | **GET** /v1/gameCenterMatchmakingRules/{id}/metrics/matchmakingRuleErrors | 
[**game_center_matchmaking_rules_update_instance**](GameCenterMatchmakingRulesApi.md#game_center_matchmaking_rules_update_instance) | **PATCH** /v1/gameCenterMatchmakingRules/{id} | 


# **game_center_matchmaking_rules_create_instance**
> GameCenterMatchmakingRuleResponse game_center_matchmaking_rules_create_instance(game_center_matchmaking_rule_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_rule_create_request import GameCenterMatchmakingRuleCreateRequest
from openapi_client.models.game_center_matchmaking_rule_response import GameCenterMatchmakingRuleResponse
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
    api_instance = openapi_client.GameCenterMatchmakingRulesApi(api_client)
    game_center_matchmaking_rule_create_request = openapi_client.GameCenterMatchmakingRuleCreateRequest() # GameCenterMatchmakingRuleCreateRequest | GameCenterMatchmakingRule representation

    try:
        api_response = api_instance.game_center_matchmaking_rules_create_instance(game_center_matchmaking_rule_create_request)
        print("The response of GameCenterMatchmakingRulesApi->game_center_matchmaking_rules_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingRulesApi->game_center_matchmaking_rules_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **game_center_matchmaking_rule_create_request** | [**GameCenterMatchmakingRuleCreateRequest**](GameCenterMatchmakingRuleCreateRequest.md)| GameCenterMatchmakingRule representation | 

### Return type

[**GameCenterMatchmakingRuleResponse**](GameCenterMatchmakingRuleResponse.md)

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
**201** | Single GameCenterMatchmakingRule |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_matchmaking_rules_delete_instance**
> game_center_matchmaking_rules_delete_instance(id)

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
    api_instance = openapi_client.GameCenterMatchmakingRulesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.game_center_matchmaking_rules_delete_instance(id)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingRulesApi->game_center_matchmaking_rules_delete_instance: %s\n" % e)
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

# **game_center_matchmaking_rules_matchmaking_boolean_rule_results_get_metrics**
> GameCenterMatchmakingBooleanRuleResultsV1MetricResponse game_center_matchmaking_rules_matchmaking_boolean_rule_results_get_metrics(id, granularity, group_by=group_by, filter_result=filter_result, filter_game_center_matchmaking_queue=filter_game_center_matchmaking_queue, sort=sort, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_boolean_rule_results_v1_metric_response import GameCenterMatchmakingBooleanRuleResultsV1MetricResponse
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
    api_instance = openapi_client.GameCenterMatchmakingRulesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    granularity = 'P7D' # str | the granularity of the per-group dataset
    group_by = ['group_by_example'] # List[str] | the dimension by which to group the results (optional)
    filter_result = 'filter_result_example' # str | filter by 'result' attribute dimension (optional)
    filter_game_center_matchmaking_queue = 'filter_game_center_matchmaking_queue_example' # str | filter by 'gameCenterMatchmakingQueue' relationship dimension (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; metrics will be sorted as specified (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_rules_matchmaking_boolean_rule_results_get_metrics(id, granularity, group_by=group_by, filter_result=filter_result, filter_game_center_matchmaking_queue=filter_game_center_matchmaking_queue, sort=sort, limit=limit)
        print("The response of GameCenterMatchmakingRulesApi->game_center_matchmaking_rules_matchmaking_boolean_rule_results_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingRulesApi->game_center_matchmaking_rules_matchmaking_boolean_rule_results_get_metrics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **granularity** | **str**| the granularity of the per-group dataset | 
 **group_by** | [**List[str]**](str.md)| the dimension by which to group the results | [optional] 
 **filter_result** | **str**| filter by &#39;result&#39; attribute dimension | [optional] 
 **filter_game_center_matchmaking_queue** | **str**| filter by &#39;gameCenterMatchmakingQueue&#39; relationship dimension | [optional] 
 **sort** | [**List[str]**](str.md)| comma-separated list of sort expressions; metrics will be sorted as specified | [optional] 
 **limit** | **int**| maximum number of groups to return per page | [optional] 

### Return type

[**GameCenterMatchmakingBooleanRuleResultsV1MetricResponse**](GameCenterMatchmakingBooleanRuleResultsV1MetricResponse.md)

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
**200** | Metrics data response |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_matchmaking_rules_matchmaking_number_rule_results_get_metrics**
> GameCenterMatchmakingNumberRuleResultsV1MetricResponse game_center_matchmaking_rules_matchmaking_number_rule_results_get_metrics(id, granularity, group_by=group_by, filter_game_center_matchmaking_queue=filter_game_center_matchmaking_queue, sort=sort, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_number_rule_results_v1_metric_response import GameCenterMatchmakingNumberRuleResultsV1MetricResponse
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
    api_instance = openapi_client.GameCenterMatchmakingRulesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    granularity = 'P7D' # str | the granularity of the per-group dataset
    group_by = ['group_by_example'] # List[str] | the dimension by which to group the results (optional)
    filter_game_center_matchmaking_queue = 'filter_game_center_matchmaking_queue_example' # str | filter by 'gameCenterMatchmakingQueue' relationship dimension (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; metrics will be sorted as specified (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_rules_matchmaking_number_rule_results_get_metrics(id, granularity, group_by=group_by, filter_game_center_matchmaking_queue=filter_game_center_matchmaking_queue, sort=sort, limit=limit)
        print("The response of GameCenterMatchmakingRulesApi->game_center_matchmaking_rules_matchmaking_number_rule_results_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingRulesApi->game_center_matchmaking_rules_matchmaking_number_rule_results_get_metrics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **granularity** | **str**| the granularity of the per-group dataset | 
 **group_by** | [**List[str]**](str.md)| the dimension by which to group the results | [optional] 
 **filter_game_center_matchmaking_queue** | **str**| filter by &#39;gameCenterMatchmakingQueue&#39; relationship dimension | [optional] 
 **sort** | [**List[str]**](str.md)| comma-separated list of sort expressions; metrics will be sorted as specified | [optional] 
 **limit** | **int**| maximum number of groups to return per page | [optional] 

### Return type

[**GameCenterMatchmakingNumberRuleResultsV1MetricResponse**](GameCenterMatchmakingNumberRuleResultsV1MetricResponse.md)

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
**200** | Metrics data response |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_matchmaking_rules_matchmaking_rule_errors_get_metrics**
> GameCenterMatchmakingRuleErrorsV1MetricResponse game_center_matchmaking_rules_matchmaking_rule_errors_get_metrics(id, granularity, group_by=group_by, filter_game_center_matchmaking_queue=filter_game_center_matchmaking_queue, sort=sort, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_rule_errors_v1_metric_response import GameCenterMatchmakingRuleErrorsV1MetricResponse
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
    api_instance = openapi_client.GameCenterMatchmakingRulesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    granularity = 'P7D' # str | the granularity of the per-group dataset
    group_by = ['group_by_example'] # List[str] | the dimension by which to group the results (optional)
    filter_game_center_matchmaking_queue = 'filter_game_center_matchmaking_queue_example' # str | filter by 'gameCenterMatchmakingQueue' relationship dimension (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; metrics will be sorted as specified (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_rules_matchmaking_rule_errors_get_metrics(id, granularity, group_by=group_by, filter_game_center_matchmaking_queue=filter_game_center_matchmaking_queue, sort=sort, limit=limit)
        print("The response of GameCenterMatchmakingRulesApi->game_center_matchmaking_rules_matchmaking_rule_errors_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingRulesApi->game_center_matchmaking_rules_matchmaking_rule_errors_get_metrics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **granularity** | **str**| the granularity of the per-group dataset | 
 **group_by** | [**List[str]**](str.md)| the dimension by which to group the results | [optional] 
 **filter_game_center_matchmaking_queue** | **str**| filter by &#39;gameCenterMatchmakingQueue&#39; relationship dimension | [optional] 
 **sort** | [**List[str]**](str.md)| comma-separated list of sort expressions; metrics will be sorted as specified | [optional] 
 **limit** | **int**| maximum number of groups to return per page | [optional] 

### Return type

[**GameCenterMatchmakingRuleErrorsV1MetricResponse**](GameCenterMatchmakingRuleErrorsV1MetricResponse.md)

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
**200** | Metrics data response |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_matchmaking_rules_update_instance**
> GameCenterMatchmakingRuleResponse game_center_matchmaking_rules_update_instance(id, game_center_matchmaking_rule_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_rule_response import GameCenterMatchmakingRuleResponse
from openapi_client.models.game_center_matchmaking_rule_update_request import GameCenterMatchmakingRuleUpdateRequest
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
    api_instance = openapi_client.GameCenterMatchmakingRulesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_matchmaking_rule_update_request = openapi_client.GameCenterMatchmakingRuleUpdateRequest() # GameCenterMatchmakingRuleUpdateRequest | GameCenterMatchmakingRule representation

    try:
        api_response = api_instance.game_center_matchmaking_rules_update_instance(id, game_center_matchmaking_rule_update_request)
        print("The response of GameCenterMatchmakingRulesApi->game_center_matchmaking_rules_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingRulesApi->game_center_matchmaking_rules_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_matchmaking_rule_update_request** | [**GameCenterMatchmakingRuleUpdateRequest**](GameCenterMatchmakingRuleUpdateRequest.md)| GameCenterMatchmakingRule representation | 

### Return type

[**GameCenterMatchmakingRuleResponse**](GameCenterMatchmakingRuleResponse.md)

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
**200** | Single GameCenterMatchmakingRule |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

