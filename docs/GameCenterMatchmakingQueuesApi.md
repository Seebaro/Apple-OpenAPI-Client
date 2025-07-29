# openapi_client.GameCenterMatchmakingQueuesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**game_center_matchmaking_queues_create_instance**](GameCenterMatchmakingQueuesApi.md#game_center_matchmaking_queues_create_instance) | **POST** /v1/gameCenterMatchmakingQueues | 
[**game_center_matchmaking_queues_delete_instance**](GameCenterMatchmakingQueuesApi.md#game_center_matchmaking_queues_delete_instance) | **DELETE** /v1/gameCenterMatchmakingQueues/{id} | 
[**game_center_matchmaking_queues_experiment_matchmaking_queue_sizes_get_metrics**](GameCenterMatchmakingQueuesApi.md#game_center_matchmaking_queues_experiment_matchmaking_queue_sizes_get_metrics) | **GET** /v1/gameCenterMatchmakingQueues/{id}/metrics/experimentMatchmakingQueueSizes | 
[**game_center_matchmaking_queues_experiment_matchmaking_requests_get_metrics**](GameCenterMatchmakingQueuesApi.md#game_center_matchmaking_queues_experiment_matchmaking_requests_get_metrics) | **GET** /v1/gameCenterMatchmakingQueues/{id}/metrics/experimentMatchmakingRequests | 
[**game_center_matchmaking_queues_get_collection**](GameCenterMatchmakingQueuesApi.md#game_center_matchmaking_queues_get_collection) | **GET** /v1/gameCenterMatchmakingQueues | 
[**game_center_matchmaking_queues_get_instance**](GameCenterMatchmakingQueuesApi.md#game_center_matchmaking_queues_get_instance) | **GET** /v1/gameCenterMatchmakingQueues/{id} | 
[**game_center_matchmaking_queues_matchmaking_queue_sizes_get_metrics**](GameCenterMatchmakingQueuesApi.md#game_center_matchmaking_queues_matchmaking_queue_sizes_get_metrics) | **GET** /v1/gameCenterMatchmakingQueues/{id}/metrics/matchmakingQueueSizes | 
[**game_center_matchmaking_queues_matchmaking_requests_get_metrics**](GameCenterMatchmakingQueuesApi.md#game_center_matchmaking_queues_matchmaking_requests_get_metrics) | **GET** /v1/gameCenterMatchmakingQueues/{id}/metrics/matchmakingRequests | 
[**game_center_matchmaking_queues_matchmaking_sessions_get_metrics**](GameCenterMatchmakingQueuesApi.md#game_center_matchmaking_queues_matchmaking_sessions_get_metrics) | **GET** /v1/gameCenterMatchmakingQueues/{id}/metrics/matchmakingSessions | 
[**game_center_matchmaking_queues_update_instance**](GameCenterMatchmakingQueuesApi.md#game_center_matchmaking_queues_update_instance) | **PATCH** /v1/gameCenterMatchmakingQueues/{id} | 


# **game_center_matchmaking_queues_create_instance**
> GameCenterMatchmakingQueueResponse game_center_matchmaking_queues_create_instance(game_center_matchmaking_queue_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_queue_create_request import GameCenterMatchmakingQueueCreateRequest
from openapi_client.models.game_center_matchmaking_queue_response import GameCenterMatchmakingQueueResponse
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
    api_instance = openapi_client.GameCenterMatchmakingQueuesApi(api_client)
    game_center_matchmaking_queue_create_request = openapi_client.GameCenterMatchmakingQueueCreateRequest() # GameCenterMatchmakingQueueCreateRequest | GameCenterMatchmakingQueue representation

    try:
        api_response = api_instance.game_center_matchmaking_queues_create_instance(game_center_matchmaking_queue_create_request)
        print("The response of GameCenterMatchmakingQueuesApi->game_center_matchmaking_queues_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingQueuesApi->game_center_matchmaking_queues_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **game_center_matchmaking_queue_create_request** | [**GameCenterMatchmakingQueueCreateRequest**](GameCenterMatchmakingQueueCreateRequest.md)| GameCenterMatchmakingQueue representation | 

### Return type

[**GameCenterMatchmakingQueueResponse**](GameCenterMatchmakingQueueResponse.md)

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
**201** | Single GameCenterMatchmakingQueue |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_matchmaking_queues_delete_instance**
> game_center_matchmaking_queues_delete_instance(id)

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
    api_instance = openapi_client.GameCenterMatchmakingQueuesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.game_center_matchmaking_queues_delete_instance(id)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingQueuesApi->game_center_matchmaking_queues_delete_instance: %s\n" % e)
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
    api_instance = openapi_client.GameCenterMatchmakingQueuesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    granularity = 'P7D' # str | the granularity of the per-group dataset
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; metrics will be sorted as specified (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_queues_experiment_matchmaking_queue_sizes_get_metrics(id, granularity, sort=sort, limit=limit)
        print("The response of GameCenterMatchmakingQueuesApi->game_center_matchmaking_queues_experiment_matchmaking_queue_sizes_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingQueuesApi->game_center_matchmaking_queues_experiment_matchmaking_queue_sizes_get_metrics: %s\n" % e)
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
    api_instance = openapi_client.GameCenterMatchmakingQueuesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    granularity = 'P7D' # str | the granularity of the per-group dataset
    group_by = ['group_by_example'] # List[str] | the dimension by which to group the results (optional)
    filter_result = 'filter_result_example' # str | filter by 'result' attribute dimension (optional)
    filter_game_center_detail = 'filter_game_center_detail_example' # str | filter by 'gameCenterDetail' relationship dimension (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; metrics will be sorted as specified (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_queues_experiment_matchmaking_requests_get_metrics(id, granularity, group_by=group_by, filter_result=filter_result, filter_game_center_detail=filter_game_center_detail, sort=sort, limit=limit)
        print("The response of GameCenterMatchmakingQueuesApi->game_center_matchmaking_queues_experiment_matchmaking_requests_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingQueuesApi->game_center_matchmaking_queues_experiment_matchmaking_requests_get_metrics: %s\n" % e)
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

# **game_center_matchmaking_queues_get_collection**
> GameCenterMatchmakingQueuesResponse game_center_matchmaking_queues_get_collection(fields_game_center_matchmaking_queues=fields_game_center_matchmaking_queues, limit=limit, include=include)

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
    api_instance = openapi_client.GameCenterMatchmakingQueuesApi(api_client)
    fields_game_center_matchmaking_queues = ['fields_game_center_matchmaking_queues_example'] # List[str] | the fields to include for returned resources of type gameCenterMatchmakingQueues (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.game_center_matchmaking_queues_get_collection(fields_game_center_matchmaking_queues=fields_game_center_matchmaking_queues, limit=limit, include=include)
        print("The response of GameCenterMatchmakingQueuesApi->game_center_matchmaking_queues_get_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingQueuesApi->game_center_matchmaking_queues_get_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fields_game_center_matchmaking_queues** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterMatchmakingQueues | [optional] 
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
**200** | List of GameCenterMatchmakingQueues |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_matchmaking_queues_get_instance**
> GameCenterMatchmakingQueueResponse game_center_matchmaking_queues_get_instance(id, fields_game_center_matchmaking_queues=fields_game_center_matchmaking_queues, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_queue_response import GameCenterMatchmakingQueueResponse
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
    api_instance = openapi_client.GameCenterMatchmakingQueuesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_matchmaking_queues = ['fields_game_center_matchmaking_queues_example'] # List[str] | the fields to include for returned resources of type gameCenterMatchmakingQueues (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.game_center_matchmaking_queues_get_instance(id, fields_game_center_matchmaking_queues=fields_game_center_matchmaking_queues, include=include)
        print("The response of GameCenterMatchmakingQueuesApi->game_center_matchmaking_queues_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingQueuesApi->game_center_matchmaking_queues_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_matchmaking_queues** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterMatchmakingQueues | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**GameCenterMatchmakingQueueResponse**](GameCenterMatchmakingQueueResponse.md)

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
**200** | Single GameCenterMatchmakingQueue |  -  |
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
    api_instance = openapi_client.GameCenterMatchmakingQueuesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    granularity = 'P7D' # str | the granularity of the per-group dataset
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; metrics will be sorted as specified (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_queues_matchmaking_queue_sizes_get_metrics(id, granularity, sort=sort, limit=limit)
        print("The response of GameCenterMatchmakingQueuesApi->game_center_matchmaking_queues_matchmaking_queue_sizes_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingQueuesApi->game_center_matchmaking_queues_matchmaking_queue_sizes_get_metrics: %s\n" % e)
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
    api_instance = openapi_client.GameCenterMatchmakingQueuesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    granularity = 'P7D' # str | the granularity of the per-group dataset
    group_by = ['group_by_example'] # List[str] | the dimension by which to group the results (optional)
    filter_result = 'filter_result_example' # str | filter by 'result' attribute dimension (optional)
    filter_game_center_detail = 'filter_game_center_detail_example' # str | filter by 'gameCenterDetail' relationship dimension (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; metrics will be sorted as specified (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_queues_matchmaking_requests_get_metrics(id, granularity, group_by=group_by, filter_result=filter_result, filter_game_center_detail=filter_game_center_detail, sort=sort, limit=limit)
        print("The response of GameCenterMatchmakingQueuesApi->game_center_matchmaking_queues_matchmaking_requests_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingQueuesApi->game_center_matchmaking_queues_matchmaking_requests_get_metrics: %s\n" % e)
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
    api_instance = openapi_client.GameCenterMatchmakingQueuesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    granularity = 'P7D' # str | the granularity of the per-group dataset
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; metrics will be sorted as specified (optional)
    limit = 56 # int | maximum number of groups to return per page (optional)

    try:
        api_response = api_instance.game_center_matchmaking_queues_matchmaking_sessions_get_metrics(id, granularity, sort=sort, limit=limit)
        print("The response of GameCenterMatchmakingQueuesApi->game_center_matchmaking_queues_matchmaking_sessions_get_metrics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingQueuesApi->game_center_matchmaking_queues_matchmaking_sessions_get_metrics: %s\n" % e)
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

# **game_center_matchmaking_queues_update_instance**
> GameCenterMatchmakingQueueResponse game_center_matchmaking_queues_update_instance(id, game_center_matchmaking_queue_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_matchmaking_queue_response import GameCenterMatchmakingQueueResponse
from openapi_client.models.game_center_matchmaking_queue_update_request import GameCenterMatchmakingQueueUpdateRequest
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
    api_instance = openapi_client.GameCenterMatchmakingQueuesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_matchmaking_queue_update_request = openapi_client.GameCenterMatchmakingQueueUpdateRequest() # GameCenterMatchmakingQueueUpdateRequest | GameCenterMatchmakingQueue representation

    try:
        api_response = api_instance.game_center_matchmaking_queues_update_instance(id, game_center_matchmaking_queue_update_request)
        print("The response of GameCenterMatchmakingQueuesApi->game_center_matchmaking_queues_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterMatchmakingQueuesApi->game_center_matchmaking_queues_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_matchmaking_queue_update_request** | [**GameCenterMatchmakingQueueUpdateRequest**](GameCenterMatchmakingQueueUpdateRequest.md)| GameCenterMatchmakingQueue representation | 

### Return type

[**GameCenterMatchmakingQueueResponse**](GameCenterMatchmakingQueueResponse.md)

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
**200** | Single GameCenterMatchmakingQueue |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

