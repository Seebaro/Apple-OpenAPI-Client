# openapi_client.AnalyticsReportInstancesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**analytics_report_instances_get_instance**](AnalyticsReportInstancesApi.md#analytics_report_instances_get_instance) | **GET** /v1/analyticsReportInstances/{id} | 
[**analytics_report_instances_segments_get_to_many_related**](AnalyticsReportInstancesApi.md#analytics_report_instances_segments_get_to_many_related) | **GET** /v1/analyticsReportInstances/{id}/segments | 
[**analytics_report_instances_segments_get_to_many_relationship**](AnalyticsReportInstancesApi.md#analytics_report_instances_segments_get_to_many_relationship) | **GET** /v1/analyticsReportInstances/{id}/relationships/segments | 


# **analytics_report_instances_get_instance**
> AnalyticsReportInstanceResponse analytics_report_instances_get_instance(id, fields_analytics_report_instances=fields_analytics_report_instances)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.analytics_report_instance_response import AnalyticsReportInstanceResponse
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
    api_instance = openapi_client.AnalyticsReportInstancesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_analytics_report_instances = ['fields_analytics_report_instances_example'] # List[str] | the fields to include for returned resources of type analyticsReportInstances (optional)

    try:
        api_response = api_instance.analytics_report_instances_get_instance(id, fields_analytics_report_instances=fields_analytics_report_instances)
        print("The response of AnalyticsReportInstancesApi->analytics_report_instances_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AnalyticsReportInstancesApi->analytics_report_instances_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_analytics_report_instances** | [**List[str]**](str.md)| the fields to include for returned resources of type analyticsReportInstances | [optional] 

### Return type

[**AnalyticsReportInstanceResponse**](AnalyticsReportInstanceResponse.md)

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
**200** | Single AnalyticsReportInstance |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **analytics_report_instances_segments_get_to_many_related**
> AnalyticsReportSegmentsResponse analytics_report_instances_segments_get_to_many_related(id, fields_analytics_report_segments=fields_analytics_report_segments, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.analytics_report_segments_response import AnalyticsReportSegmentsResponse
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
    api_instance = openapi_client.AnalyticsReportInstancesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_analytics_report_segments = ['fields_analytics_report_segments_example'] # List[str] | the fields to include for returned resources of type analyticsReportSegments (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.analytics_report_instances_segments_get_to_many_related(id, fields_analytics_report_segments=fields_analytics_report_segments, limit=limit)
        print("The response of AnalyticsReportInstancesApi->analytics_report_instances_segments_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AnalyticsReportInstancesApi->analytics_report_instances_segments_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_analytics_report_segments** | [**List[str]**](str.md)| the fields to include for returned resources of type analyticsReportSegments | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AnalyticsReportSegmentsResponse**](AnalyticsReportSegmentsResponse.md)

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
**200** | List of AnalyticsReportSegments |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **analytics_report_instances_segments_get_to_many_relationship**
> AnalyticsReportInstanceSegmentsLinkagesResponse analytics_report_instances_segments_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.analytics_report_instance_segments_linkages_response import AnalyticsReportInstanceSegmentsLinkagesResponse
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
    api_instance = openapi_client.AnalyticsReportInstancesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.analytics_report_instances_segments_get_to_many_relationship(id, limit=limit)
        print("The response of AnalyticsReportInstancesApi->analytics_report_instances_segments_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AnalyticsReportInstancesApi->analytics_report_instances_segments_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AnalyticsReportInstanceSegmentsLinkagesResponse**](AnalyticsReportInstanceSegmentsLinkagesResponse.md)

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

