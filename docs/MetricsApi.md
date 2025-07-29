# openapi_client.MetricsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apps_beta_tester_usages_get_metrics**](MetricsApi.md#apps_beta_tester_usages_get_metrics) | **GET** /v1/apps/{id}/metrics/betaTesterUsages | 
[**beta_groups_beta_tester_usages_get_metrics**](MetricsApi.md#beta_groups_beta_tester_usages_get_metrics) | **GET** /v1/betaGroups/{id}/metrics/betaTesterUsages | 
[**beta_groups_public_link_usages_get_metrics**](MetricsApi.md#beta_groups_public_link_usages_get_metrics) | **GET** /v1/betaGroups/{id}/metrics/publicLinkUsages | 
[**beta_testers_beta_tester_usages_get_metrics**](MetricsApi.md#beta_testers_beta_tester_usages_get_metrics) | **GET** /v1/betaTesters/{id}/metrics/betaTesterUsages | 
[**builds_beta_build_usages_get_metrics**](MetricsApi.md#builds_beta_build_usages_get_metrics) | **GET** /v1/builds/{id}/metrics/betaBuildUsages | 
[**game_center_details_classic_matchmaking_requests_get_metrics**](MetricsApi.md#game_center_details_classic_matchmaking_requests_get_metrics) | **GET** /v1/gameCenterDetails/{id}/metrics/classicMatchmakingRequests | 
[**game_center_details_rule_based_matchmaking_requests_get_metrics**](MetricsApi.md#game_center_details_rule_based_matchmaking_requests_get_metrics) | **GET** /v1/gameCenterDetails/{id}/metrics/ruleBasedMatchmakingRequests | 
[**game_center_matchmaking_queues_experiment_matchmaking_queue_sizes_get_metrics**](MetricsApi.md#game_center_matchmaking_queues_experiment_matchmaking_queue_sizes_get_metrics) | **GET** /v1/gameCenterMatchmakingQueues/{id}/metrics/experimentMatchmakingQueueSizes | 
[**game_center_matchmaking_queues_experiment_matchmaking_requests_get_metrics**](MetricsApi.md#game_center_matchmaking_queues_experiment_matchmaking_requests_get_metrics) | **GET** /v1/gameCenterMatchmakingQueues/{id}/metrics/experimentMatchmakingRequests | 
[**game_center_matchmaking_queues_matchmaking_queue_sizes_get_metrics**](MetricsApi.md#game_center_matchmaking_queues_matchmaking_queue_sizes_get_metrics) | **GET** /v1/gameCenterMatchmakingQueues/{id}/metrics/matchmakingQueueSizes | 
[**game_center_matchmaking_queues_matchmaking_requests_get_metrics**](MetricsApi.md#game_center_matchmaking_queues_matchmaking_requests_get_metrics) | **GET** /v1/gameCenterMatchmakingQueues/{id}/metrics/matchmakingRequests | 
[**game_center_matchmaking_queues_matchmaking_sessions_get_metrics**](MetricsApi.md#game_center_matchmaking_queues_matchmaking_sessions_get_metrics) | **GET** /v1/gameCenterMatchmakingQueues/{id}/metrics/matchmakingSessions | 
[**game_center_matchmaking_rules_matchmaking_boolean_rule_results_get_metrics**](MetricsApi.md#game_center_matchmaking_rules_matchmaking_boolean_rule_results_get_metrics) | **GET** /v1/gameCenterMatchmakingRules/{id}/metrics/matchmakingBooleanRuleResults | 
[**game_center_matchmaking_rules_matchmaking_number_rule_results_get_metrics**](MetricsApi.md#game_center_matchmaking_rules_matchmaking_number_rule_results_get_metrics) | **GET** /v1/gameCenterMatchmakingRules/{id}/metrics/matchmakingNumberRuleResults | 
[**game_center_matchmaking_rules_matchmaking_rule_errors_get_metrics**](MetricsApi.md#game_center_matchmaking_rules_matchmaking_rule_errors_get_metrics) | **GET** /v1/gameCenterMatchmakingRules/{id}/metrics/matchmakingRuleErrors | 


# **apps_beta_tester_usages_get_metrics**
> AppsBetaTesterUsagesV1MetricResponse apps_beta_tester_usages_get_metrics(id, period=period, group_by=group_by, filter_beta_testers=filter_beta_testers, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.apps_beta_tester_usages_v1_metric_response import AppsBetaTesterUsagesV1MetricResponse
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
    api_instance = openapi_client.MetricsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    period = 'P7D' # str | the duration of the reporting period (optional)
    group_by = ['group_by_example'] # List[str] | the dimension by which to group the results (optional)
    filter_beta_testers = 'filter_beta_testers_example' # str | filter by 'betaTesters' relationship dimension (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.apps_beta_tester_usages_get_metrics(id, period=period, group_by=group_by, filter_beta_testers=filter_beta_testers, limit=limit)
        print("The response of MetricsApi->apps_beta_tester_usages_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MetricsApi->apps_beta_tester_usages_get_metrics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **period** | **str**| the duration of the reporting period | [optional] 
 **group_by** | [**List[str]**](str.md)| the dimension by which to group the results | [optional] 
 **filter_beta_testers** | **str**| filter by &#39;betaTesters&#39; relationship dimension | [optional] 
 **limit** | **int**| maximum number of groups to return per page | [optional] 

### Return type

[**AppsBetaTesterUsagesV1MetricResponse**](AppsBetaTesterUsagesV1MetricResponse.md)

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

# **beta_groups_beta_tester_usages_get_metrics**
> AppsBetaTesterUsagesV1MetricResponse beta_groups_beta_tester_usages_get_metrics(id, period=period, group_by=group_by, filter_beta_testers=filter_beta_testers, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.apps_beta_tester_usages_v1_metric_response import AppsBetaTesterUsagesV1MetricResponse
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
    api_instance = openapi_client.MetricsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    period = 'P7D' # str | the duration of the reporting period (optional)
    group_by = ['group_by_example'] # List[str] | the dimension by which to group the results (optional)
    filter_beta_testers = 'filter_beta_testers_example' # str | filter by 'betaTesters' relationship dimension (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.beta_groups_beta_tester_usages_get_metrics(id, period=period, group_by=group_by, filter_beta_testers=filter_beta_testers, limit=limit)
        print("The response of MetricsApi->beta_groups_beta_tester_usages_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MetricsApi->beta_groups_beta_tester_usages_get_metrics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **period** | **str**| the duration of the reporting period | [optional] 
 **group_by** | [**List[str]**](str.md)| the dimension by which to group the results | [optional] 
 **filter_beta_testers** | **str**| filter by &#39;betaTesters&#39; relationship dimension | [optional] 
 **limit** | **int**| maximum number of groups to return per page | [optional] 

### Return type

[**AppsBetaTesterUsagesV1MetricResponse**](AppsBetaTesterUsagesV1MetricResponse.md)

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

# **beta_groups_public_link_usages_get_metrics**
> BetaPublicLinkUsagesV1MetricResponse beta_groups_public_link_usages_get_metrics(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.beta_public_link_usages_v1_metric_response import BetaPublicLinkUsagesV1MetricResponse
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
    api_instance = openapi_client.MetricsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.beta_groups_public_link_usages_get_metrics(id, limit=limit)
        print("The response of MetricsApi->beta_groups_public_link_usages_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MetricsApi->beta_groups_public_link_usages_get_metrics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum number of groups to return per page | [optional] 

### Return type

[**BetaPublicLinkUsagesV1MetricResponse**](BetaPublicLinkUsagesV1MetricResponse.md)

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

# **beta_testers_beta_tester_usages_get_metrics**
> BetaTesterUsagesV1MetricResponse beta_testers_beta_tester_usages_get_metrics(id, filter_apps, period=period, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.beta_tester_usages_v1_metric_response import BetaTesterUsagesV1MetricResponse
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
    api_instance = openapi_client.MetricsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_apps = 'filter_apps_example' # str | filter by 'apps' relationship dimension
    period = 'P7D' # str | the duration of the reporting period (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.beta_testers_beta_tester_usages_get_metrics(id, filter_apps, period=period, limit=limit)
        print("The response of MetricsApi->beta_testers_beta_tester_usages_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MetricsApi->beta_testers_beta_tester_usages_get_metrics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_apps** | **str**| filter by &#39;apps&#39; relationship dimension | 
 **period** | **str**| the duration of the reporting period | [optional] 
 **limit** | **int**| maximum number of groups to return per page | [optional] 

### Return type

[**BetaTesterUsagesV1MetricResponse**](BetaTesterUsagesV1MetricResponse.md)

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

# **builds_beta_build_usages_get_metrics**
> BetaBuildUsagesV1MetricResponse builds_beta_build_usages_get_metrics(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.beta_build_usages_v1_metric_response import BetaBuildUsagesV1MetricResponse
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
    api_instance = openapi_client.MetricsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.builds_beta_build_usages_get_metrics(id, limit=limit)
        print("The response of MetricsApi->builds_beta_build_usages_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MetricsApi->builds_beta_build_usages_get_metrics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum number of groups to return per page | [optional] 

### Return type

[**BetaBuildUsagesV1MetricResponse**](BetaBuildUsagesV1MetricResponse.md)

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

# **game_center_details_classic_matchmaking_requests_get_metrics**
> GameCenterMatchmakingAppRequestsV1MetricResponse game_center_details_classic_matchmaking_requests_get_metrics(id, granularity, group_by=group_by, filter_result=filter_result, sort=sort, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_app_requests_v1_metric_response import GameCenterMatchmakingAppRequestsV1MetricResponse
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
    api_instance = openapi_client.MetricsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    granularity = 'P7D' # str | the granularity of the per-group dataset
    group_by = ['group_by_example'] # List[str] | the dimension by which to group the results (optional)
    filter_result = 'filter_result_example' # str | filter by 'result' attribute dimension (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; metrics will be sorted as specified (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.game_center_details_classic_matchmaking_requests_get_metrics(id, granularity, group_by=group_by, filter_result=filter_result, sort=sort, limit=limit)
        print("The response of MetricsApi->game_center_details_classic_matchmaking_requests_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MetricsApi->game_center_details_classic_matchmaking_requests_get_metrics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **granularity** | **str**| the granularity of the per-group dataset | 
 **group_by** | [**List[str]**](str.md)| the dimension by which to group the results | [optional] 
 **filter_result** | **str**| filter by &#39;result&#39; attribute dimension | [optional] 
 **sort** | [**List[str]**](str.md)| comma-separated list of sort expressions; metrics will be sorted as specified | [optional] 
 **limit** | **int**| maximum number of groups to return per page | [optional] 

### Return type

[**GameCenterMatchmakingAppRequestsV1MetricResponse**](GameCenterMatchmakingAppRequestsV1MetricResponse.md)

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

# **game_center_details_rule_based_matchmaking_requests_get_metrics**
> GameCenterMatchmakingAppRequestsV1MetricResponse game_center_details_rule_based_matchmaking_requests_get_metrics(id, granularity, group_by=group_by, filter_result=filter_result, sort=sort, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_app_requests_v1_metric_response import GameCenterMatchmakingAppRequestsV1MetricResponse
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
    api_instance = openapi_client.MetricsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    granularity = 'P7D' # str | the granularity of the per-group dataset
    group_by = ['group_by_example'] # List[str] | the dimension by which to group the results (optional)
    filter_result = 'filter_result_example' # str | filter by 'result' attribute dimension (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; metrics will be sorted as specified (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.game_center_details_rule_based_matchmaking_requests_get_metrics(id, granularity, group_by=group_by, filter_result=filter_result, sort=sort, limit=limit)
        print("The response of MetricsApi->game_center_details_rule_based_matchmaking_requests_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MetricsApi->game_center_details_rule_based_matchmaking_requests_get_metrics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **granularity** | **str**| the granularity of the per-group dataset | 
 **group_by** | [**List[str]**](str.md)| the dimension by which to group the results | [optional] 
 **filter_result** | **str**| filter by &#39;result&#39; attribute dimension | [optional] 
 **sort** | [**List[str]**](str.md)| comma-separated list of sort expressions; metrics will be sorted as specified | [optional] 
 **limit** | **int**| maximum number of groups to return per page | [optional] 

### Return type

[**GameCenterMatchmakingAppRequestsV1MetricResponse**](GameCenterMatchmakingAppRequestsV1MetricResponse.md)

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

# **game_center_matchmaking_queues_experiment_matchmaking_queue_sizes_get_metrics**
> GameCenterMatchmakingQueueSizesV1MetricResponse game_center_matchmaking_queues_experiment_matchmaking_queue_sizes_get_metrics(id, granularity, sort=sort, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_queue_sizes_v1_metric_response import GameCenterMatchmakingQueueSizesV1MetricResponse
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
    api_instance = openapi_client.MetricsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    granularity = 'P7D' # str | the granularity of the per-group dataset
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; metrics will be sorted as specified (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_queues_experiment_matchmaking_queue_sizes_get_metrics(id, granularity, sort=sort, limit=limit)
        print("The response of MetricsApi->game_center_matchmaking_queues_experiment_matchmaking_queue_sizes_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MetricsApi->game_center_matchmaking_queues_experiment_matchmaking_queue_sizes_get_metrics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **granularity** | **str**| the granularity of the per-group dataset | 
 **sort** | [**List[str]**](str.md)| comma-separated list of sort expressions; metrics will be sorted as specified | [optional] 
 **limit** | **int**| maximum number of groups to return per page | [optional] 

### Return type

[**GameCenterMatchmakingQueueSizesV1MetricResponse**](GameCenterMatchmakingQueueSizesV1MetricResponse.md)

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

# **game_center_matchmaking_queues_experiment_matchmaking_requests_get_metrics**
> GameCenterMatchmakingQueueRequestsV1MetricResponse game_center_matchmaking_queues_experiment_matchmaking_requests_get_metrics(id, granularity, group_by=group_by, filter_result=filter_result, filter_game_center_detail=filter_game_center_detail, sort=sort, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_queue_requests_v1_metric_response import GameCenterMatchmakingQueueRequestsV1MetricResponse
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
    api_instance = openapi_client.MetricsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    granularity = 'P7D' # str | the granularity of the per-group dataset
    group_by = ['group_by_example'] # List[str] | the dimension by which to group the results (optional)
    filter_result = 'filter_result_example' # str | filter by 'result' attribute dimension (optional)
    filter_game_center_detail = 'filter_game_center_detail_example' # str | filter by 'gameCenterDetail' relationship dimension (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; metrics will be sorted as specified (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_queues_experiment_matchmaking_requests_get_metrics(id, granularity, group_by=group_by, filter_result=filter_result, filter_game_center_detail=filter_game_center_detail, sort=sort, limit=limit)
        print("The response of MetricsApi->game_center_matchmaking_queues_experiment_matchmaking_requests_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MetricsApi->game_center_matchmaking_queues_experiment_matchmaking_requests_get_metrics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **granularity** | **str**| the granularity of the per-group dataset | 
 **group_by** | [**List[str]**](str.md)| the dimension by which to group the results | [optional] 
 **filter_result** | **str**| filter by &#39;result&#39; attribute dimension | [optional] 
 **filter_game_center_detail** | **str**| filter by &#39;gameCenterDetail&#39; relationship dimension | [optional] 
 **sort** | [**List[str]**](str.md)| comma-separated list of sort expressions; metrics will be sorted as specified | [optional] 
 **limit** | **int**| maximum number of groups to return per page | [optional] 

### Return type

[**GameCenterMatchmakingQueueRequestsV1MetricResponse**](GameCenterMatchmakingQueueRequestsV1MetricResponse.md)

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

# **game_center_matchmaking_queues_matchmaking_queue_sizes_get_metrics**
> GameCenterMatchmakingQueueSizesV1MetricResponse game_center_matchmaking_queues_matchmaking_queue_sizes_get_metrics(id, granularity, sort=sort, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_queue_sizes_v1_metric_response import GameCenterMatchmakingQueueSizesV1MetricResponse
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
    api_instance = openapi_client.MetricsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    granularity = 'P7D' # str | the granularity of the per-group dataset
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; metrics will be sorted as specified (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_queues_matchmaking_queue_sizes_get_metrics(id, granularity, sort=sort, limit=limit)
        print("The response of MetricsApi->game_center_matchmaking_queues_matchmaking_queue_sizes_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MetricsApi->game_center_matchmaking_queues_matchmaking_queue_sizes_get_metrics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **granularity** | **str**| the granularity of the per-group dataset | 
 **sort** | [**List[str]**](str.md)| comma-separated list of sort expressions; metrics will be sorted as specified | [optional] 
 **limit** | **int**| maximum number of groups to return per page | [optional] 

### Return type

[**GameCenterMatchmakingQueueSizesV1MetricResponse**](GameCenterMatchmakingQueueSizesV1MetricResponse.md)

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

# **game_center_matchmaking_queues_matchmaking_requests_get_metrics**
> GameCenterMatchmakingQueueRequestsV1MetricResponse game_center_matchmaking_queues_matchmaking_requests_get_metrics(id, granularity, group_by=group_by, filter_result=filter_result, filter_game_center_detail=filter_game_center_detail, sort=sort, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_queue_requests_v1_metric_response import GameCenterMatchmakingQueueRequestsV1MetricResponse
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
    api_instance = openapi_client.MetricsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    granularity = 'P7D' # str | the granularity of the per-group dataset
    group_by = ['group_by_example'] # List[str] | the dimension by which to group the results (optional)
    filter_result = 'filter_result_example' # str | filter by 'result' attribute dimension (optional)
    filter_game_center_detail = 'filter_game_center_detail_example' # str | filter by 'gameCenterDetail' relationship dimension (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; metrics will be sorted as specified (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_queues_matchmaking_requests_get_metrics(id, granularity, group_by=group_by, filter_result=filter_result, filter_game_center_detail=filter_game_center_detail, sort=sort, limit=limit)
        print("The response of MetricsApi->game_center_matchmaking_queues_matchmaking_requests_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MetricsApi->game_center_matchmaking_queues_matchmaking_requests_get_metrics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **granularity** | **str**| the granularity of the per-group dataset | 
 **group_by** | [**List[str]**](str.md)| the dimension by which to group the results | [optional] 
 **filter_result** | **str**| filter by &#39;result&#39; attribute dimension | [optional] 
 **filter_game_center_detail** | **str**| filter by &#39;gameCenterDetail&#39; relationship dimension | [optional] 
 **sort** | [**List[str]**](str.md)| comma-separated list of sort expressions; metrics will be sorted as specified | [optional] 
 **limit** | **int**| maximum number of groups to return per page | [optional] 

### Return type

[**GameCenterMatchmakingQueueRequestsV1MetricResponse**](GameCenterMatchmakingQueueRequestsV1MetricResponse.md)

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

# **game_center_matchmaking_queues_matchmaking_sessions_get_metrics**
> GameCenterMatchmakingSessionsV1MetricResponse game_center_matchmaking_queues_matchmaking_sessions_get_metrics(id, granularity, sort=sort, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_sessions_v1_metric_response import GameCenterMatchmakingSessionsV1MetricResponse
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
    api_instance = openapi_client.MetricsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    granularity = 'P7D' # str | the granularity of the per-group dataset
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; metrics will be sorted as specified (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_queues_matchmaking_sessions_get_metrics(id, granularity, sort=sort, limit=limit)
        print("The response of MetricsApi->game_center_matchmaking_queues_matchmaking_sessions_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MetricsApi->game_center_matchmaking_queues_matchmaking_sessions_get_metrics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **granularity** | **str**| the granularity of the per-group dataset | 
 **sort** | [**List[str]**](str.md)| comma-separated list of sort expressions; metrics will be sorted as specified | [optional] 
 **limit** | **int**| maximum number of groups to return per page | [optional] 

### Return type

[**GameCenterMatchmakingSessionsV1MetricResponse**](GameCenterMatchmakingSessionsV1MetricResponse.md)

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
    api_instance = openapi_client.MetricsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    granularity = 'P7D' # str | the granularity of the per-group dataset
    group_by = ['group_by_example'] # List[str] | the dimension by which to group the results (optional)
    filter_result = 'filter_result_example' # str | filter by 'result' attribute dimension (optional)
    filter_game_center_matchmaking_queue = 'filter_game_center_matchmaking_queue_example' # str | filter by 'gameCenterMatchmakingQueue' relationship dimension (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; metrics will be sorted as specified (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_rules_matchmaking_boolean_rule_results_get_metrics(id, granularity, group_by=group_by, filter_result=filter_result, filter_game_center_matchmaking_queue=filter_game_center_matchmaking_queue, sort=sort, limit=limit)
        print("The response of MetricsApi->game_center_matchmaking_rules_matchmaking_boolean_rule_results_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MetricsApi->game_center_matchmaking_rules_matchmaking_boolean_rule_results_get_metrics: %s\n" % e)
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
    api_instance = openapi_client.MetricsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    granularity = 'P7D' # str | the granularity of the per-group dataset
    group_by = ['group_by_example'] # List[str] | the dimension by which to group the results (optional)
    filter_game_center_matchmaking_queue = 'filter_game_center_matchmaking_queue_example' # str | filter by 'gameCenterMatchmakingQueue' relationship dimension (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; metrics will be sorted as specified (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_rules_matchmaking_number_rule_results_get_metrics(id, granularity, group_by=group_by, filter_game_center_matchmaking_queue=filter_game_center_matchmaking_queue, sort=sort, limit=limit)
        print("The response of MetricsApi->game_center_matchmaking_rules_matchmaking_number_rule_results_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MetricsApi->game_center_matchmaking_rules_matchmaking_number_rule_results_get_metrics: %s\n" % e)
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
    api_instance = openapi_client.MetricsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    granularity = 'P7D' # str | the granularity of the per-group dataset
    group_by = ['group_by_example'] # List[str] | the dimension by which to group the results (optional)
    filter_game_center_matchmaking_queue = 'filter_game_center_matchmaking_queue_example' # str | filter by 'gameCenterMatchmakingQueue' relationship dimension (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; metrics will be sorted as specified (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_rules_matchmaking_rule_errors_get_metrics(id, granularity, group_by=group_by, filter_game_center_matchmaking_queue=filter_game_center_matchmaking_queue, sort=sort, limit=limit)
        print("The response of MetricsApi->game_center_matchmaking_rules_matchmaking_rule_errors_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MetricsApi->game_center_matchmaking_rules_matchmaking_rule_errors_get_metrics: %s\n" % e)
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

